---
title: 保管人资源类型
description: 在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。
author: mahage-msft
localization_priority: Normal
ms.prod: compliance
doc_type: resourcePageType
ms.openlocfilehash: a2e22f711eaec4cd68cc5026e36b900d5284e71a
ms.sourcegitcommit: f729068e1fbb6b0f34a3d6144b59ec9aafcd8a62
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49597595"
---
# <a name="custodian-resource-type"></a>保管人资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

在电子数据展示的上下文中，表示用户及其所有数字资产，如电子邮件和文档。

## <a name="methods"></a>方法

|方法|返回类型|Description|
|:---|:---|:---|
|[列出保管人](../api/ediscoverycase-list-custodians.md)|[保管人](../resources/custodian.md) 集合|获取 **保管人** 对象及其属性的列表。|
|[创建管理员](../api/ediscoverycase-post-custodians.md)|[保管人](../resources/custodian.md)|创建新的 **保管人** 对象。|
|[获取管理员](../api/custodian-get.md)|[保管人](../resources/custodian.md)|读取 **保管人** 对象的属性和关系。|
|[更新管理员](../api/custodian-update.md)|[保管人](../resources/custodian.md)|更新 **保管人** 对象的属性。|
|[7.2](../api/custodian-release.md)|无|从案例发布管理员。|
|[启用](../api/custodian-activate.md)|无|重新激活已从某个事例发布的管理员，并再次使其成为事例的一部分。|
|[列出 siteSources](../api/custodian-list-sitesources.md)|[siteSource](../resources/sitesource.md) 集合|从 **siteSources** 导航属性中获取 **siteSource** 资源。|
|[创建 siteSources](../api/custodian-post-sitesources.md)|[siteSource](../resources/sitesource.md)|创建新的 **siteSource** 对象。|
|[列出 unifiedGroupSources](../api/custodian-list-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合|从 **unifiedGroupSources** 导航属性中获取 **unifiedGroupSource** 资源。|
|[创建 unifiedGroupSources](../api/custodian-post-unifiedgroupsources.md)|[unifiedGroupSource](../resources/unifiedgroupsource.md)|创建新的 **unifiedGroupSource** 对象。|
|[列出 userSources](../api/custodian-list-usersources.md)|[userSource](../resources/usersource.md) 集合|从 **userSources** 导航属性中获取 **userSource** 资源。|
|[创建 userSources](../api/custodian-post-usersources.md)|[userSource](../resources/usersource.md)|创建新的 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|Description|
|:---|:---|:---|
|acknowledgedDateTime|DateTimeOffset|管理员确认保留通知的日期和时间。|
|applyHoldToSources|布尔值|标识在创建过程中是否将保管人的源置于保留状态。|
|createdDateTime|DateTimeOffset|向事例中添加管理员的日期和时间。|
|displayName|String|保管人的显示名称。|
|email|String|保管人的电子邮件地址。|
|id|String|指定的事例中保管人的 ID。 只读。|
|lastModifiedDateTime|DateTimeOffset|上次修改保管人对象的日期和时间|
|releasedDateTime|DateTimeOffset|从事例中释放保管人的日期和时间。|
|status|custodianStatus|保管人的状态。 可取值为：`active`、`released`。|

### <a name="custodianstatus-values"></a>custodianStatus 值

|成员|说明|
|:----|-----------|
|工作|保管人是事例的活动部分。 |
|以后|在此情况下，将发布保管人。|

## <a name="relationships"></a>关系

|关系|类型|Description|
|:---|:---|:---|
|siteSources|[siteSource](../resources/sitesource.md) 集合|与保管人关联的 SharePoint 网站的数据源实体。|
|unifiedGroupSources|[unifiedGroupSource](../resources/unifiedgroupsource.md) 集合|与保管人关联的组的数据源实体。|
|userSources|[userSource](../resources/usersource.md) 集合|保管人的数据源实体。 这是用于保管人邮箱和 OneDrive for business 网站的容器。|

<!--|lastIndexOperation|[caseIndexOperation](../resources/caseindexoperation.md)|**TODO: Add Description**| -->

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.custodian",
  "baseType": "",
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
