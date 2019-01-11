---
title: inferenceClassification 资源类型
description: '用户邮件分类，确保仅关注对用户更相关或更重要的邮件。 '
localization_priority: Normal
ms.openlocfilehash: 82d16e24e21231b8ec168eda793257ef780c2219
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877789"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="28cb1-103">inferenceClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="28cb1-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="28cb1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="28cb1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="28cb1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="28cb1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="28cb1-106">用户邮件分类，确保仅关注对用户更相关或更重要的邮件。</span><span class="sxs-lookup"><span data-stu-id="28cb1-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="28cb1-107">有关详细信息，请参阅 [管理重点收件箱](manage-focused-inbox.md)。</span><span class="sxs-lookup"><span data-stu-id="28cb1-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="28cb1-108">方法</span><span class="sxs-lookup"><span data-stu-id="28cb1-108">Methods</span></span>

| <span data-ttu-id="28cb1-109">方法</span><span class="sxs-lookup"><span data-stu-id="28cb1-109">Method</span></span>           | <span data-ttu-id="28cb1-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="28cb1-110">Return Type</span></span>    |<span data-ttu-id="28cb1-111">说明</span><span class="sxs-lookup"><span data-stu-id="28cb1-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="28cb1-112">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="28cb1-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="28cb1-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="28cb1-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="28cb1-p102">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="28cb1-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="28cb1-116">列出替代</span><span class="sxs-lookup"><span data-stu-id="28cb1-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="28cb1-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28cb1-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="28cb1-118">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="28cb1-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="28cb1-119">属性</span><span class="sxs-lookup"><span data-stu-id="28cb1-119">Properties</span></span>
| <span data-ttu-id="28cb1-120">属性</span><span class="sxs-lookup"><span data-stu-id="28cb1-120">Property</span></span>     | <span data-ttu-id="28cb1-121">类型</span><span class="sxs-lookup"><span data-stu-id="28cb1-121">Type</span></span>   |<span data-ttu-id="28cb1-122">说明</span><span class="sxs-lookup"><span data-stu-id="28cb1-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28cb1-123">ID</span><span class="sxs-lookup"><span data-stu-id="28cb1-123">id</span></span>|<span data-ttu-id="28cb1-124">string</span><span class="sxs-lookup"><span data-stu-id="28cb1-124">string</span></span>| <span data-ttu-id="28cb1-125">只读。</span><span class="sxs-lookup"><span data-stu-id="28cb1-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="28cb1-126">Relationships</span><span class="sxs-lookup"><span data-stu-id="28cb1-126">Relationships</span></span>
| <span data-ttu-id="28cb1-127">关系</span><span class="sxs-lookup"><span data-stu-id="28cb1-127">Relationship</span></span> | <span data-ttu-id="28cb1-128">类型</span><span class="sxs-lookup"><span data-stu-id="28cb1-128">Type</span></span>   |<span data-ttu-id="28cb1-129">说明</span><span class="sxs-lookup"><span data-stu-id="28cb1-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="28cb1-130">替代</span><span class="sxs-lookup"><span data-stu-id="28cb1-130">overrides</span></span>|<span data-ttu-id="28cb1-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="28cb1-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="28cb1-p103">用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。</span><span class="sxs-lookup"><span data-stu-id="28cb1-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="28cb1-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="28cb1-135">JSON representation</span></span>

<span data-ttu-id="28cb1-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="28cb1-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
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
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
