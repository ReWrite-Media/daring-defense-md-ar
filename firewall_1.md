### @explicitHints 1
### @flyoutOnly true

# السماح بكل شيء

## ما هو جدار الحماية؟ @unplugged
جدار الحماية هو نظام تصفية يستخدم للتحكم في حركة المرور الداخلة والخارجة من شبكة أو موقع معين.  يعتمد هذا النظام على مجموعة من القواعد المحددة التي تحدد ما إذا كان يجب السماح أو رفض حركة معينة، مما يتيح أو يمنع أنواعا مختلفة من حركة المرور، في هذه المهمة، ستقوم بوضع مجموعة من القواعد لتحديد ما إذا كان يُسمح لشخصيات مختلفة بدخول القلعة أو لا.

## القرويين @unplugged
يبدو أن هناك مجموعة من القرويين (سكان القرية) في طريقهم إلى القلعة. يجب أن نسمح لهم بالدخول. لنبدأ بإنشاء جدار حماية يسمح للجميع بالدخول.
![Villages](https://raw.githubusercontent.com/CausewayDigital/Minecraft-EE-MakeCode/main/tutorials/cyber-kingdom/firewall/images/level_1.jpg)
## الخطوة الأولى
يبدو أن هناك مجموعة من القرويين  في طريقهم إلى القلعة. لنبدأ بإنشاء جدار حماية يسمح للجميع بالدخول. عندما تكون مستعدا لتجربة جدار الحماية، اضغط على زر التشغيل.
```template
cyber.setupFirewall(function () {
})
```

### ~ tutorialhint
```blocks
cyber.setupFirewall(function () {
    cyber.allowAll()
})

```

```package
cyber-expert-daring-defense=github:ReWrite-Media/daring-defense-ts-ar/
```