---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7394ab6b8a0a81a005f7f6d8966214b17251ec0b
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58818749"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>windowsInformationProtectionApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于 Windows 信息保护的应用

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|应用显示名称。|
|description|String|应用的说明。|
|publisherName|String|发布者名称|
|productName|String|产品名称。|
|denied|Boolean|如果为 true，则应用的保护或免除受到拒绝。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionApp",
  "displayName": "String",
  "description": "String",
  "publisherName": "String",
  "productName": "String",
  "denied": true
}
```



