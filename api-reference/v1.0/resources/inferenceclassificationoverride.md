---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件始终应如何分类的用户的替代。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 7a80283bd3f32c28b71d02acd2ae93e76cac1299
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42531304"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="cb028-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="cb028-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="cb028-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb028-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb028-105">表示来自特定发件人的传入邮件始终应如何分类的用户的替代。</span><span class="sxs-lookup"><span data-stu-id="cb028-105">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="cb028-106">Methods</span><span class="sxs-lookup"><span data-stu-id="cb028-106">Methods</span></span>

| <span data-ttu-id="cb028-107">方法</span><span class="sxs-lookup"><span data-stu-id="cb028-107">Method</span></span>           | <span data-ttu-id="cb028-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="cb028-108">Return Type</span></span>    |<span data-ttu-id="cb028-109">说明</span><span class="sxs-lookup"><span data-stu-id="cb028-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb028-110">更新</span><span class="sxs-lookup"><span data-stu-id="cb028-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="cb028-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="cb028-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="cb028-112">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="cb028-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="cb028-113">删除</span><span class="sxs-lookup"><span data-stu-id="cb028-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="cb028-114">无</span><span class="sxs-lookup"><span data-stu-id="cb028-114">None</span></span> |<span data-ttu-id="cb028-115">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="cb028-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb028-116">属性</span><span class="sxs-lookup"><span data-stu-id="cb028-116">Properties</span></span>
| <span data-ttu-id="cb028-117">属性</span><span class="sxs-lookup"><span data-stu-id="cb028-117">Property</span></span>     | <span data-ttu-id="cb028-118">类型</span><span class="sxs-lookup"><span data-stu-id="cb028-118">Type</span></span>   |<span data-ttu-id="cb028-119">说明</span><span class="sxs-lookup"><span data-stu-id="cb028-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb028-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="cb028-120">classifyAs</span></span>|<span data-ttu-id="cb028-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="cb028-121">inferenceClassificationType</span></span>| <span data-ttu-id="cb028-122">指定来自特定发件人的传入邮件始终应如何分类。</span><span class="sxs-lookup"><span data-stu-id="cb028-122">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="cb028-123">可能的值为： `focused`、 `other`。</span><span class="sxs-lookup"><span data-stu-id="cb028-123">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="cb028-124">id</span><span class="sxs-lookup"><span data-stu-id="cb028-124">id</span></span>|<span data-ttu-id="cb028-125">string</span><span class="sxs-lookup"><span data-stu-id="cb028-125">string</span></span>| <span data-ttu-id="cb028-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="cb028-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="cb028-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="cb028-128">senderEmailAddress</span></span>|[<span data-ttu-id="cb028-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="cb028-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="cb028-130">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="cb028-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cb028-131">关系</span><span class="sxs-lookup"><span data-stu-id="cb028-131">Relationships</span></span>
<span data-ttu-id="cb028-132">无</span><span class="sxs-lookup"><span data-stu-id="cb028-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cb028-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cb028-133">JSON representation</span></span>

<span data-ttu-id="cb028-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb028-134">Here is a JSON representation of the resource.</span></span>

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
