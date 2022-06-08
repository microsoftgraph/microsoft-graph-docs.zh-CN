---
title: ediscoveryReviewTag 资源类型
description: 表示电子数据展示标记，用于在审阅期间将文档标记为单独的响应和无响应内容
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: resourcePageType
ms.openlocfilehash: 1e5ba6fecb006a270d256e0f53f63e643874cec4
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945159"
---
# <a name="ediscoveryreviewtag-resource-type"></a>ediscoveryReviewTag 资源类型

命名空间：microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

表示电子数据展示标记，用于在审阅期间将文档标记为单独的响应和无响应内容。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 ediscoveryReviewTags](../api/security-ediscoverycase-list-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|获取 [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 对象及其属性的列表。|
|[创建 ediscoveryReviewTag](../api/security-ediscoverycase-post-tags.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|创建新的 [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 对象。|
|[获取 ediscoveryReviewTag](../api/security-ediscoveryreviewtag-get.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|读取 [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 对象的属性和关系。|
|[更新 ediscoveryReviewTag](../api/security-ediscoveryreviewtag-update.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|更新 [ediscoveryReviewTag 对象的](../resources/security-ediscoveryreviewtag.md) 属性。|
|[删除 ediscoveryReviewTag](../api/security-ediscoverycase-delete-tags.md)|无|删除 [ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 对象。|
|[asHierarchy](../api/security-ediscoveryreviewtag-ashierarchy.md)|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|列出以层次结构形式组织的标记。|


## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|childSelectability|String|指示是否可以将单个或多个子标记与文档关联。 可取值为：`One`、`Many`。  此值控制 UX 是将标记显示为复选框还是单选按钮组。|
|createdBy|[identitySet](../resources/identityset.md)|创建标记的用户。|
|description|字符串|标记的说明。|
|displayName|String|标记的显示名称。|
|id|字符串|标记的唯一标识符。|
|lastModifiedDateTime|DateTimeOffset|上次修改标记的日期和时间。|

### <a name="childselectability-values"></a>childSelectability 值

|成员|说明|
|:----|-----------|
|一个|只能选择一个子级。 这与显示带单选按钮的标记的 UI 相对应。|
|许多|可以选择零个或多个子级。 这对应于显示带有复选框的标记的 UI。|

## <a name="relationships"></a>关系

|关系|类型|说明|
|:---|:---|:---|
|childTags|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md) 集合|返回标记的子级标记。|
|父级|[microsoft.graph.security.ediscoveryReviewTag](../resources/security-ediscoveryreviewtag.md)|返回指定标记的父标记。|
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.security.ediscoveryReviewTag",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.security.ediscoveryReviewTag",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "lastModifiedDateTime": "String (timestamp)",
  "childSelectability": "String"
}
```

