---
title: ediscoveryNoncustodialDataSource 资源类型
description: 使用非保管数据源可将数据添加到事例，而无需将其关联到保管人。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: fcf2022747ee7b98526d522eecc268be2def490d
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945166"
---
# <a name="ediscoverynoncustodialdatasource-resource-type"></a>ediscoveryNoncustodialDataSource 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

使用非保管数据源可将数据添加到案例，而无需将其关联到保管人。 若要了解详细信息，请访问 [将非托管数据源添加到高级电子数据展示案例 ](/microsoft-365/compliance/non-custodial-data-sources)


继承自 [dataSourceContainer](../resources/security-datasourcecontainer.md)。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryNoncustodialDataSources](../api/security-ediscoverysearch-list-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 集合|获取 [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 对象及其属性的列表。|
|[创建 ediscoveryNoncustodialDataSource](../api/security-ediscoverysearch-post-noncustodialsources.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|创建新的 [ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md) 对象。|
|[获取 ediscoveryNoncustodialDataSource](../api/security-ediscoverynoncustodialdatasource-get.md)|[microsoft.graph.security.ediscoveryNoncustodialDataSource](../resources/security-ediscoverynoncustodialdatasource.md)|读取 [ediscoveryNoncustodialDataSource 对象的](../resources/security-ediscoverynoncustodialdatasource.md) 属性和关系。|
|[updateIndex](../api/security-ediscoverynoncustodialdatasource-updateindex.md)|无|触发 indexOperation，使非保管数据源和关联的数据源可搜索。|
|[释放](../api/security-ediscoverynoncustodialdatasource-release.md)|无|从案例中释放非存储数据源。|
|[applyHold](../api/security-ediscoverynoncustodialdatasource-applyhold.md)|无|开始将保留应用到电子数据展示非托管数据源的过程。|
|[removeHold](../api/security-ediscoverynoncustodialdatasource-removehold.md)|无|开始从电子数据展示非存储数据源中删除保留的过程。|
|[列出 ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md) 集合|从 lastIndexOperation 导航属性获取 ediscoveryIndexOperation 资源。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|创建了非CustodialDataSource 的日期和时间。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|displayName|字符串|noncustodialDataSource 的显示名称。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|id|String|nonCustodialDataSource 的唯一标识符。 继承自 [entity](../resources/entity.md)。|
|lastModifiedDateTime|DateTimeOffset|非CustodialDataSource 的上次修改日期和时间。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|releasedDateTime|DateTimeOffset|非CustodialDataSource 从案例中释放的日期和时间。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。|
|status|String|nonCustodialDataSource 的最新状态。 继承自 [microsoft.graph.ediscovery.dataSourceContainer](../resources/ediscovery-datasourcecontainer.md)。 可取值为：`Active`、`Released`。|
|holdStatus|字符串|nonCustodialDataSource 的保留状态。可能的值为： `notApplied`， ， `applied`， `applying`， `removing``partial`|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|dataSource|[microsoft.graph.security.dataSource](../resources/security-datasource.md)|用户源或 SharePoint 站点数据源作为非保管数据源。|
|lastIndexOperation|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|表示非存储数据源的最新索引的操作实体。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryNoncustodialDataSource",
  "baseType": "microsoft.graph.security.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryNoncustodialDataSource",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```