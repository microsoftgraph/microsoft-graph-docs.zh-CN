---
title: macOSSystemExtensionTypeMapping 资源类型
description: 表示 macOS 系统扩展和系统扩展类型的团队标识符之间的映射。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: d376b69e64b0e9dc5699918e748c6be91dc5fa7264986e96cff924533cdcd649
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54251517"
---
# <a name="macossystemextensiontypemapping-resource-type"></a>macOSSystemExtensionTypeMapping 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 系统扩展和系统扩展类型的团队标识符之间的映射。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|teamIdentifier|String|获取或设置用于对系统扩展进行签名的团队标识符。|
|allowedTypes|[macOSSystemExtensionType](../resources/intune-deviceconfig-macossystemextensiontype.md)|获取或设置允许的 macOS 系统扩展类型。 可取值为：`driverExtensionsAllowed`、`networkExtensionsAllowed`、`endpointSecurityExtensionsAllowed`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSSystemExtensionTypeMapping"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSSystemExtensionTypeMapping",
  "teamIdentifier": "String",
  "allowedTypes": "String"
}
```




