---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件应始终按如下方式分类的用户替代
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 944d9784e43ff5c1277c526a6b9fe3115487ac8d
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42496206"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="5ee9c-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="5ee9c-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="5ee9c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="5ee9c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5ee9c-105">表示有关特定发件人的传入邮件应始终按[重点收件箱](manage-focused-inbox.md)的方式进行分类的用户替代。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-105">Represents a user's override for how incoming messages from a specific sender should always be classified as in a [Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="5ee9c-106">方法</span><span class="sxs-lookup"><span data-stu-id="5ee9c-106">Methods</span></span>

| <span data-ttu-id="5ee9c-107">方法</span><span class="sxs-lookup"><span data-stu-id="5ee9c-107">Method</span></span>           | <span data-ttu-id="5ee9c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="5ee9c-108">Return Type</span></span>    |<span data-ttu-id="5ee9c-109">说明</span><span class="sxs-lookup"><span data-stu-id="5ee9c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5ee9c-110">更新</span><span class="sxs-lookup"><span data-stu-id="5ee9c-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="5ee9c-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="5ee9c-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="5ee9c-112">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="5ee9c-113">删除</span><span class="sxs-lookup"><span data-stu-id="5ee9c-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="5ee9c-114">无</span><span class="sxs-lookup"><span data-stu-id="5ee9c-114">None</span></span> |<span data-ttu-id="5ee9c-115">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="5ee9c-116">属性</span><span class="sxs-lookup"><span data-stu-id="5ee9c-116">Properties</span></span>
| <span data-ttu-id="5ee9c-117">属性</span><span class="sxs-lookup"><span data-stu-id="5ee9c-117">Property</span></span>     | <span data-ttu-id="5ee9c-118">类型</span><span class="sxs-lookup"><span data-stu-id="5ee9c-118">Type</span></span>   |<span data-ttu-id="5ee9c-119">说明</span><span class="sxs-lookup"><span data-stu-id="5ee9c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5ee9c-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="5ee9c-120">classifyAs</span></span>|<span data-ttu-id="5ee9c-121">string</span><span class="sxs-lookup"><span data-stu-id="5ee9c-121">string</span></span>| <span data-ttu-id="5ee9c-p101">指定来自特定发件人的传入邮件始终应如何分类。可能的值是：`focused`、`other`。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-p101">Specifies how incoming messages from a specific sender should always be classified as. Possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="5ee9c-124">id</span><span class="sxs-lookup"><span data-stu-id="5ee9c-124">id</span></span>|<span data-ttu-id="5ee9c-125">string</span><span class="sxs-lookup"><span data-stu-id="5ee9c-125">string</span></span>| <span data-ttu-id="5ee9c-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="5ee9c-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="5ee9c-128">senderEmailAddress</span></span>|[<span data-ttu-id="5ee9c-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="5ee9c-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="5ee9c-130">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5ee9c-131">关系</span><span class="sxs-lookup"><span data-stu-id="5ee9c-131">Relationships</span></span>
<span data-ttu-id="5ee9c-132">无</span><span class="sxs-lookup"><span data-stu-id="5ee9c-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="5ee9c-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5ee9c-133">JSON representation</span></span>

<span data-ttu-id="5ee9c-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ee9c-134">Here is a JSON representation of the resource.</span></span>

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
