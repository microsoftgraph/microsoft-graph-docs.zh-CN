---
title: inferenceClassification 资源类型
description: '用户邮件分类，确保仅关注对用户更相关或更重要的邮件。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf1ea3b61df2166f58f161b804f55e87e474be97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006267"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="e21f7-103">inferenceClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="e21f7-103">inferenceClassification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e21f7-104">用户邮件分类，确保仅关注对用户更相关或更重要的邮件。</span><span class="sxs-lookup"><span data-stu-id="e21f7-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="e21f7-105">有关详细信息，请参阅 [管理重点收件箱](manage-focused-inbox.md)。</span><span class="sxs-lookup"><span data-stu-id="e21f7-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="e21f7-106">方法</span><span class="sxs-lookup"><span data-stu-id="e21f7-106">Methods</span></span>

| <span data-ttu-id="e21f7-107">方法</span><span class="sxs-lookup"><span data-stu-id="e21f7-107">Method</span></span>           | <span data-ttu-id="e21f7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="e21f7-108">Return Type</span></span>    |<span data-ttu-id="e21f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="e21f7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e21f7-110">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e21f7-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="e21f7-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e21f7-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="e21f7-p101">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="e21f7-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="e21f7-114">列出替代</span><span class="sxs-lookup"><span data-stu-id="e21f7-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="e21f7-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e21f7-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="e21f7-116">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="e21f7-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="e21f7-117">属性</span><span class="sxs-lookup"><span data-stu-id="e21f7-117">Properties</span></span>
| <span data-ttu-id="e21f7-118">属性</span><span class="sxs-lookup"><span data-stu-id="e21f7-118">Property</span></span>     | <span data-ttu-id="e21f7-119">类型</span><span class="sxs-lookup"><span data-stu-id="e21f7-119">Type</span></span>   |<span data-ttu-id="e21f7-120">说明</span><span class="sxs-lookup"><span data-stu-id="e21f7-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e21f7-121">id</span><span class="sxs-lookup"><span data-stu-id="e21f7-121">id</span></span>|<span data-ttu-id="e21f7-122">string</span><span class="sxs-lookup"><span data-stu-id="e21f7-122">string</span></span>| <span data-ttu-id="e21f7-123">只读。</span><span class="sxs-lookup"><span data-stu-id="e21f7-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e21f7-124">关系</span><span class="sxs-lookup"><span data-stu-id="e21f7-124">Relationships</span></span>
| <span data-ttu-id="e21f7-125">关系</span><span class="sxs-lookup"><span data-stu-id="e21f7-125">Relationship</span></span> | <span data-ttu-id="e21f7-126">类型</span><span class="sxs-lookup"><span data-stu-id="e21f7-126">Type</span></span>   |<span data-ttu-id="e21f7-127">说明</span><span class="sxs-lookup"><span data-stu-id="e21f7-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e21f7-128">替代</span><span class="sxs-lookup"><span data-stu-id="e21f7-128">overrides</span></span>|<span data-ttu-id="e21f7-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="e21f7-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="e21f7-p102">用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。</span><span class="sxs-lookup"><span data-stu-id="e21f7-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e21f7-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e21f7-133">JSON representation</span></span>

<span data-ttu-id="e21f7-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e21f7-134">Here is a JSON representation of the resource.</span></span>

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
