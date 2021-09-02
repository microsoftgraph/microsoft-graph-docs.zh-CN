---
title: windowsAppIdentifier 资源类型
description: 应用应用的Windows标识符。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6eb5275d6b2c690f75b8ea5e72bb0bd9edab59a8
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58795506"
---
# <a name="windowsappidentifier-resource-type"></a>windowsAppIdentifier 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用应用的Windows标识符。


继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|windowsAppId|String|应用的标识符，如应用商店中指定。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsAppIdentifier",
  "windowsAppId": "String"
}
```



