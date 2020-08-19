---
title: inferenceClassificationOverride 资源类型
description: 表示来自特定发件人的传入邮件始终应如何分类的用户的替代。
localization_priority: Normal
author: svpsiva
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: c65bbecda618115e40a3c3cc36f2b952597b9c85
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46808905"
---
# <a name="inferenceclassificationoverride-resource-type"></a><span data-ttu-id="d6fb7-103">inferenceClassificationOverride 资源类型</span><span class="sxs-lookup"><span data-stu-id="d6fb7-103">inferenceClassificationOverride resource type</span></span>

<span data-ttu-id="d6fb7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d6fb7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d6fb7-105">表示来自特定发件人的传入邮件始终应如何分类的用户的替代。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-105">Represents a user's override for how incoming messages from a specific sender should always be classified as.</span></span>


## <a name="methods"></a><span data-ttu-id="d6fb7-106">方法</span><span class="sxs-lookup"><span data-stu-id="d6fb7-106">Methods</span></span>

| <span data-ttu-id="d6fb7-107">方法</span><span class="sxs-lookup"><span data-stu-id="d6fb7-107">Method</span></span>           | <span data-ttu-id="d6fb7-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="d6fb7-108">Return Type</span></span>    |<span data-ttu-id="d6fb7-109">说明</span><span class="sxs-lookup"><span data-stu-id="d6fb7-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d6fb7-110">更新</span><span class="sxs-lookup"><span data-stu-id="d6fb7-110">Update</span></span>](../api/inferenceclassificationoverride-update.md) | [<span data-ttu-id="d6fb7-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d6fb7-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md) |<span data-ttu-id="d6fb7-112">按指定内容更改替代的 **ClassifyAs** 字段。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-112">Change the **ClassifyAs** field of an override as specified.</span></span> |
|[<span data-ttu-id="d6fb7-113">删除</span><span class="sxs-lookup"><span data-stu-id="d6fb7-113">Delete</span></span>](../api/inferenceclassificationoverride-delete.md) | <span data-ttu-id="d6fb7-114">无</span><span class="sxs-lookup"><span data-stu-id="d6fb7-114">None</span></span> |<span data-ttu-id="d6fb7-115">删除由其 ID 指定的替代。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-115">Delete an override specified by its ID.</span></span> |

## <a name="properties"></a><span data-ttu-id="d6fb7-116">属性</span><span class="sxs-lookup"><span data-stu-id="d6fb7-116">Properties</span></span>
| <span data-ttu-id="d6fb7-117">属性</span><span class="sxs-lookup"><span data-stu-id="d6fb7-117">Property</span></span>     | <span data-ttu-id="d6fb7-118">类型</span><span class="sxs-lookup"><span data-stu-id="d6fb7-118">Type</span></span>   |<span data-ttu-id="d6fb7-119">说明</span><span class="sxs-lookup"><span data-stu-id="d6fb7-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d6fb7-120">classifyAs</span><span class="sxs-lookup"><span data-stu-id="d6fb7-120">classifyAs</span></span>|<span data-ttu-id="d6fb7-121">inferenceClassificationType</span><span class="sxs-lookup"><span data-stu-id="d6fb7-121">inferenceClassificationType</span></span>| <span data-ttu-id="d6fb7-122">指定来自特定发件人的传入邮件始终应如何分类。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-122">Specifies how incoming messages from a specific sender should always be classified as.</span></span> <span data-ttu-id="d6fb7-123">可能的值为： `focused` 、 `other` 。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-123">The possible values are: `focused`, `other`.</span></span>|
|<span data-ttu-id="d6fb7-124">id</span><span class="sxs-lookup"><span data-stu-id="d6fb7-124">id</span></span>|<span data-ttu-id="d6fb7-125">string</span><span class="sxs-lookup"><span data-stu-id="d6fb7-125">string</span></span>| <span data-ttu-id="d6fb7-p102">替代的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-p102">The unique identifier of the override. Read-only.</span></span>|
|<span data-ttu-id="d6fb7-128">senderEmailAddress</span><span class="sxs-lookup"><span data-stu-id="d6fb7-128">senderEmailAddress</span></span>|[<span data-ttu-id="d6fb7-129">emailAddress</span><span class="sxs-lookup"><span data-stu-id="d6fb7-129">emailAddress</span></span>](emailaddress.md)|<span data-ttu-id="d6fb7-130">为其创建替代的发件人的电子邮件地址信息。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-130">The email address information of the sender for whom the override is created.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d6fb7-131">关系</span><span class="sxs-lookup"><span data-stu-id="d6fb7-131">Relationships</span></span>
<span data-ttu-id="d6fb7-132">无</span><span class="sxs-lookup"><span data-stu-id="d6fb7-132">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d6fb7-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d6fb7-133">JSON representation</span></span>

<span data-ttu-id="d6fb7-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6fb7-134">Here is a JSON representation of the resource.</span></span>

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
