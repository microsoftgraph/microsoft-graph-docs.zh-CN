---
title: externalItem 资源类型
description: 通过 Microsoft Search 连接编制索引的项目。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: d775cfefa7a0cd1fdb87a291ba7ac61bb4b40782
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48013704"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="6dd17-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="6dd17-103">externalItem resource type</span></span>

<span data-ttu-id="6dd17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dd17-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dd17-105">通过 Microsoft Search [连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="6dd17-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="6dd17-106">方法</span><span class="sxs-lookup"><span data-stu-id="6dd17-106">Methods</span></span>

| <span data-ttu-id="6dd17-107">方法</span><span class="sxs-lookup"><span data-stu-id="6dd17-107">Method</span></span>                                                        | <span data-ttu-id="6dd17-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="6dd17-108">Return Type</span></span>                     | <span data-ttu-id="6dd17-109">说明</span><span class="sxs-lookup"><span data-stu-id="6dd17-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="6dd17-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="6dd17-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="6dd17-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="6dd17-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="6dd17-113">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="6dd17-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="6dd17-115">获取 externalItem。</span><span class="sxs-lookup"><span data-stu-id="6dd17-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="6dd17-116">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="6dd17-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="6dd17-118">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="6dd17-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="6dd17-119">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="6dd17-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="6dd17-120">无</span><span class="sxs-lookup"><span data-stu-id="6dd17-120">None</span></span>                            | <span data-ttu-id="6dd17-121">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="6dd17-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="6dd17-122">属性</span><span class="sxs-lookup"><span data-stu-id="6dd17-122">Properties</span></span>

| <span data-ttu-id="6dd17-123">属性</span><span class="sxs-lookup"><span data-stu-id="6dd17-123">Property</span></span>   | <span data-ttu-id="6dd17-124">类型</span><span class="sxs-lookup"><span data-stu-id="6dd17-124">Type</span></span>                     | <span data-ttu-id="6dd17-125">说明</span><span class="sxs-lookup"><span data-stu-id="6dd17-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="6dd17-126">acl</span><span class="sxs-lookup"><span data-stu-id="6dd17-126">acl</span></span>        | <span data-ttu-id="6dd17-127">[acl](acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="6dd17-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="6dd17-128">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="6dd17-128">An array of access control entries.</span></span> <span data-ttu-id="6dd17-129">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="6dd17-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="6dd17-130">必需。</span><span class="sxs-lookup"><span data-stu-id="6dd17-130">Required.</span></span> |
| <span data-ttu-id="6dd17-131">content</span><span class="sxs-lookup"><span data-stu-id="6dd17-131">content</span></span>    | [<span data-ttu-id="6dd17-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="6dd17-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="6dd17-133">项目内容的纯文本或 HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dd17-133">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="6dd17-134">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="6dd17-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="6dd17-135">可选。</span><span class="sxs-lookup"><span data-stu-id="6dd17-135">Optional.</span></span> |
| <span data-ttu-id="6dd17-136">id</span><span class="sxs-lookup"><span data-stu-id="6dd17-136">id</span></span>         | <span data-ttu-id="6dd17-137">String</span><span class="sxs-lookup"><span data-stu-id="6dd17-137">String</span></span>                   | <span data-ttu-id="6dd17-138">开发人员提供的包含 [externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="6dd17-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="6dd17-139">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="6dd17-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="6dd17-140">必需。</span><span class="sxs-lookup"><span data-stu-id="6dd17-140">Required.</span></span> |
| <span data-ttu-id="6dd17-141">properties</span><span class="sxs-lookup"><span data-stu-id="6dd17-141">properties</span></span> | <span data-ttu-id="6dd17-142">Object</span><span class="sxs-lookup"><span data-stu-id="6dd17-142">Object</span></span>                   | <span data-ttu-id="6dd17-143">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="6dd17-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="6dd17-144">属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="6dd17-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="6dd17-145">必需。</span><span class="sxs-lookup"><span data-stu-id="6dd17-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="6dd17-146">关系</span><span class="sxs-lookup"><span data-stu-id="6dd17-146">Relationships</span></span>

<span data-ttu-id="6dd17-147">无。</span><span class="sxs-lookup"><span data-stu-id="6dd17-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6dd17-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6dd17-148">JSON representation</span></span>

<span data-ttu-id="6dd17-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6dd17-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalItem",
  "baseType": "",
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


