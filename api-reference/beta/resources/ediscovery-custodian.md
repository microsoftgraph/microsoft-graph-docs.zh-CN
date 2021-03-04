---
title: 保管人资源类型
description: 在电子数据展示上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: mahage-msft
localization_priority: Normal
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 0d71542b796f5256f21e19a886533e3a88e1d7ed
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446658"
---
# <a name="custodian-resource-type"></a>保管人资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在电子数据展示上下文中，表示用户及其所有数字资产，如电子邮件和文档。

## <a name="methods"></a>Methods

|方法|返回类型|说明|
|:---|:---|:---|
|[列出保管人](../api/ediscovery-case-list-custodians.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md) 集合|获取保管 **人对象及其** 属性的列表。|
|[创建保管人](../api/ediscovery-case-post-custodians.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|创建新的保管 **人** 对象。|
|[获取保管人](../api/ediscovery-custodian-get.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|读取保管人对象 **的属性** 和关系。|
|[更新保管人](../api/ediscovery-custodian-update.md)|[microsoft.graph.ediscovery.custodian](../resources/ediscovery-custodian.md)|更新保管人 **对象** 的属性。|
|[release](../api/ediscovery-custodian-release.md)|无|从案例释放保管人。|
|[activate](../api/ediscovery-custodian-activate.md)|无|重新激活从案例释放的保管人，并再次将其作为案例的一部分。|
|[列出 siteSources](../api/ediscovery-custodian-list-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合|获取与保管人关联的 **siteSource** 资源。|
|[创建 siteSources](../api/ediscovery-custodian-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|创建新的 **siteSource** 对象。|
|[列出 unifiedGroupSources](../api/ediscovery-custodian-list-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 集合|获取与 **保管人关联的 unifiedGroupSource** 资源列表。|
|[创建 unifiedGroupSources](../api/ediscovery-custodian-post-unifiedgroupsources.md)|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md)|创建新的 **unifiedGroupSource** 对象。|
|[列出 userSources](../api/ediscovery-custodian-list-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合|获取与 **保管人关联的 userSource** 资源列表。|
|[创建 userSources](../api/ediscovery-custodian-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|创建新的 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|保管人确认保留通知的日期和时间。|
|applyHoldToSources|布尔|标识保管人的来源在创建期间是否处于保留状态。|
|createdDateTime|DateTimeOffset|将保管人添加到案例的日期和时间。|
|displayName|String|保管人显示名称。|
|email|String|保管人的电子邮件地址。|
|id|String|指定情况下保管人 ID。 只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改保管人对象的日期和时间|
|releasedDateTime|DateTimeOffset|保管人从案例中释放的日期和时间。|
|status|microsoft.graph.ediscovery.custodianStatus|保管人的状态。 可取值为：`active`、`released`。|

### <a name="custodianstatus-values"></a>custodianStatus 值

|成员|说明|
|:----|-----------|
|active|Custodian 是案例的一个活动部分。 |
|released|保管人从案例中释放。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|siteSources|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合|与保管人关联的 SharePoint 网站的数据源实体。|
|unifiedGroupSources|[microsoft.graph.ediscovery.unifiedGroupSource](../resources/ediscovery-unifiedgroupsource.md) 集合|与保管人关联的组的数据源实体。|
|userSources|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合|保管人数据源实体。 这是保管人邮箱和 OneDrive for Business 网站的容器。|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.custodian",
  "email": "String",
  "applyHoldToSources": "Boolean",
  "status": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "releasedDateTime": "String (timestamp)",
  "acknowledgedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "displayName": "String"
}
```
