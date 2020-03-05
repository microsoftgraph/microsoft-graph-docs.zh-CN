---
title: externalItem 资源类型
description: 通过 Microsoft Search 连接编制索引的项目。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e115135bedecfe4b055e028d5c19902a068c8a53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42498698"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="63aa4-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="63aa4-103">externalItem resource type</span></span>

<span data-ttu-id="63aa4-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="63aa4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63aa4-105">通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="63aa4-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="63aa4-106">方法</span><span class="sxs-lookup"><span data-stu-id="63aa4-106">Methods</span></span>

| <span data-ttu-id="63aa4-107">方法</span><span class="sxs-lookup"><span data-stu-id="63aa4-107">Method</span></span>                                                        | <span data-ttu-id="63aa4-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="63aa4-108">Return Type</span></span>                     | <span data-ttu-id="63aa4-109">说明</span><span class="sxs-lookup"><span data-stu-id="63aa4-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="63aa4-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="63aa4-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="63aa4-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="63aa4-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="63aa4-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="63aa4-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="63aa4-113">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="63aa4-113">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="63aa4-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="63aa4-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="63aa4-115">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="63aa4-115">Update an externalItem.</span></span> |
| [<span data-ttu-id="63aa4-116">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="63aa4-116">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="63aa4-117">无</span><span class="sxs-lookup"><span data-stu-id="63aa4-117">None</span></span>                            | <span data-ttu-id="63aa4-118">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="63aa4-118">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="63aa4-119">属性</span><span class="sxs-lookup"><span data-stu-id="63aa4-119">Properties</span></span>

| <span data-ttu-id="63aa4-120">属性</span><span class="sxs-lookup"><span data-stu-id="63aa4-120">Property</span></span>   | <span data-ttu-id="63aa4-121">类型</span><span class="sxs-lookup"><span data-stu-id="63aa4-121">Type</span></span>                     | <span data-ttu-id="63aa4-122">说明</span><span class="sxs-lookup"><span data-stu-id="63aa4-122">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="63aa4-123">acl</span><span class="sxs-lookup"><span data-stu-id="63aa4-123">acl</span></span>        | <span data-ttu-id="63aa4-124">[acl](acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="63aa4-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="63aa4-125">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="63aa4-125">An array of access control entries.</span></span> <span data-ttu-id="63aa4-126">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="63aa4-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="63aa4-127">必填。</span><span class="sxs-lookup"><span data-stu-id="63aa4-127">Required.</span></span> |
| <span data-ttu-id="63aa4-128">内容</span><span class="sxs-lookup"><span data-stu-id="63aa4-128">content</span></span>    | <span data-ttu-id="63aa4-129">String</span><span class="sxs-lookup"><span data-stu-id="63aa4-129">String</span></span>                   | <span data-ttu-id="63aa4-130">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="63aa4-130">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="63aa4-131">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="63aa4-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="63aa4-132">可选。</span><span class="sxs-lookup"><span data-stu-id="63aa4-132">Optional.</span></span> |
| <span data-ttu-id="63aa4-133">id</span><span class="sxs-lookup"><span data-stu-id="63aa4-133">id</span></span>         | <span data-ttu-id="63aa4-134">String</span><span class="sxs-lookup"><span data-stu-id="63aa4-134">String</span></span>                   | <span data-ttu-id="63aa4-135">开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="63aa4-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="63aa4-136">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="63aa4-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="63aa4-137">必填。</span><span class="sxs-lookup"><span data-stu-id="63aa4-137">Required.</span></span> |
| <span data-ttu-id="63aa4-138">properties</span><span class="sxs-lookup"><span data-stu-id="63aa4-138">properties</span></span> | <span data-ttu-id="63aa4-139">Object</span><span class="sxs-lookup"><span data-stu-id="63aa4-139">Object</span></span>                   | <span data-ttu-id="63aa4-140">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="63aa4-140">A property bag with the properties of the item.</span></span> <span data-ttu-id="63aa4-141">属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="63aa4-141">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="63aa4-142">必填。</span><span class="sxs-lookup"><span data-stu-id="63aa4-142">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="63aa4-143">关系</span><span class="sxs-lookup"><span data-stu-id="63aa4-143">Relationships</span></span>

<span data-ttu-id="63aa4-144">无</span><span class="sxs-lookup"><span data-stu-id="63aa4-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="63aa4-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="63aa4-145">JSON representation</span></span>

<span data-ttu-id="63aa4-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="63aa4-146">The following is a JSON representation of the resource.</span></span>

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
  "content": "String",
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
