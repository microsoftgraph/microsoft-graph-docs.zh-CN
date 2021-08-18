---
title: win32LobAppFileSystemDetection 资源类型
description: 包含用于检测 Win32 应用的文件或文件夹路径
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 1448a08261dd4140f5882f68bb8c40b4a97fe593651ddc61f9b904f918070266
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54156455"
---
# <a name="win32lobappfilesystemdetection-resource-type"></a>win32LobAppFileSystemDetection 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含用于检测 Win32 应用的文件或文件夹路径


继承自 [win32LobAppDetection](../resources/intune-apps-win32lobappdetection.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|路径|String|用于检测 Win32 业务线应用或 LoB (的文件) 路径|
|fileOrFolderName|String|用于检测 Win32 业务线或 LoB (应用) 名称|
|check32BitOn64System|布尔值|指示此文件或文件夹是否用于检查 64 位系统上的 32 位应用的值|
|detectionType|[win32LobAppFileSystemDetectionType](../resources/intune-apps-win32lobappfilesystemdetectiontype.md)|文件系统检测类型。 可取值为：`notConfigured`、`exists`、`modifiedDate`、`createdDate`、`version`、`sizeInMB` 或 `doesNotExist`。|
|operator|[win32LobAppDetectionOperator](../resources/intune-apps-win32lobappdetectionoperator.md)|文件或文件夹检测的运算符。 可取值为：`notConfigured`、`equal`、`notEqual`、`greaterThan`、`greaterThanOrEqual`、`lessThan` 或 `lessThanOrEqual`。|
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




