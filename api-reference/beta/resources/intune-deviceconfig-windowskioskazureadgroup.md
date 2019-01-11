---
title: windowsKioskAzureADGroup 资源类型
description: 用于标识为网亭配置 AzureAD 组的类
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 16c2b17220a92f9f230b786238b1195e2af48d6b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849866"
---
# <a name="windowskioskazureadgroup-resource-type"></a>windowsKioskAzureADGroup 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

用于标识为网亭配置 AzureAD 组的类

继承自[windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|字符串|将锁定到此网亭配置 AzureAD 组的显示名称|
|groupId|字符串|将此网亭配置到锁定的 AzureAD 组 ID|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskAzureADGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskAzureADGroup",
  "displayName": "String",
  "groupId": "String"
}
```





