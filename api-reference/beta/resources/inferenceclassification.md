---
title: inferenceClassification 资源类型
description: '用户邮件分类，确保仅关注对用户更相关或更重要的邮件。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: e2055e49d627edc4492df622f916518ca0ab71df
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46809437"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="2f0fa-103">inferenceClassification 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f0fa-103">inferenceClassification resource type</span></span>

<span data-ttu-id="2f0fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f0fa-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f0fa-105">用户邮件分类，确保仅关注对用户更相关或更重要的邮件。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-105">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span>

<span data-ttu-id="2f0fa-106">有关详细信息，请参阅 [管理重点收件箱](manage-focused-inbox.md)。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-106">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="2f0fa-107">方法</span><span class="sxs-lookup"><span data-stu-id="2f0fa-107">Methods</span></span>

| <span data-ttu-id="2f0fa-108">方法</span><span class="sxs-lookup"><span data-stu-id="2f0fa-108">Method</span></span>           | <span data-ttu-id="2f0fa-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2f0fa-109">Return Type</span></span>    |<span data-ttu-id="2f0fa-110">说明</span><span class="sxs-lookup"><span data-stu-id="2f0fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2f0fa-111">创建 inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2f0fa-111">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="2f0fa-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="2f0fa-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="2f0fa-p101">创建由 SMTP 地址识别的发件人的替代。将以后来自该 SMTP 地址的邮件一致归为替代中指定的类别。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="2f0fa-115">列出替代</span><span class="sxs-lookup"><span data-stu-id="2f0fa-115">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="2f0fa-116">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f0fa-116">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="2f0fa-117">获取用户设置为始终以特定方式对来自特定发件人的邮件进行分类的替代。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-117">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f0fa-118">属性</span><span class="sxs-lookup"><span data-stu-id="2f0fa-118">Properties</span></span>
| <span data-ttu-id="2f0fa-119">属性</span><span class="sxs-lookup"><span data-stu-id="2f0fa-119">Property</span></span>     | <span data-ttu-id="2f0fa-120">类型</span><span class="sxs-lookup"><span data-stu-id="2f0fa-120">Type</span></span>   |<span data-ttu-id="2f0fa-121">说明</span><span class="sxs-lookup"><span data-stu-id="2f0fa-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f0fa-122">id</span><span class="sxs-lookup"><span data-stu-id="2f0fa-122">id</span></span>|<span data-ttu-id="2f0fa-123">string</span><span class="sxs-lookup"><span data-stu-id="2f0fa-123">string</span></span>| <span data-ttu-id="2f0fa-124">只读。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-124">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f0fa-125">关系</span><span class="sxs-lookup"><span data-stu-id="2f0fa-125">Relationships</span></span>
| <span data-ttu-id="2f0fa-126">关系</span><span class="sxs-lookup"><span data-stu-id="2f0fa-126">Relationship</span></span> | <span data-ttu-id="2f0fa-127">类型</span><span class="sxs-lookup"><span data-stu-id="2f0fa-127">Type</span></span>   |<span data-ttu-id="2f0fa-128">说明</span><span class="sxs-lookup"><span data-stu-id="2f0fa-128">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f0fa-129">替代</span><span class="sxs-lookup"><span data-stu-id="2f0fa-129">overrides</span></span>|<span data-ttu-id="2f0fa-130">[inferenceClassificationOverride](inferenceclassificationoverride.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2f0fa-130">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="2f0fa-p102">用户始终按某种方式（`focused` 或 `other`）对来自特定发件人的邮件分类的一组替代。只读。可为 null。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f0fa-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f0fa-134">JSON representation</span></span>

<span data-ttu-id="2f0fa-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f0fa-135">Here is a JSON representation of the resource.</span></span>

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
