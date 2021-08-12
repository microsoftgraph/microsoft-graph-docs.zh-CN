---
title: '显示 Microsoft Graph Toolkit组件从右到左 (rtl) '
description: 介绍 Microsoft (组件) 从右向左Graph Toolkit rtl。
localization_priority: Normal
author: vogtn
ms.openlocfilehash: fce2d055ae5e859fe65d06edffb99039b8e258bec601f33b3ada8f5b2c671f1e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54129546"
---
# <a name="display-microsoft-graph-toolkit-components-right-to-left-rtl"></a>显示 Microsoft Graph Toolkit组件从右到左 (rtl) 

Microsoft Graph Toolkit 组件支持从右向左语言脚本的双向标记。

若要更改页面上所有组件的方向，请设置 document 或 tag 上的 属性 `dir` `html` `body` ， `rtl` 如以下示例所示。

```html
<body dir="rtl"></body>
```

或者

```html
<html dir="rtl"></html>
```

![从右向左](../images/rightToLeft.png)
