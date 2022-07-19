---
title: ediscoveryCustodian 资源类型
description: 在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: b9edba3e4521177e26b3b13d409c4a6c7c1ea025
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/18/2022
ms.locfileid: "66837546"
---
# <a name="ediscoverycustodian-resource-type"></a>ediscoveryCustodian 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryCustodians](../api/security-ediscoverycase-list-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 集合|获取 [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 对象及其属性的列表。|
|[创建 ediscoveryCustodian](../api/security-ediscoverycase-post-custodians.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|创建新的 [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 对象。|
|[获取 ediscoveryCustodian](../api/security-ediscoverycustodian-get.md)|[microsoft.graph.security.ediscoveryCustodian](../resources/security-ediscoverycustodian.md)|读取 [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 对象的属性和关系。|
|[updateIndex](../api/security-ediscoverycustodian-updateindex.md)|触发 indexOperation，使保管人和关联的源可搜索。|
|[激活](../api/security-ediscoverycustodian-activate.md)|无|从事例中重新激活保管人。|
|[释放](../api/security-ediscoverycustodian-release.md)|无|从案例中释放保管人。|
|[applyHold](../api/security-ediscoverycustodian-applyhold.md)|无|开始将保留应用到电子数据展示保管人的过程。|
|[removeHold](../api/security-ediscoverycustodian-removehold.md)|无|开始从电子数据展示保管人中删除保留的过程。|
|[列出 ediscoveryIndexOperation](../api/security-ediscoverycustodian-list-lastindexoperation.md)|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md) 集合|获取与 [ediscoveryCustodian](../resources/security-ediscoverycustodian.md) 关联的 [ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md) 的列表。|
|[列出 siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md) 集合|从 siteSources 导航属性获取 siteSource 资源。|
|[创建 siteSource](../api/security-ediscoverycustodian-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|创建与[电子数据展示保管人](../resources/security-ediscoverycustodian.md)关联的新 [siteSource](../resources/security-sitesource.md) 对象。|
|[列出 unifiedGroupSources](../api/security-ediscoverycustodian-list-unifiedgroupsources.md)|[microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md) 集合|从 unifiedGroupSources 导航属性获取 unifiedGroupSource 资源。|
|[创建 unifiedGroupSource](../api/security-ediscoverycustodian-post-unifiedgroupsources.md)|[microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md)|创建与[电子数据展示保管人](../resources/security-ediscoverycustodian.md)关联的新 [unifiedGroupSource](../resources/security-unifiedgroupsource.md) 对象。|
|[列出 userSources](../api/security-ediscoverycustodian-list-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md) 集合|从 userSources 导航属性获取 userSource 资源。|
|[创建 userSource](../api/security-ediscoverycustodian-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|创建与[电子数据展示保管人](../resources/security-ediscoverycustodian.md)关联的新 [userSource](../resources/security-usersource.md) 对象。|

## <a name="properties"></a>属性
|属性|类型|描述|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|保管人确认保留通知的日期和时间。|
|createdDateTime|DateTimeOffset|将保管人添加到事例的日期和时间。|
|displayName|String|保管人显示名称。|
|email|String|Email保管人地址。|
|id|String|指定情况下的保管人 ID。 只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改保管人对象的日期和时间|
|releasedDateTime|DateTimeOffset|保管人从案例中释放的日期和时间。|
|status|microsoft.graph.security.dataSourceContainerStatus|保管人状态。 可取值为：`active`、`released`。|
|holdStatus|microsoft.graph.security.dataSourceHoldStatus|保管人保留状态。可能的值为： `notApplied`， `applied`， `applying`， `removing``partial`|

### <a name="custodianstatus-values"></a>保管人Status 值

|名称|说明|
|:----|-----------|
|积极|保管人是本案的活跃部分。 |
|释放|保管人已从案例中释放。|

### <a name="custodianholdstatus-values"></a>保管人HoldStatus 值

|名称|说明|
|:----|-----------|
|notApplied|保管人不在“保留”状态 (其中的所有源都未被搁置) 。|
|应用|保管人处于保留状态 (所有源都保留) 。|
|应用|保管人正在应用保留状态 () 触发的 applyHold 操作。|
|删除|保管人正在删除 () 触发的 removeHold 操作的保留状态。|
|部分|保管人处于混合状态，其中某些源处于保留状态，有些源未处于保留或错误状态。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|lastIndexOperation|[microsoft.graph.security.ediscoveryIndexOperation](../resources/security-ediscoveryindexoperation.md)|表示保管人的最新索引的操作实体。|
|siteSources|[microsoft.graph.security.siteSource](../resources/security-sitesource.md) 集合|与保管人关联的 SharePoint 网站的数据源实体。|
|unifiedGroupSources|[microsoft.graph.security.unifiedGroupSource](../resources/security-unifiedgroupsource.md) 集合|与保管人关联的组的数据源实体。|
|userSources|[microsoft.graph.security.userSource](../resources/security-usersource.md) 集合|保管人的数据源实体。 这是保管人的邮箱和OneDrive for Business网站的容器。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryCustodian",
  "baseType": "microsoft.graph.security.dataSourceContainer",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryCustodian",
  "id": "String (identifier)",
  "status": "String",
  "holdStatus": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "displayName": "String",
  "createdDateTime": "String (timestamp)",
  "email": "String",
  "acknowledgedDateTime": "String (timestamp)"
}
```

