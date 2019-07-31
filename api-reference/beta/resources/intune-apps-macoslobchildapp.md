---
title: macOSLobChildApp 资源类型
description: 包含捆绑包包中的 MacOS LOB 应用程序的属性
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4ca4d371966781378c9097769d9178de69d8f7d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36012588"
---
# <a name="macoslobchildapp-resource-type"></a>macOSLobChildApp 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含捆绑包包中的 MacOS LOB 应用程序的属性

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|标识名称。|
|buildNumber|String|MacOS 业务线 (LoB) 应用的内部版本号。|
|versionNumber|String|MacOS 业务线 (LoB) 应用的版本号。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSLobChildApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSLobChildApp",
  "bundleId": "String",
  "buildNumber": "String",
  "versionNumber": "String"
}
```





