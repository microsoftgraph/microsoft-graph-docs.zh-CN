---
title: inferenceClassification 资源类型
description: '用户邮件分类，确保仅关注对用户更相关或更重要的邮件。 '
ms.localizationpriority: medium
doc_type: resourcePageType
ms.prod: mail
author: abheek-das
ms.openlocfilehash: 53754b1a803a7c6e550bd8afc682d0d6403b77b1
ms.sourcegitcommit: 95df356bd43b8e5f60fb4c2b62bfa0d5f36a61c2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2022
ms.locfileid: "65899398"
---
# <a name="inferenceclassification-resource-type"></a>inferenceClassification 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

用户邮件分类，确保仅关注对用户更相关或更重要的邮件。

有关详细信息，请参阅 [管理重点收件箱](manage-focused-inbox.md)。


## <a name="methods"></a>方法

| 方法           | 返回类型    |说明|
|:---------------|:--------|:----------|
|[创建 inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md)| 创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。|
|[列出替代](../api/inferenceclassification-list-overrides.md) |[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合| 获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。|

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|id|string| 只读。|

## <a name="relationships"></a>关系
| 关系 | 类型   |说明|
|:---------------|:--------|:----------|
|替代|[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合| 用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。|

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


