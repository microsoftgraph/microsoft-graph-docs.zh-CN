---
title: retentionDurationInDays 资源类型
description: 表示项目在删除之前将保留的天数
author: sseth
ms.localizationpriority: medium
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 4f8546d98e5430651ae672737e3d32a5e4744738
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66447572"
---
# <a name="retentiondurationindays-resource-type"></a>retentionDurationInDays 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示项目在删除之前将保留的天数。


继承自 [retentionDuration](../resources/security-retentionduration.md)。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|天|Int32|指定将保留具有已应用保留标签的项目的时间段（以天为单位）。|

## <a name="relationships"></a>关系
无。

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.security.retentionDurationInDays"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.retentionDurationInDays",
  "days": "Integer"
}
```