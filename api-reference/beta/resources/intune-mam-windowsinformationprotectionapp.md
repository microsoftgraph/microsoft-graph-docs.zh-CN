---
title: windowsInformationProtectionApp 资源类型
description: 用于 Windows 信息保护的应用
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e2b8739fd045d4b8e6293164fc7e9b14154a475c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30139282"
---
# <a name="windowsinformationprotectionapp-resource-type"></a>windowsInformationProtectionApp 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于 Windows 信息保护的应用

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|应用显示名称。|
|description|字符串|应用的说明。|
|publisherName|String|发布者名称|
|productName|String|产品名称。|
|denied|布尔值|如果为 true，则应用的保护或免除受到拒绝。|

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




