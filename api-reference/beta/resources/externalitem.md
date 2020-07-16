---
title: externalItem 资源类型
description: 通过 Microsoft Search 连接编制索引的项目。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 3b82f67f12d263e56e3375ed87a9d6dff71c2204
ms.sourcegitcommit: 05645bc582d14781a9ca6b78ed598a4e7dc26869
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "44989821"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="7c7ec-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="7c7ec-103">externalItem resource type</span></span>

<span data-ttu-id="7c7ec-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c7ec-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7c7ec-105">通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="7c7ec-106">方法</span><span class="sxs-lookup"><span data-stu-id="7c7ec-106">Methods</span></span>

| <span data-ttu-id="7c7ec-107">方法</span><span class="sxs-lookup"><span data-stu-id="7c7ec-107">Method</span></span>                                                        | <span data-ttu-id="7c7ec-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="7c7ec-108">Return Type</span></span>                     | <span data-ttu-id="7c7ec-109">说明</span><span class="sxs-lookup"><span data-stu-id="7c7ec-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="7c7ec-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="7c7ec-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="7c7ec-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="7c7ec-113">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="7c7ec-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="7c7ec-115">获取 externalItem。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="7c7ec-116">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="7c7ec-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="7c7ec-118">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="7c7ec-119">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="7c7ec-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="7c7ec-120">无</span><span class="sxs-lookup"><span data-stu-id="7c7ec-120">None</span></span>                            | <span data-ttu-id="7c7ec-121">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="7c7ec-122">属性</span><span class="sxs-lookup"><span data-stu-id="7c7ec-122">Properties</span></span>

| <span data-ttu-id="7c7ec-123">属性</span><span class="sxs-lookup"><span data-stu-id="7c7ec-123">Property</span></span>   | <span data-ttu-id="7c7ec-124">类型</span><span class="sxs-lookup"><span data-stu-id="7c7ec-124">Type</span></span>                     | <span data-ttu-id="7c7ec-125">说明</span><span class="sxs-lookup"><span data-stu-id="7c7ec-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="7c7ec-126">acl</span><span class="sxs-lookup"><span data-stu-id="7c7ec-126">acl</span></span>        | <span data-ttu-id="7c7ec-127">[acl](acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="7c7ec-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="7c7ec-128">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-128">An array of access control entries.</span></span> <span data-ttu-id="7c7ec-129">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="7c7ec-130">必需。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-130">Required.</span></span> |
| <span data-ttu-id="7c7ec-131">content</span><span class="sxs-lookup"><span data-stu-id="7c7ec-131">content</span></span>    | [<span data-ttu-id="7c7ec-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="7c7ec-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="7c7ec-133">项目内容的纯文本或 HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-133">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="7c7ec-134">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="7c7ec-135">可选。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-135">Optional.</span></span> |
| <span data-ttu-id="7c7ec-136">id</span><span class="sxs-lookup"><span data-stu-id="7c7ec-136">id</span></span>         | <span data-ttu-id="7c7ec-137">String</span><span class="sxs-lookup"><span data-stu-id="7c7ec-137">String</span></span>                   | <span data-ttu-id="7c7ec-138">开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="7c7ec-139">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="7c7ec-140">必需。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-140">Required.</span></span> |
| <span data-ttu-id="7c7ec-141">properties</span><span class="sxs-lookup"><span data-stu-id="7c7ec-141">properties</span></span> | <span data-ttu-id="7c7ec-142">对象</span><span class="sxs-lookup"><span data-stu-id="7c7ec-142">Object</span></span>                   | <span data-ttu-id="7c7ec-143">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="7c7ec-144">属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="7c7ec-145">必需。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="7c7ec-146">关系</span><span class="sxs-lookup"><span data-stu-id="7c7ec-146">Relationships</span></span>

<span data-ttu-id="7c7ec-147">无。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="7c7ec-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7c7ec-148">JSON representation</span></span>

<span data-ttu-id="7c7ec-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7c7ec-149">The following is a JSON representation of the resource.</span></span>

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
