---
title: ediscoveryHoldPolicy 资源类型
description: '*ediscoveryHoldPolicy 资源类型'
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 8f40b4fe05858cfd37f401e640937867d617edcc
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945170"
---
# <a name="ediscoveryholdpolicy-resource-type"></a>ediscoveryHoldPolicy 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示法律保留策略。 法律保留与电子数据展示案相关。 法律保留不应与保留内容混淆，保留期用于控制 Microsoft 365 内容的保留策略。 电子数据展示法律保留用于无限期保存内容以进行诉讼、内部调查和其他需要保护内容免受删除的法律行为。 有关详细信息，请参阅[高级电子数据展示中的“管理保留](/microsoft-365/compliance/managing-holds)”

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryHoldPolicies](../api/security-ediscoverycase-list-legalholds.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 集合|获取 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象及其属性的列表。|
|[创建 ediscoveryHoldPolicy](../api/security-ediscoverycase-post-legalholds.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|创建新的 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象。|
|[获取 ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-get.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|读取 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象的属性和关系。|
|[更新 ediscoveryHoldPolicy](../api/security-ediscoveryholdpolicy-update.md)|[microsoft.graph.security.ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md)|更新 [ediscoveryHoldPolicy 对象的](../resources/security-ediscoveryholdpolicy.md) 属性。|
|[删除 ediscoveryHoldPolicy](../api/security-ediscoverycase-delete-legalholds.md)|无|删除 [ediscoveryHoldPolicy](../resources/security-ediscoveryholdpolicy.md) 对象。|
|[列出 siteSources](../api/security-ediscoverycustodian-list-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md) 集合|从 siteSources 导航属性获取 siteSource 资源。|
|[创建 siteSource](../api/security-ediscoveryholdpolicy-post-sitesources.md)|[microsoft.graph.security.siteSource](../resources/security-sitesource.md)|创建新的 siteSource 对象。|
|[列出 userSources](../api/security-ediscoverycustodian-list-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md) 集合|从 userSources 导航属性获取 userSource 资源。|
|[创建 userSource](../api/security-ediscoveryholdpolicy-post-usersources.md)|[microsoft.graph.security.userSource](../resources/security-usersource.md)|创建新的 userSource 对象。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|contentQuery|字符串|指定要保存在指定位置的内容的 KQL 查询。 若要了解详细信息，请参阅 [内容搜索和电子数据展示的关键字查询和搜索条件](/microsoft-365/compliance/keyword-queries-and-search-conditions)。  若要保存指定位置中的所有内容，请将 **contentQuery** 留空。 |
|createdBy|[identitySet](../resources/identityset.md)|创建法定保留的用户。 |
|createdDateTime|DateTimeOffset|法定保留的创建日期和时间。 |
|description|String| 法定保留说明。 |
|displayName|String| 法定保留的显示名称。 |
|错误|String collection|列出放置保留时发生的任何错误。 |
|id|String|电子数据展示案例的 ID。 只读。 继承自 [entity](../resources/entity.md)。 |
|isEnabled|Boolean|指示是否启用了保留并主动保存内容。 |
|lastModifiedBy|[identitySet](../resources/identityset.md)|上次修改法定保留的用户。|
|lastModifiedDateTime|DateTimeOffset|上次修改法定保留的日期和时间。 |
|status|String|法定保留的状态。 可取值为：`Pending`、`Error`、`Success`。|

### <a name="legalholdstatus-values"></a>legalHoldStatus 值

|成员|说明|
|:---|-----------|
|Pending| 保留分发过程正在进行中。 |
|错误| 应用保留时出错。 |
|成功| 已成功应用保留并保存指定的内容。 |

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|siteSources|[microsoft.graph.security.siteSource](../resources/security-sitesource.md) 集合|**TODO：添加说明**|
|userSources|[microsoft.graph.security.userSource](../resources/security-usersource.md) 集合|**TODO：添加说明**|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryHoldPolicy",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryHoldPolicy",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "createdDateTime": "String (timestamp)",
  "lastModifiedBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "status": "String",
  "isEnabled": "Boolean",
  "contentQuery": "String",
  "errors": [
    "String"
  ]
}
```

