---
title: 保管人资源类型
description: 在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: 6c6b2befbb4066b851e38e6e17fd8be5aa59b031
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50157678"
---
# <a name="custodian-resource-type"></a>保管人资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出保管人](../api/ediscoverycase-list-custodians.md)|[custodian](../resources/custodian.md) collection|获取保管 **人对象及其** 属性的列表。|
|[创建保管人](../api/ediscoverycase-post-custodians.md)|[custodian](../resources/custodian.md)|创建新的保管 **人** 对象。|
|[获取保管人](../api/custodian-get.md)|[custodian](../resources/custodian.md)|读取保管人对象 **的属性** 和关系。|
|[更新保管人](../api/custodian-update.md)|[custodian](../resources/custodian.md)|更新保管人 **对象** 的属性。|
|[release](../api/custodian-release.md)|无|从案例释放保管人。|
|[activate](../api/custodian-activate.md)|无|重新激活从案例释放的保管人，并再次将其作为案例的一部分。|
|[列出 siteSources](../api/custodian-list-sitesources.md)|[siteSource](../resources/sitesource.md) 集合|从 **siteSources** 导航属性获取 **siteSource** 资源。|
|[创建 siteSources](../api/custodian-post-sitesources.md)|[siteSource](../resources/sitesource.md)|创建新的 **siteSource** 对象。|
|[列出 unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合|从 **unifiedGroupSources** 导航属性获取 **unifiedGroupSource** 资源。|
|[创建 unifiedGroupSources](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|创建新的 **unifiedGroupSource** 对象。|
|[列出 userSources](../api/custodian-list-usersources.md)|[userSource](../resources/usersource.md) 集合|从 **userSources** 导航属性获取 **userSource** 资源。|
|[创建 userSources](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|创建新的 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|保管人确认保留通知的日期和时间。|
|applyHoldToSources|布尔|标识保管人的来源在创建过程中是否处于保留状态。|
|createdDateTime|DateTimeOffset|将保管人添加到案例的日期和时间。|
|displayName|String|保管人显示名称。|
|email|String|保管人的电子邮件地址。|
|id|String|指定情况下保管人 ID。 只读。|
|lastModifiedDateTime|DateTimeOffset|保管人对象的上次修改日期和时间|
|releasedDateTime|DateTimeOffset|保管人从案例中释放的日期和时间。|
|status|custodianStatus|保管人的状态。 可取值为：`active`、`released`。|

### <a name="custodianstatus-values"></a>custodianStatus 值

|成员|说明|
|:----|-----------|
|active|保管人是案例的活跃部分。 |
|released|保管人从案例中释放。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|siteSources|[siteSource](../resources/sitesource.md) 集合|与保管人关联的 SharePoint 网站的数据源实体。|
|unifiedGroupSources|[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合|与保管人关联的组的数据源实体。|
|userSources|[userSource](../resources/usersource.md) 集合|保管人数据源实体。 这是保管人邮箱和 OneDrive for Business 网站的容器。|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.custodian",
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
