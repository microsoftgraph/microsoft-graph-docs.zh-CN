---
title: retentionDuration 资源类型
description: '表示内容在删除之前将保留多长时间。 '
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 943e5d18ef5c19dc309da3b26df9b34480cf392f
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447569"
---
# <a name="retentionduration-resource-type"></a>retentionDuration 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示项目在删除之前将保留多长时间。 这是一种抽象类型。 **retentionDuration** 资源是 [retentionDurationForever](../resources/security-retentiondurationforever.md) 和 [retnetionDurationInDays resourceTypes](../resources/security-retentiondurationindays.md) 的基础类型。

## <a name="properties"></a>属性
无。

## <a name="relationships"></a>关系
无。

## <a name="json-representation-for-retentionduration"></a>retentionDuration 的 JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionDuration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionDuration"
}
```


