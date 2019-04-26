---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件始终应如何分类的用户的替代。
localization_priority: Normal
ms.openlocfilehash: 8df0f1e5fa34c630c51de7c73234e6092448f867
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32567534"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="e3cf5-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="e3cf5-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="e3cf5-104">表示来自特定发件人的传入邮件始终应如何分类的用户的替代。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-104">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="e3cf5-105">方法</span><span class="sxs-lookup"><span data-stu-id="e3cf5-105">Methods</span></span>

| <span data-ttu-id="e3cf5-106">方法</span><span class="sxs-lookup"><span data-stu-id="e3cf5-106">Method</span></span>           | <span data-ttu-id="e3cf5-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="e3cf5-107">Return Type</span></span>    |<span data-ttu-id="e3cf5-108">说明</span><span class="sxs-lookup"><span data-stu-id="e3cf5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="e3cf5-109">更新</span><span class="sxs-lookup"><span data-stu-id="e3cf5-109">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="e3cf5-110">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="e3cf5-110">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="e3cf5-111">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-111">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="e3cf5-112">删除</span><span class="sxs-lookup"><span data-stu-id="e3cf5-112">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="e3cf5-113">无</span><span class="sxs-lookup"><span data-stu-id="e3cf5-113">None</span></span> |<span data-ttu-id="e3cf5-114">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-114">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="e3cf5-115">属性</span><span class="sxs-lookup"><span data-stu-id="e3cf5-115">Properties</span></span>
| <span data-ttu-id="e3cf5-116">属性</span><span class="sxs-lookup"><span data-stu-id="e3cf5-116">Property</span></span>     | <span data-ttu-id="e3cf5-117">类型</span><span class="sxs-lookup"><span data-stu-id="e3cf5-117">Type</span></span>   |<span data-ttu-id="e3cf5-118">说明</span><span class="sxs-lookup"><span data-stu-id="e3cf5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e3cf5-119">classifyAs</span><span class="sxs-lookup"><span data-stu-id="e3cf5-119">classifyAs</span></span>|<span data-ttu-id="e3cf5-120">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="e3cf5-120">inferenceClassificationType</span></span>| <span data-ttu-id="e3cf5-121">指定来自特定发件人的传入邮件始终应如何分类。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-121">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="e3cf5-122">可能的值为: `focused`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-122">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="e3cf5-123">id</span><span class="sxs-lookup"><span data-stu-id="e3cf5-123">id</span></span>|<span data-ttu-id="e3cf5-124">string</span><span class="sxs-lookup"><span data-stu-id="e3cf5-124">string</span></span>| <span data-ttu-id="e3cf5-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="e3cf5-127">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="e3cf5-127">senderEmailAddress</span></span>|[<span data-ttu-id="e3cf5-128">emailAddress</span><span class="sxs-lookup"><span data-stu-id="e3cf5-128">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="e3cf5-129">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-129">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e3cf5-130">关系</span><span class="sxs-lookup"><span data-stu-id="e3cf5-130">Relationships</span></span>
<span data-ttu-id="e3cf5-131">无</span><span class="sxs-lookup"><span data-stu-id="e3cf5-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="e3cf5-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e3cf5-132">JSON representation</span></span>

<span data-ttu-id="e3cf5-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e3cf5-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
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
