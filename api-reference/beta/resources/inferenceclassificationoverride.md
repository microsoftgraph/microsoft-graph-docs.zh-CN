---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件始终应如何分类的用户的替代。
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511798"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="bed59-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="bed59-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bed59-104">表示用户替代收到来自特定发件人的邮件应始终进行分类如[中心收件箱](manage-focused-inbox.md)中所示。</span><span class="sxs-lookup"><span data-stu-id="bed59-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="bed59-105">方法</span><span class="sxs-lookup"><span data-stu-id="bed59-105">Methods</span></span>

| <span data-ttu-id="bed59-106">方法</span><span class="sxs-lookup"><span data-stu-id="bed59-106">Method</span></span>           | <span data-ttu-id="bed59-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="bed59-107">Return Type</span></span>    |<span data-ttu-id="bed59-108">说明</span><span class="sxs-lookup"><span data-stu-id="bed59-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="bed59-109">Update</span><span class="sxs-lookup"><span data-stu-id="bed59-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="bed59-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="bed59-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="bed59-111">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="bed59-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="bed59-112">删除</span><span class="sxs-lookup"><span data-stu-id="bed59-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="bed59-113">无</span><span class="sxs-lookup"><span data-stu-id="bed59-113">None</span></span> |<span data-ttu-id="bed59-114">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="bed59-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="bed59-115">属性</span><span class="sxs-lookup"><span data-stu-id="bed59-115">Properties</span></span>
| <span data-ttu-id="bed59-116">属性</span><span class="sxs-lookup"><span data-stu-id="bed59-116">Property</span></span>     | <span data-ttu-id="bed59-117">类型</span><span class="sxs-lookup"><span data-stu-id="bed59-117">Type</span></span>   |<span data-ttu-id="bed59-118">说明</span><span class="sxs-lookup"><span data-stu-id="bed59-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="bed59-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="bed59-119">classifyAs</span></span>|<span data-ttu-id="bed59-120">string</span><span class="sxs-lookup"><span data-stu-id="bed59-120">string</span></span>| <span data-ttu-id="bed59-p101">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="bed59-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="bed59-123">id</span><span class="sxs-lookup"><span data-stu-id="bed59-123">id</span></span>|<span data-ttu-id="bed59-124">string</span><span class="sxs-lookup"><span data-stu-id="bed59-124">string</span></span>| <span data-ttu-id="bed59-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="bed59-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="bed59-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="bed59-127">senderEmailAddress</span></span>|[<span data-ttu-id="bed59-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="bed59-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="bed59-129">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="bed59-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="bed59-130">关系</span><span class="sxs-lookup"><span data-stu-id="bed59-130">Relationships</span></span>
<span data-ttu-id="bed59-131">无</span><span class="sxs-lookup"><span data-stu-id="bed59-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="bed59-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bed59-132">JSON representation</span></span>

<span data-ttu-id="bed59-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bed59-133">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassificationOverride resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassificationoverride.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
