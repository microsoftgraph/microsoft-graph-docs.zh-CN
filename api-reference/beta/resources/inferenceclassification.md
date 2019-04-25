---
title: inferenceClassification 资源类型
description: '用户邮件分类，确保仅关注对用户更相关或更重要的邮件。 '
localization_priority: Normal
ms.openlocfilehash: f06177db9907deb3be38c2cdab82669764503cd6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549040"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="db59e-103">inferenceClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="db59e-103">inferenceClassification resource type</span></span>

<span data-ttu-id="db59e-104">用户邮件分类，确保仅关注对用户更相关或更重要的邮件。</span><span class="sxs-lookup"><span data-stu-id="db59e-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="db59e-105">有关详细信息，请参阅 [管理重点收件箱](manage-focused-inbox.md)。</span><span class="sxs-lookup"><span data-stu-id="db59e-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="db59e-106">方法</span><span class="sxs-lookup"><span data-stu-id="db59e-106">Methods</span></span>

| <span data-ttu-id="db59e-107">方法</span><span class="sxs-lookup"><span data-stu-id="db59e-107">Method</span></span>           | <span data-ttu-id="db59e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="db59e-108">Return Type</span></span>    |<span data-ttu-id="db59e-109">说明</span><span class="sxs-lookup"><span data-stu-id="db59e-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="db59e-110">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="db59e-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="db59e-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="db59e-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="db59e-p101">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="db59e-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="db59e-114">列出替代</span><span class="sxs-lookup"><span data-stu-id="db59e-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="db59e-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db59e-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="db59e-116">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="db59e-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="db59e-117">属性</span><span class="sxs-lookup"><span data-stu-id="db59e-117">Properties</span></span>
| <span data-ttu-id="db59e-118">属性</span><span class="sxs-lookup"><span data-stu-id="db59e-118">Property</span></span>     | <span data-ttu-id="db59e-119">类型</span><span class="sxs-lookup"><span data-stu-id="db59e-119">Type</span></span>   |<span data-ttu-id="db59e-120">说明</span><span class="sxs-lookup"><span data-stu-id="db59e-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db59e-121">id</span><span class="sxs-lookup"><span data-stu-id="db59e-121">id</span></span>|<span data-ttu-id="db59e-122">string</span><span class="sxs-lookup"><span data-stu-id="db59e-122">string</span></span>| <span data-ttu-id="db59e-123">只读。</span><span class="sxs-lookup"><span data-stu-id="db59e-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="db59e-124">关系</span><span class="sxs-lookup"><span data-stu-id="db59e-124">Relationships</span></span>
| <span data-ttu-id="db59e-125">关系</span><span class="sxs-lookup"><span data-stu-id="db59e-125">Relationship</span></span> | <span data-ttu-id="db59e-126">类型</span><span class="sxs-lookup"><span data-stu-id="db59e-126">Type</span></span>   |<span data-ttu-id="db59e-127">说明</span><span class="sxs-lookup"><span data-stu-id="db59e-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db59e-128">替代</span><span class="sxs-lookup"><span data-stu-id="db59e-128">overrides</span></span>|<span data-ttu-id="db59e-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="db59e-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="db59e-p102">用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。</span><span class="sxs-lookup"><span data-stu-id="db59e-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="db59e-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="db59e-133">JSON representation</span></span>

<span data-ttu-id="db59e-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db59e-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
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
