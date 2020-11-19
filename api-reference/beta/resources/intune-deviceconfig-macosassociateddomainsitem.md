---
title: macOSAssociatedDomainsItem 资源类型
description: 应用程序标识符到关联域的映射。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 7b14cc5fe7c13bbcdde94733c41caf2b68c0451e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268935"
---
# <a name="macosassociateddomainsitem-resource-type"></a>macOSAssociatedDomainsItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用程序标识符到关联域的映射。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationIdentifier|字符串|要与域关联的应用程序的应用程序标识符。|
|域|String 集合|要关联的域的列表。|
|directDownloadsEnabled|Boolean|确定是应直接下载数据还是通过 CDN 下载数据。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSAssociatedDomainsItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSAssociatedDomainsItem",
  "applicationIdentifier": "String",
  "domains": [
    "String"
  ],
  "directDownloadsEnabled": true
}
```




