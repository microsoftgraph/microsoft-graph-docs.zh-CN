---
title: externalItem 资源类型
description: 添加到 Microsoft Graph 连接中的项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 63f0285427a17280169d31a35c3a622d38a6a8c6
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50161698"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="13b78-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="13b78-103">externalItem resource type</span></span>

<span data-ttu-id="13b78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13b78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="13b78-105">添加到 Microsoft Graph 连接 [中的项](externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="13b78-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="13b78-106">方法</span><span class="sxs-lookup"><span data-stu-id="13b78-106">Methods</span></span>

| <span data-ttu-id="13b78-107">方法</span><span class="sxs-lookup"><span data-stu-id="13b78-107">Method</span></span>                                                        | <span data-ttu-id="13b78-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="13b78-108">Return Type</span></span>                     | <span data-ttu-id="13b78-109">说明</span><span class="sxs-lookup"><span data-stu-id="13b78-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="13b78-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="13b78-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="13b78-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="13b78-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="13b78-113">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="13b78-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="13b78-115">获取 externalItem。</span><span class="sxs-lookup"><span data-stu-id="13b78-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="13b78-116">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="13b78-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="13b78-118">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="13b78-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="13b78-119">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="13b78-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="13b78-120">无</span><span class="sxs-lookup"><span data-stu-id="13b78-120">None</span></span>                            | <span data-ttu-id="13b78-121">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="13b78-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="13b78-122">属性</span><span class="sxs-lookup"><span data-stu-id="13b78-122">Properties</span></span>

| <span data-ttu-id="13b78-123">属性</span><span class="sxs-lookup"><span data-stu-id="13b78-123">Property</span></span>   | <span data-ttu-id="13b78-124">类型</span><span class="sxs-lookup"><span data-stu-id="13b78-124">Type</span></span>                     | <span data-ttu-id="13b78-125">说明</span><span class="sxs-lookup"><span data-stu-id="13b78-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="13b78-126">acl</span><span class="sxs-lookup"><span data-stu-id="13b78-126">acl</span></span>        | <span data-ttu-id="13b78-127">[acl](acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="13b78-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="13b78-128">访问控制项数组。</span><span class="sxs-lookup"><span data-stu-id="13b78-128">An array of access control entries.</span></span> <span data-ttu-id="13b78-129">每个条目指定授予用户或组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="13b78-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="13b78-130">必需。</span><span class="sxs-lookup"><span data-stu-id="13b78-130">Required.</span></span> |
| <span data-ttu-id="13b78-131">content</span><span class="sxs-lookup"><span data-stu-id="13b78-131">content</span></span>    | [<span data-ttu-id="13b78-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="13b78-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="13b78-133">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="13b78-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="13b78-134">此属性中的文本是全文索引。</span><span class="sxs-lookup"><span data-stu-id="13b78-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="13b78-135">可选。</span><span class="sxs-lookup"><span data-stu-id="13b78-135">Optional.</span></span> |
| <span data-ttu-id="13b78-136">id</span><span class="sxs-lookup"><span data-stu-id="13b78-136">id</span></span>         | <span data-ttu-id="13b78-137">String</span><span class="sxs-lookup"><span data-stu-id="13b78-137">String</span></span>                   | <span data-ttu-id="13b78-138">开发人员提供包含外部Connection 中的项的唯一[ID。](externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="13b78-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="13b78-139">必须为字母数字，最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="13b78-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="13b78-140">必需。</span><span class="sxs-lookup"><span data-stu-id="13b78-140">Required.</span></span> |
| <span data-ttu-id="13b78-141">properties</span><span class="sxs-lookup"><span data-stu-id="13b78-141">properties</span></span> | <span data-ttu-id="13b78-142">Object</span><span class="sxs-lookup"><span data-stu-id="13b78-142">Object</span></span>                   | <span data-ttu-id="13b78-143">具有项目属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="13b78-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="13b78-144">属性必须符合为[externalConnection](externalconnection.md)定义的架构。 [](schema.md)</span><span class="sxs-lookup"><span data-stu-id="13b78-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="13b78-145">必填。</span><span class="sxs-lookup"><span data-stu-id="13b78-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="13b78-146">关系</span><span class="sxs-lookup"><span data-stu-id="13b78-146">Relationships</span></span>

<span data-ttu-id="13b78-147">无。</span><span class="sxs-lookup"><span data-stu-id="13b78-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="13b78-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13b78-148">JSON representation</span></span>

<span data-ttu-id="13b78-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13b78-149">The following is a JSON representation of the resource.</span></span>

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
