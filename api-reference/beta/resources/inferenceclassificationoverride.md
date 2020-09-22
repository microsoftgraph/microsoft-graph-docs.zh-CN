---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件应始终按如下方式分类的用户替代
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: svpsiva
ms.openlocfilehash: b289d369c151e2f735fb992c5bd9a3347da67d17
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48016533"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="a4bf0-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="a4bf0-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="a4bf0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a4bf0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a4bf0-105">表示有关特定发件人的传入邮件应始终按 [重点收件箱](manage-focused-inbox.md)的方式进行分类的用户替代。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-105">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="a4bf0-106">方法</span><span class="sxs-lookup"><span data-stu-id="a4bf0-106">Methods</span></span>

| <span data-ttu-id="a4bf0-107">方法</span><span class="sxs-lookup"><span data-stu-id="a4bf0-107">Method</span></span>           | <span data-ttu-id="a4bf0-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a4bf0-108">Return Type</span></span>    |<span data-ttu-id="a4bf0-109">说明</span><span class="sxs-lookup"><span data-stu-id="a4bf0-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a4bf0-110">更新</span><span class="sxs-lookup"><span data-stu-id="a4bf0-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="a4bf0-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="a4bf0-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="a4bf0-112">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="a4bf0-113">删除</span><span class="sxs-lookup"><span data-stu-id="a4bf0-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="a4bf0-114">无</span><span class="sxs-lookup"><span data-stu-id="a4bf0-114">None</span></span> |<span data-ttu-id="a4bf0-115">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="a4bf0-116">属性</span><span class="sxs-lookup"><span data-stu-id="a4bf0-116">Properties</span></span>
| <span data-ttu-id="a4bf0-117">属性</span><span class="sxs-lookup"><span data-stu-id="a4bf0-117">Property</span></span>     | <span data-ttu-id="a4bf0-118">类型</span><span class="sxs-lookup"><span data-stu-id="a4bf0-118">Type</span></span>   |<span data-ttu-id="a4bf0-119">说明</span><span class="sxs-lookup"><span data-stu-id="a4bf0-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a4bf0-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="a4bf0-120">classifyAs</span></span>|<span data-ttu-id="a4bf0-121">string</span><span class="sxs-lookup"><span data-stu-id="a4bf0-121">string</span></span>| <span data-ttu-id="a4bf0-p101">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="a4bf0-124">id</span><span class="sxs-lookup"><span data-stu-id="a4bf0-124">id</span></span>|<span data-ttu-id="a4bf0-125">string</span><span class="sxs-lookup"><span data-stu-id="a4bf0-125">string</span></span>| <span data-ttu-id="a4bf0-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="a4bf0-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="a4bf0-128">senderEmailAddress</span></span>|[<span data-ttu-id="a4bf0-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="a4bf0-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="a4bf0-130">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a4bf0-131">关系</span><span class="sxs-lookup"><span data-stu-id="a4bf0-131">Relationships</span></span>
<span data-ttu-id="a4bf0-132">无</span><span class="sxs-lookup"><span data-stu-id="a4bf0-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a4bf0-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a4bf0-133">JSON representation</span></span>

<span data-ttu-id="a4bf0-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a4bf0-134">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->


