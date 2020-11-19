---
title: macOSSystemExtension 资源类型
description: 表示特定的 macOS 系统扩展。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 8cea7fb3cb7c0c95fb0ad5174b171bc1993aa1fb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49294023"
---
# <a name="macossystemextension-resource-type"></a>macOSSystemExtension 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示特定的 macOS 系统扩展。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|teamIdentifier|字符串|获取或设置用于对系统扩展进行签名的团队标识符。|
|bundleId|String|获取或设置系统扩展的捆绑包标识符。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtension"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtension",
  "teamIdentifier": "String",
  "bundleId": "String"
}
```




