### @explicitHints 1
### @flyoutOnly true

# الجنود

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
    cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireLegs(Legs.OverFourLegs), cyber.requireHoldingItem(HoldingItem.NoItem)))
    cyber.addDenyFirewallRule(cyber.requireEyewear(WearingEyeware.WearingEyeware))
    cyber.addDenyFirewallRule(cyber.requireCrest(cyber.createGridString(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)))
})

```

## الجنود@showdialog
يبدو أن المملكة المنافسة غير راضية عن حظرنا دخول جواسيسها إلى مملكننا، وقد أقدمت على إرسال جنود!
![Soldiers](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_6.jpg)


## جنود!
بسرعة، قم بإنشاء بعض القواعد لمنع هؤلاء الجنود من المرور عبر أسوار القلعة! يمكننا تمييزهم من خلال شعارهم الملكي على الدروع . جنودنا يحملون شعارا **ذهبيا** و**بنفسجيا**، ويجب السماح لهم بالدخول.


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireHat(WearingHat.NoHat), cyber.requireHoldingItem(HoldingItem.NoItem)))
cyber.addDenyFirewallRule(cyber.requireEyewear(WearingEyeware.WearingEyeware))
})
```

### ~ tutorialhint
أعط اهتماما خاصا لدروع الجنود، هل يمكننا تصفية الجنود حسب تلك الدروع؟ لكن تأكد من عدم حظر جنودنا!
![Soldiers Shields](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_6_shields.jpg)



```package
cyber-expert-daring-defense=github:ReWrite-Media/daring-defense-ts-ar/
```