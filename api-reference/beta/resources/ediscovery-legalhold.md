---
title: legalHold 资源类型
description: legalHold 资源类型
ms.localizationpriority: medium
author: mahage-msft
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 6de7272e31476a925f4e9e08f680e41b7b8fed14
ms.sourcegitcommit: 33e0bbada1b47310a18d8f794914b1319d88e6f4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2021
ms.locfileid: "61402872"
---
# <a name="legalhold-resource-type"></a>legalHold 资源类型

命名空间：microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示合法保留。 合法保留与电子数据展示案例关联。 法律保留不应与保留保留混淆，保留保留用于控制内容保留Microsoft 365策略。 电子数据展示法律保留用于无限期保留内容，以用于需要防止删除内容的诉讼、内部调查和其他法律操作。 有关详细信息，请参阅管理[Advanced eDiscovery](/microsoft-365/compliance/managing-holds)

继承自 [实体](../resources/entity.md)。

## <a name="methods"></a>方法

|方法|返回类型|说明|
|:---|:---|:---|
|[列出 legalHolds](../api/ediscovery-case-list-legalholds.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md) 集合|获取  **legalHold 对象** 及其属性的列表。|
|[创建 legalHold](../api/ediscovery-case-post-legalholds.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|创建新的 **legalHold** 对象。|
|[获取 legalHold](../api/ediscovery-legalhold-get.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|读取 **legalHold 对象的属性和** 关系。|
|[更新 legalHold](../api/ediscovery-legalhold-update.md)|[microsoft.graph.ediscovery.legalHold](../resources/ediscovery-legalhold.md)|更新 **legalHold 对象** 的属性。|
|[删除 legalHold](../api/ediscovery-legalhold-delete.md)|无|删除 **legalHold** 对象。|
|[列出 siteSources](../api/ediscovery-legalhold-list-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合|获取与合法保留相关联的 [siteSource](../resources/ediscovery-sitesource.md) 对象列表。|
|[创建 siteSource](../api/ediscovery-legalhold-post-sitesources.md)|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md)|创建新的 siteSource 对象。|
|[列出 userSources](../api/ediscovery-legalhold-list-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合|获取与 [合法保留相关联的 userSource](../resources/ediscovery-usersource.md) 对象列表。|
|[创建 userSource](../api/ediscovery-legalhold-post-usersources.md)|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md)|创建新的 **userSource** 对象。|

## <a name="properties"></a>属性

|属性|类型|说明|
|:---|:---|:---|
|contentQuery|String|指定要位于指定位置的内容的 KQL 查询。 若要了解更多信息，请参阅内容搜索和电子数据展示的关键字 [查询和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。  若要保留指定位置中所有的内容，请保留 **contentQuery** 为空。 |
|createdBy|[identitySet](../resources/identityset.md)|创建合法保留的用户。 |
|createdDateTime|DateTimeOffset|创建合法保留的日期和时间。 |
|说明|String| 法定保留说明。 |
|displayName|String| 合法显示名称的保留项。 |
|错误|字符串集合|列出放置保留时发生的任何错误。 |
|id|String|电子数据展示案例的 ID。 只读。 继承自 [实体](../resources/entity.md)。 |
|isEnabled|Boolean|指示是否启用保留并主动保留内容。 |
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改法定保留的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改法定保留的日期和时间。 |
|状态|microsoft.graph.ediscovery.legalHoldStatus|合法保留的状态。 可能的值是：`Pending`、`Error`、`Success`、`UnknownFutureValue`。|

### <a name="legalholdstatus-values"></a>legalHoldStatus 值

|成员|说明|
|:---|-----------|
|Pending| 保留分配过程正在进行中。 |
|错误| 应用保留时出错。 有关详细信息，请参阅 legalHold 对象的 errors 属性。 |
|成功| 成功应用保留并保留指定内容。 |

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|siteSources|[microsoft.graph.ediscovery.siteSource](../resources/ediscovery-sitesource.md) 集合|与合法保留SharePoint网站的数据源实体。 |
|userSources|[microsoft.graph.ediscovery.userSource](../resources/ediscovery-usersource.md) 集合| 合法保留的数据源实体。 这是邮箱和邮箱网站的OneDrive for Business。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.ediscovery.legalHold",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.ediscovery.legalHold",
  "id": "String (identifier)",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "isEnabled": "Boolean",
  "status": "String",
  "contentQuery": "String",
  "errors": [
    "String"
  ],
  "displayName": "String",
  "createdDateTime": "String (timestamp)"
}
```
