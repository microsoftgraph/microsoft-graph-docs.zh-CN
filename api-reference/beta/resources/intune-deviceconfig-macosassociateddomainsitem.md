---
title: macOSAssociatedDomainsItem 资源类型
description: 应用程序标识符到关联域的映射。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6fa40fda83eb6dd89fa0d8fd709a8bf744a8cc19
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736252"
---
# <a name="macosassociateddomainsitem-resource-type"></a>macOSAssociatedDomainsItem 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用程序标识符到关联域的映射。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|applicationIdentifier|String|要与域关联的应用程序的应用程序标识符。|
|域|String collection|要关联的域的列表。|
|directDownloadsEnabled|布尔|确定是应直接下载数据还是通过 CDN 下载数据。|

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





