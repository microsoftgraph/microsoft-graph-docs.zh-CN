---
title: siteSource 资源类型
description: 与保管人关联的网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: c178565b628728fcf6124ea3058e979f8423ce90
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52080475"
---
# <a name="sitesource-resource-type"></a>siteSource 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与保管人 关联的网站的 [容器](ediscovery-custodian.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 siteSources](../api/ediscovery-custodian-list-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合|获取 **siteSource 对象** 及其属性的列表。|
|[创建 siteSource](../api/ediscovery-custodian-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|创建新的 **siteSource** 对象。|
|[获取 siteSource](../api/ediscovery-sitesource-get.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|读取 **siteSource** 对象的属性和关系。|
|[删除 siteSource](../api/ediscovery-sitesource-delete.md)|无|删除 **siteSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **siteSource 的用户**。|
|createdDateTime|DateTimeOffset|创建 **siteSource 的** 日期和时间。|
|displayName|String|siteSource 显示名称 **的一部分**。 这将是网站SharePoint的名称。|
|id|String| **siteSource** 的 ID。 可通过 Get site 随时检索 [网站源](../api/site-get.md) - https://graph.microsoft.com/v1.0/sites/{siteId}|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|网站|[site](../resources/site.md)|与SharePoint网站源 关联的 **网站**。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.siteSource",
  "baseType": "microsoft.graph.ediscovery.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
