---
title: siteSource 资源类型
description: 与保管人关联的网站的容器。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 60b2d8fb3374dd4f97dcff802caf509e66ca6db1
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597593"
---
# <a name="sitesource-resource-type"></a>siteSource 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

与 [保管人](custodian.md)关联的网站的容器。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 siteSources](../api/custodian-list-sitesources.md)|[siteSource](../resources/sitesource.md) 集合|获取 **siteSource** 对象及其属性的列表。|
|[创建 siteSource](../api/custodian-post-sitesources.md)|[siteSource](../resources/sitesource.md)|创建新的 **siteSource** 对象。|
|[获取 siteSource](../api/sitesource-get.md)|[siteSource](../resources/sitesource.md)|读取 **siteSource** 对象的属性和关系。|
|[删除 siteSource](../api/sitesource-delete.md)|无|删除 **siteSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|createdBy|[identitySet](../resources/identityset.md)|创建 **siteSource** 的用户。|
|createdDateTime|DateTimeOffset|**SiteSource** 的创建日期和时间。|
|displayName|String|**SiteSource** 的显示名称。 这将是 SharePoint 网站的名称。|
|id|String| **SiteSource** 的 ID。 这不是实际网站的 ID。|

## <a name="relationships"></a>关系

|关系|类型|Description|
|:---|:---|:---|
|网站|[site](../resources/site.md)|与 **siteSource** 相关联的 SharePoint 网站。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.siteSource",
  "baseType": "microsoft.graph.dataSource",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.siteSource",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "id": "String (identifier)"
}
```
