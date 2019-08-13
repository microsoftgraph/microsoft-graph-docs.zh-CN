---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 08a1ed7d56c41eee69ee907a9efd91c12fad9b4e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36373257"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>windowsInformationProtectionApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于 Windows 信息保护的应用

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|应用显示名称。|
|说明|字符串|应用的说明。|
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



