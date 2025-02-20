### @explicitHints 1
### @flyoutOnly true

# Anomaly 2

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
})

```

## الكائنات المشبوهة 2 @showdialog
إنه كائن مشبوه أخر!   
![Anomaly](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_3.jpg)


## أوقف المشبوهين
This is a different anomaly! Add another rule to stop this particular anomaly. 
Can you see anything that might help us distinguish between a villager and the anomaly?   
Remember, you can press the < (خلف) button to check the lookout view again.


```template
cyber.setupFirewall(function () {
cyber.allowAll()
cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
})
```

### ~ tutorialhint
هل يرتدي هؤلاء القرويون قبعات؟


```package
cyber-expert-daring-defense=github:ReWrite-Media/daring-defense-ts-ar/
```