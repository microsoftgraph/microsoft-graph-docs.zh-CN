---
title: macOSLobChildApp 资源类型
description: 包含捆绑包中的 MacOS LOB 应用的属性
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8a590ffdc3cb9e8d0a01724c9b6f2c37841817f5
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59020453"
---
# <a name="macoslobchildapp-resource-type"></a>macOSLobChildApp 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含捆绑包中的 MacOS LOB 应用的属性

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|bundleId|String|标识名称。|
|buildNumber|String|MacOS 业务线 (LoB 应用) 号。|
|versionNumber|String|MacOS 业务线 (LoB) 版本号。|

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



