### @explicitHints 1
### @flyoutOnly true

# Anomaly 1

```ghost
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireHat(WearingHat.NoHat))
    cyber.addDenyFirewallRule(cyber.requireHoldingItem(HoldingItem.NoItem))
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.TwoLegs))
})

```

## Anomaly 1 @showdialog
هناك بعض الكائنات المشبوهة! يبدو أن هذا الكائن يمتلك العديد من الأرجل ويحاول اقتحام القلعة...
 يجب أن نضع قاعدة لمنعه من الدخول إليها.![Anomaly](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_2.jpg)


## Deny rule
يجب علينا وضع قاعدة تمنع وصول الكائنات المشبوهة إلى القلعة، مع السماح للقرويين بالدخول. 
قم بإضافة البلوك  ``||cyber:إضافة قاعدة رفض  إلى جدار الحماية||`` إلى قواعدك، حيث تتيح لك هذه القاعدة إبلاغ الحراس برفض دخول أي شيء تنطبق عليه.

### Distinguishing Features
هل تلاحظ أي شيء قد يساعدنا في التمييز بين القروي وهذه الكائنات المشبوهة؟   
اضغط على الزر < (خلف) لتحقق من المظهر لمتابعة ما هو قادم إذا كنت غير متأكد من ماهيته.
```template
cyber.setupFirewall(function () {
cyber.allowAll()
})
```

### ~ tutorialhint
```blocks
cyber.setupFirewall(function () {
    cyber.allowAll()
    cyber.addDenyFirewallRule(cyber.requireLegs(Legs.OverFourLegs))
})

```

```package
cyber-expert-daring-defense=github:ReWrite-Media/daring-defense-ts-ar/
```
