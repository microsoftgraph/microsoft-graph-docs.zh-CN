---
title: identitySet 资源类型
description: 标识集
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 427c627ac25e7ed795f6891c3deac470471b2ee8
ms.sourcegitcommit: 4a960067cf2cd7d3c605550150eb3c9259adfe92
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/19/2021
ms.locfileid: "60481586"
---
# <a name="identityset-resource-type"></a>identitySet 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

标识集

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|application|[Identity](../resources/intune-rbac-identity.md)|应用程序的标识。 此属性是只读的。|
|设备|[identity](../resources/intune-rbac-identity.md)|设备的标识。 此属性是只读的。|
|用户|[identity](../resources/intune-rbac-identity.md)|用户的标识。 此属性是只读的。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identitySet"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.identitySet",
  "application": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  },
  "device": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  },
  "user": {
    "@odata.type": "microsoft.graph.identity",
    "id": "String",
    "displayName": "String"
  }
}
```



