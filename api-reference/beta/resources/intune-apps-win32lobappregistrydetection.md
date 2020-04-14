---
title: win32LobAppRegistryDetection 资源类型
description: 包含用于检测 Win32 应用程序的注册表属性
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 2b6f28d6c042ab86273cd11d9e756bb4941e315b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43422737"
---
# <a name="win32lobappregistrydetection-resource-type"></a>win32LobAppRegistryDetection 资源类型

命名空间：microsoft.graph

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用程序的注册表属性


继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|check32BitOn64System|Boolean|一个值，该值指示此注册表路径是否用于检查64位系统上的32位应用|
|keyPath|String|用于检测 Win32 业务线（LoB）应用程序的注册表项路径|
|等值|String|注册表值名称|
|detectionType|[win32LobAppRegistryDetectionType](../resources/intune-apps-win32lobappregistrydetectiontype.md)|注册表数据检测类型。 可取值为：`notConfigured`、`exists`、`doesNotExist`、`string`、`integer`、`version`。|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|用于注册表数据检测的运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。|
|detectionValue|String|注册表检测值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppRegistryDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppRegistryDetection",
  "check32BitOn64System": true,
  "keyPath": "String",
  "valueName": "String",
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```



