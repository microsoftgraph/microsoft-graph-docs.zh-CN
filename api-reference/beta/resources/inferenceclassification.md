---
title: inferenceClassification 资源类型
description: '用户邮件分类，确保仅关注对用户更相关或更重要的邮件。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: abheek-das
ms.openlocfilehash: b69f892a9d8223e467a10ce1c055cc470a2c171e
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130253"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="851b0-103">inferenceClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="851b0-103">inferenceClassification resource type</span></span>

<span data-ttu-id="851b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="851b0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="851b0-105">用户邮件分类，确保仅关注对用户更相关或更重要的邮件。</span><span class="sxs-lookup"><span data-stu-id="851b0-105">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span>

<span data-ttu-id="851b0-106">有关详细信息，请参阅 [管理重点收件箱](manage-focused-inbox.md)。</span><span class="sxs-lookup"><span data-stu-id="851b0-106">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="851b0-107">方法</span><span class="sxs-lookup"><span data-stu-id="851b0-107">Methods</span></span>

| <span data-ttu-id="851b0-108">方法</span><span class="sxs-lookup"><span data-stu-id="851b0-108">Method</span></span>           | <span data-ttu-id="851b0-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="851b0-109">Return Type</span></span>    |<span data-ttu-id="851b0-110">说明</span><span class="sxs-lookup"><span data-stu-id="851b0-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="851b0-111">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="851b0-111">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="851b0-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="851b0-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="851b0-p101">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="851b0-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="851b0-115">列出替代</span><span class="sxs-lookup"><span data-stu-id="851b0-115">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="851b0-116">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="851b0-116">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="851b0-117">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="851b0-117">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="851b0-118">属性</span><span class="sxs-lookup"><span data-stu-id="851b0-118">Properties</span></span>
| <span data-ttu-id="851b0-119">属性</span><span class="sxs-lookup"><span data-stu-id="851b0-119">Property</span></span>     | <span data-ttu-id="851b0-120">类型</span><span class="sxs-lookup"><span data-stu-id="851b0-120">Type</span></span>   |<span data-ttu-id="851b0-121">说明</span><span class="sxs-lookup"><span data-stu-id="851b0-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="851b0-122">id</span><span class="sxs-lookup"><span data-stu-id="851b0-122">id</span></span>|<span data-ttu-id="851b0-123">string</span><span class="sxs-lookup"><span data-stu-id="851b0-123">string</span></span>| <span data-ttu-id="851b0-124">只读。</span><span class="sxs-lookup"><span data-stu-id="851b0-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="851b0-125">关系</span><span class="sxs-lookup"><span data-stu-id="851b0-125">Relationships</span></span>
| <span data-ttu-id="851b0-126">关系</span><span class="sxs-lookup"><span data-stu-id="851b0-126">Relationship</span></span> | <span data-ttu-id="851b0-127">类型</span><span class="sxs-lookup"><span data-stu-id="851b0-127">Type</span></span>   |<span data-ttu-id="851b0-128">说明</span><span class="sxs-lookup"><span data-stu-id="851b0-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="851b0-129">替代</span><span class="sxs-lookup"><span data-stu-id="851b0-129">overrides</span></span>|<span data-ttu-id="851b0-130">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="851b0-130">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="851b0-p102">用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。</span><span class="sxs-lookup"><span data-stu-id="851b0-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="851b0-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="851b0-134">JSON representation</span></span>

<span data-ttu-id="851b0-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="851b0-135">Here is a JSON representation of the resource.</span></span>

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


