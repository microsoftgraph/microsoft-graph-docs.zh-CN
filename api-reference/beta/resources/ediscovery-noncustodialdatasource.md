---
title: noncustodialDataSource 资源类型
description: 通过非托管数据源，你可以向案例添加数据，而无需将其与保管人关联
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 238a09015efa5f445dcc92390ee7a8eff19d8df5
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115188"
---
# <a name="noncustodialdatasource-resource-type"></a>noncustodialDataSource 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

通过非托管数据源，您可以向案例添加数据，而无需将其与保管人关联。 若要了解更多信息，请访问将[非托管数据源添加到Advanced eDiscovery案例](/microsoft-365/compliance/non-custodial-data-sources)

继承自 [dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出 noncustodialDataSources](../api/ediscovery-noncustodialdatasource-list.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 集合|获取 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象及其属性的列表。|
|[获取 noncustodialDataSource](../api/ediscovery-noncustodialdatasource-get.md)|[microsoft.graph.ediscovery.noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md)|读取 [noncustodialDataSource](../resources/ediscovery-noncustodialdatasource.md) 对象的属性和关系。|
|[Release dataSource](../api/ediscovery-noncustodialdatasource-release.md)|None|释放非安全数据源。|
|[列出 dataSource](../api/ediscovery-noncustodialdatasource-list-datasource.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md) 集合|从 dataSource 导航属性获取 dataSource 资源。|
|[创建 dataSource](../api/ediscovery-noncustodialdatasource-post.md)|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|创建新的 dataSource 对象。|

## <a name="properties"></a>属性

|属性|类型|Description|
|:---|:---|:---|
|applyHoldToSource|布尔|指示是否将保留应用于非 (数据源，如邮箱或网站) 。|
|createdDateTime|DateTimeOffset|创建 nonCustodialDataSource 的日期和时间。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|displayName|String|noncustodialDataSource 的显示名称。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|id|String|nonCustodialDataSource 的唯一标识符。 继承自 [实体](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|nonCustodialDataSource 的上次修改日期和时间。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|releasedDateTime|DateTimeOffset|从案例发布 nonCustodialDataSource 的日期和时间。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|状态|microsoft.graph.ediscovery.dataSourceContainerStatus|nonCustodialDataSource 的最新状态。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。 可取值为：`Active`、`Released`。|

## <a name="relationships"></a>关系

|关系|类型|Description|
|:---|:---|:---|
|dataSource|[microsoft.graph.ediscovery.dataSource](../resources/ediscovery-datasource.md)|用户源SharePoint网站数据源作为非安全数据源。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.noncustodialDataSource",
  "baseType": "microsoft.graph.ediscovery.dataSourceContainer",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.noncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "applyHoldToSource": "Boolean"
}
```