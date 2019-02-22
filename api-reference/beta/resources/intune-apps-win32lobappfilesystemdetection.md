---
title: win32LobAppFileSystemDetection 资源类型
description: 包含用于检测 Win32 应用程序的文件或文件夹路径
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c8145e6196b6537eec4142d4412a11234913df7c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157510"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>win32LobAppFileSystemDetection 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用程序的文件或文件夹路径


继承自[win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|路径|字符串|用于检测 Win32 业务线 (LoB) 应用程序的文件或文件夹路径|
|fileOrFolderName|字符串|要检测 Win32 业务线 (LoB) 应用程序的文件或文件夹名称|
|check32BitOn64System|布尔|一个指示此文件或文件夹是否用于检查64位系统上的32位应用程序的值|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|文件系统检测类型。 可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB`。|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|用于 file 或 fodler 检测的运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan`、`lessThanOrEqual`。|
|detectionValue|字符串|文件或文件夹检测值|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.win32LobAppFileSystemDetection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.win32LobAppFileSystemDetection",
  "path": "String",
  "fileOrFolderName": "String",
  "check32BitOn64System": true,
  "detectionType": "String",
  "operator": "String",
  "detectionValue": "String"
}
```




