### @explicitHints 1
### @flyoutOnly true

# دمج القواعد

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
    cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireLegs(Legs.OverFourLegs), cyber.requireHoldingItem(HoldingItem.NoItem)))
})

```

## More villagers @showdialog
يبدو أن هناك مجموعة كبيرة من القرويين في طريقهم إلى القلعة. 
هل سيسمح لهم جميعا  بالمرور عبر  جدار الحماية؟
![Villagers](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_4.jpg)


## More villagers
قد تحتاج لوضع قواعد باستخدام الحرف **و** مما يعني أنه يمكنك دمج قاعدتين معا. 
انتبه، فبعض هؤلاء القرويين لا يرتدون قبعات، لكنهم يحملون أشياء مثل فأس أو خريطة. وهذا يعني أنه لا يمكننا حظر أي شخص لا يرتدي قبعة فقط.


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
})
```

### ~ tutorialhint
يبدو أن الشخص المشبوه لا يرتدي قبعة ولا يحمل أي شيء.

```package
cyber-expert-daring-defense=github:ReWrite-Media/daring-defense-ts-ar/
```