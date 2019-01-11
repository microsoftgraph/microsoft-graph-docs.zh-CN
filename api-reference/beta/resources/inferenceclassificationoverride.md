---
title: inferenceClassificationOverride 资源类型
description: 代表收到来自特定发件人的邮件的用户的重写应始终分类为
localization_priority: Normal
ms.openlocfilehash: 9124f773a26c9edf1238276c3d0017dcc46e7ad8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876265"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="fcdca-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="fcdca-103">inferenceClassificationOverride resource type</span></span>

> <span data-ttu-id="fcdca-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fcdca-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcdca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fcdca-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fcdca-106">表示用户替代收到来自特定发件人的邮件应始终进行分类如[中心收件箱](manage-focused-inbox.md)中所示。</span><span class="sxs-lookup"><span data-stu-id="fcdca-106">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="fcdca-107">方法</span><span class="sxs-lookup"><span data-stu-id="fcdca-107">Methods</span></span>

| <span data-ttu-id="fcdca-108">方法</span><span class="sxs-lookup"><span data-stu-id="fcdca-108">Method</span></span>           | <span data-ttu-id="fcdca-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="fcdca-109">Return Type</span></span>    |<span data-ttu-id="fcdca-110">说明</span><span class="sxs-lookup"><span data-stu-id="fcdca-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fcdca-111">Update</span><span class="sxs-lookup"><span data-stu-id="fcdca-111">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="fcdca-112">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="fcdca-112">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="fcdca-113">更改指定重写**ClassifyAs**字段。</span><span class="sxs-lookup"><span data-stu-id="fcdca-113">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="fcdca-114">删除</span><span class="sxs-lookup"><span data-stu-id="fcdca-114">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="fcdca-115">无</span><span class="sxs-lookup"><span data-stu-id="fcdca-115">None</span></span> |<span data-ttu-id="fcdca-116">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="fcdca-116">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="fcdca-117">属性</span><span class="sxs-lookup"><span data-stu-id="fcdca-117">Properties</span></span>
| <span data-ttu-id="fcdca-118">属性</span><span class="sxs-lookup"><span data-stu-id="fcdca-118">Property</span></span>     | <span data-ttu-id="fcdca-119">类型</span><span class="sxs-lookup"><span data-stu-id="fcdca-119">Type</span></span>   |<span data-ttu-id="fcdca-120">说明</span><span class="sxs-lookup"><span data-stu-id="fcdca-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fcdca-121">classifyAs</span><span class="sxs-lookup"><span data-stu-id="fcdca-121">classifyAs</span></span>|<span data-ttu-id="fcdca-122">string</span><span class="sxs-lookup"><span data-stu-id="fcdca-122">string</span></span>| <span data-ttu-id="fcdca-p102">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="fcdca-p102">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="fcdca-125">id</span><span class="sxs-lookup"><span data-stu-id="fcdca-125">id</span></span>|<span data-ttu-id="fcdca-126">string</span><span class="sxs-lookup"><span data-stu-id="fcdca-126">string</span></span>| <span data-ttu-id="fcdca-p103">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="fcdca-p103">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="fcdca-129">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="fcdca-129">senderEmailAddress</span></span>|[<span data-ttu-id="fcdca-130">emailAddress</span><span class="sxs-lookup"><span data-stu-id="fcdca-130">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="fcdca-131">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="fcdca-131">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fcdca-132">Relationships</span><span class="sxs-lookup"><span data-stu-id="fcdca-132">Relationships</span></span>
<span data-ttu-id="fcdca-133">无</span><span class="sxs-lookup"><span data-stu-id="fcdca-133">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fcdca-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fcdca-134">JSON representation</span></span>

<span data-ttu-id="fcdca-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcdca-135">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassificationOverride"
}-->

```json
{
  "classifyAs": "string",
  "id": "string (identifier)",
  "senderEmailAddress": {"@odata.type": "microsoft.graph.emailAddress"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
