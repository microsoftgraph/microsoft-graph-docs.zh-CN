---
title: externalItem 资源类型
description: 添加到 Microsoft Graph项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 7c570a7e4754724ca4239b7e3dbe128d09db9d75
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/10/2021
ms.locfileid: "53366526"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="eb1cc-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="eb1cc-103">externalItem resource type</span></span>

<span data-ttu-id="eb1cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eb1cc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="eb1cc-105">添加到 Microsoft Graph[项](externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

## <a name="methods"></a><span data-ttu-id="eb1cc-106">方法</span><span class="sxs-lookup"><span data-stu-id="eb1cc-106">Methods</span></span>

| <span data-ttu-id="eb1cc-107">方法</span><span class="sxs-lookup"><span data-stu-id="eb1cc-107">Method</span></span>                                                        | <span data-ttu-id="eb1cc-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="eb1cc-108">Return Type</span></span>                     | <span data-ttu-id="eb1cc-109">说明</span><span class="sxs-lookup"><span data-stu-id="eb1cc-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="eb1cc-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="eb1cc-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="eb1cc-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="eb1cc-113">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="eb1cc-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="eb1cc-115">获取 externalItem。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="eb1cc-116">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="eb1cc-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="eb1cc-118">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="eb1cc-119">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="eb1cc-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="eb1cc-120">无</span><span class="sxs-lookup"><span data-stu-id="eb1cc-120">None</span></span>                            | <span data-ttu-id="eb1cc-121">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="eb1cc-122">属性</span><span class="sxs-lookup"><span data-stu-id="eb1cc-122">Properties</span></span>

| <span data-ttu-id="eb1cc-123">属性</span><span class="sxs-lookup"><span data-stu-id="eb1cc-123">Property</span></span>   | <span data-ttu-id="eb1cc-124">类型</span><span class="sxs-lookup"><span data-stu-id="eb1cc-124">Type</span></span>                     | <span data-ttu-id="eb1cc-125">说明</span><span class="sxs-lookup"><span data-stu-id="eb1cc-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="eb1cc-126">acl</span><span class="sxs-lookup"><span data-stu-id="eb1cc-126">acl</span></span>        | <span data-ttu-id="eb1cc-127">[acl](acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="eb1cc-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="eb1cc-128">访问控制项数组。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-128">An array of access control entries.</span></span> <span data-ttu-id="eb1cc-129">每个条目指定授予用户或组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="eb1cc-130">必填。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-130">Required.</span></span> |
| <span data-ttu-id="eb1cc-131">content</span><span class="sxs-lookup"><span data-stu-id="eb1cc-131">content</span></span>    | [<span data-ttu-id="eb1cc-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="eb1cc-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="eb1cc-133">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="eb1cc-134">此属性中的文本已编制全文索引。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="eb1cc-135">可选。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-135">Optional.</span></span> |
| <span data-ttu-id="eb1cc-136">id</span><span class="sxs-lookup"><span data-stu-id="eb1cc-136">id</span></span>         | <span data-ttu-id="eb1cc-137">String</span><span class="sxs-lookup"><span data-stu-id="eb1cc-137">String</span></span>                   | <span data-ttu-id="eb1cc-138">开发人员提供的项目在包含[externalConnection 中的唯一 ID。](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="eb1cc-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="eb1cc-139">必须为字母数字，最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="eb1cc-140">必填。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-140">Required.</span></span> |
| <span data-ttu-id="eb1cc-141">properties</span><span class="sxs-lookup"><span data-stu-id="eb1cc-141">properties</span></span> | <span data-ttu-id="eb1cc-142">Object</span><span class="sxs-lookup"><span data-stu-id="eb1cc-142">Object</span></span>                   | <span data-ttu-id="eb1cc-143">具有项目属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="eb1cc-144">属性必须符合为[externalConnection](externalconnection.md)定义的架构。 [](schema.md)</span><span class="sxs-lookup"><span data-stu-id="eb1cc-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="eb1cc-145">必填。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="eb1cc-146">关系</span><span class="sxs-lookup"><span data-stu-id="eb1cc-146">Relationships</span></span>

<span data-ttu-id="eb1cc-147">无。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="eb1cc-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eb1cc-148">JSON representation</span></span>

<span data-ttu-id="eb1cc-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eb1cc-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [{"@odata.type": "microsoft.graph.acl"}],
  "content": {"@odata.type": "microsoft.graph.externalItemContent"},
  "id": "String (identifier)",
  "properties": "Object"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalItem resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: microsoft.graph.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
