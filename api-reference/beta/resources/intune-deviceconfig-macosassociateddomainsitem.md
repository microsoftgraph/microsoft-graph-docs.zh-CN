---
title: macOSAssociatedDomainsItem 资源类型
description: 应用程序标识符到关联域的映射。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2658a02a4881e793879a68bc6d1822d9a9b2a0a5
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58819141"
---
# <a name="macosassociateddomainsitem-resource-type"></a>macOSAssociatedDomainsItem 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

应用程序标识符到关联域的映射。

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|applicationIdentifier|String|要与域关联的应用程序的应用程序标识符。|
|domains|String collection|要关联的域列表。|
|directDownloadsEnabled|Boolean|确定数据是应该直接下载还是通过 CDN。|

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



