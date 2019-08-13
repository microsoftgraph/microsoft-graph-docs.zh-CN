---
title: iosMobileAppIdentifier 资源类型
description: iOS 应用的标识符。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c4b3de2dd5dd25e5995e7a1d30ad4314bb34efa5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36332216"
---
# <a name="iosmobileappidentifier-resource-type"></a>iosMobileAppIdentifier 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

iOS 应用的标识符。


继承自 [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|应用的标识符，如应用商店中指定。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```



