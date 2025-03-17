### @explicitHints 1
### @flyoutOnly true

# الجواسيس والأعداء

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
    cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireLegs(Legs.OverFourLegs), cyber.requireHoldingItem(HoldingItem.NoItem)))
    cyber.addDenyFirewallRule(cyber.requireEyewear(WearingEyeware.WearingEyeware))
})

```

## الجواسيس والأعداء @showdialog
احذر، فقد عُرف عن المملكة المنافسة لمملكتنا سعيها لإرسال جواسيس يتسللون عبر بوابتنا![Spies](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_5.jpg)  


## الجواسيس والأعداء!
تأكد من عدم السماح للجواسيس بالدخول، فهم يحاولون التنكر حتى لا يتم التعرف عليهم.   
أتساءل كيف يمكن أن نمييز بينهم وبين القرويين العاديين؟


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
cyber.addDenyFirewallRule(cyber.ruleAnd(cyber.requireHat(WearingHat.NoHat), cyber.requireHoldingItem(HoldingItem.NoItem)))
})
```

### ~ tutorialhint
ماذا يرتدي الجواسيس عندما يرغبون في إخفاء هويتهم؟

```package
cyber-expert-daring-defense=github:ReWrite-Media/daring-defense-ts-ar/
```