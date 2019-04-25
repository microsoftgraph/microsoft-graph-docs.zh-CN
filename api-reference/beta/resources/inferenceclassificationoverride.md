---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件应始终按如下方式分类的用户替代
localization_priority: Normal
ms.openlocfilehash: 1cf1896b43dccfe59ed253c22a8a7341e9ee6e1d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548731"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="9978b-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="9978b-103">inferenceClassificationOverride resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9978b-104">表示有关特定发件人的传入邮件应始终按[重点收件箱](manage-focused-inbox.md)的方式进行分类的用户替代。</span><span class="sxs-lookup"><span data-stu-id="9978b-104">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9978b-105">方法</span><span class="sxs-lookup"><span data-stu-id="9978b-105">Methods</span></span>

| <span data-ttu-id="9978b-106">方法</span><span class="sxs-lookup"><span data-stu-id="9978b-106">Method</span></span>           | <span data-ttu-id="9978b-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="9978b-107">Return Type</span></span>    |<span data-ttu-id="9978b-108">说明</span><span class="sxs-lookup"><span data-stu-id="9978b-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9978b-109">更新</span><span class="sxs-lookup"><span data-stu-id="9978b-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="9978b-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="9978b-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="9978b-111">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="9978b-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="9978b-112">删除</span><span class="sxs-lookup"><span data-stu-id="9978b-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="9978b-113">无</span><span class="sxs-lookup"><span data-stu-id="9978b-113">None</span></span> |<span data-ttu-id="9978b-114">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="9978b-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="9978b-115">属性</span><span class="sxs-lookup"><span data-stu-id="9978b-115">Properties</span></span>
| <span data-ttu-id="9978b-116">属性</span><span class="sxs-lookup"><span data-stu-id="9978b-116">Property</span></span>     | <span data-ttu-id="9978b-117">类型</span><span class="sxs-lookup"><span data-stu-id="9978b-117">Type</span></span>   |<span data-ttu-id="9978b-118">说明</span><span class="sxs-lookup"><span data-stu-id="9978b-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9978b-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="9978b-119">classifyAs</span></span>|<span data-ttu-id="9978b-120">string</span><span class="sxs-lookup"><span data-stu-id="9978b-120">string</span></span>| <span data-ttu-id="9978b-p101">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="9978b-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="9978b-123">id</span><span class="sxs-lookup"><span data-stu-id="9978b-123">id</span></span>|<span data-ttu-id="9978b-124">string</span><span class="sxs-lookup"><span data-stu-id="9978b-124">string</span></span>| <span data-ttu-id="9978b-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="9978b-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="9978b-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="9978b-127">senderEmailAddress</span></span>|[<span data-ttu-id="9978b-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="9978b-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="9978b-129">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="9978b-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9978b-130">关系</span><span class="sxs-lookup"><span data-stu-id="9978b-130">Relationships</span></span>
<span data-ttu-id="9978b-131">无</span><span class="sxs-lookup"><span data-stu-id="9978b-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9978b-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9978b-132">JSON representation</span></span>

<span data-ttu-id="9978b-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9978b-133">Here is a JSON representation of the resource.</span></span>

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
