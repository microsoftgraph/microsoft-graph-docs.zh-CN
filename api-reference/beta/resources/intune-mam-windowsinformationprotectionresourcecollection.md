---
title: windowsInformationProtectionResourceCollection 资源类型
description: Windows 信息保护资源集合
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 09a86848620bc5f8e5b51096c18e31763b373e166320ea1a902e4154184e9b21
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54147915"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a>windowsInformationProtectionResourceCollection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows 信息保护资源集合

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|显示名称|
|资源|字符串集合|资源集合|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```




