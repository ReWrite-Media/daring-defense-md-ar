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
هذا نوع أخر من الكائنات المشبوهة! أضف قاعدة أخرى لمنع هذا النوع من المشبوهين بالتحديد.
هل تلاحظ أي شيء قد يساعدنا في التمييز بين القروي وهذه الكائنات المشبوهة؟   
تذكر، يمكنك الضغط على الزر < (خلف) لتحقق من المظهر ومتابعة ما هو قادم إذا كنت غير متأكد من ماهيته.


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