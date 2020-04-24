---
title: externalItem 资源类型
description: 通过 Microsoft Search 连接编制索引的项目。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: e1497528e759a2fb5556aed3e9b936b1c9797ee0
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43805657"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="53501-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="53501-103">externalItem resource type</span></span>

<span data-ttu-id="53501-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53501-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53501-105">通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="53501-105">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="53501-106">Methods</span><span class="sxs-lookup"><span data-stu-id="53501-106">Methods</span></span>

| <span data-ttu-id="53501-107">方法</span><span class="sxs-lookup"><span data-stu-id="53501-107">Method</span></span>                                                        | <span data-ttu-id="53501-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="53501-108">Return Type</span></span>                     | <span data-ttu-id="53501-109">说明</span><span class="sxs-lookup"><span data-stu-id="53501-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="53501-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="53501-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="53501-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="53501-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="53501-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="53501-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="53501-113">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="53501-113">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="53501-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="53501-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="53501-115">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="53501-115">Update an externalItem.</span></span> |
| [<span data-ttu-id="53501-116">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="53501-116">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="53501-117">无</span><span class="sxs-lookup"><span data-stu-id="53501-117">None</span></span>                            | <span data-ttu-id="53501-118">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="53501-118">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="53501-119">属性</span><span class="sxs-lookup"><span data-stu-id="53501-119">Properties</span></span>

| <span data-ttu-id="53501-120">属性</span><span class="sxs-lookup"><span data-stu-id="53501-120">Property</span></span>   | <span data-ttu-id="53501-121">类型</span><span class="sxs-lookup"><span data-stu-id="53501-121">Type</span></span>                     | <span data-ttu-id="53501-122">说明</span><span class="sxs-lookup"><span data-stu-id="53501-122">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="53501-123">acl</span><span class="sxs-lookup"><span data-stu-id="53501-123">acl</span></span>        | <span data-ttu-id="53501-124">[acl](acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="53501-124">[acl](acl.md) collection</span></span> | <span data-ttu-id="53501-125">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="53501-125">An array of access control entries.</span></span> <span data-ttu-id="53501-126">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="53501-126">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="53501-127">必需。</span><span class="sxs-lookup"><span data-stu-id="53501-127">Required.</span></span> |
| <span data-ttu-id="53501-128">content</span><span class="sxs-lookup"><span data-stu-id="53501-128">content</span></span>    | [<span data-ttu-id="53501-129">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="53501-129">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="53501-130">项目内容的纯文本或 HTML 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53501-130">A plain-text or HTML representation of the contents of the item.</span></span> <span data-ttu-id="53501-131">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="53501-131">The text in this property is full-text indexed.</span></span> <span data-ttu-id="53501-132">可选。</span><span class="sxs-lookup"><span data-stu-id="53501-132">Optional.</span></span> |
| <span data-ttu-id="53501-133">id</span><span class="sxs-lookup"><span data-stu-id="53501-133">id</span></span>         | <span data-ttu-id="53501-134">字符串</span><span class="sxs-lookup"><span data-stu-id="53501-134">String</span></span>                   | <span data-ttu-id="53501-135">开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="53501-135">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="53501-136">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="53501-136">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="53501-137">必需。</span><span class="sxs-lookup"><span data-stu-id="53501-137">Required.</span></span> |
| <span data-ttu-id="53501-138">properties</span><span class="sxs-lookup"><span data-stu-id="53501-138">properties</span></span> | <span data-ttu-id="53501-139">对象</span><span class="sxs-lookup"><span data-stu-id="53501-139">Object</span></span>                   | <span data-ttu-id="53501-140">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="53501-140">A property bag with the properties of the item.</span></span> <span data-ttu-id="53501-141">属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="53501-141">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="53501-142">必需。</span><span class="sxs-lookup"><span data-stu-id="53501-142">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="53501-143">关系</span><span class="sxs-lookup"><span data-stu-id="53501-143">Relationships</span></span>

<span data-ttu-id="53501-144">无</span><span class="sxs-lookup"><span data-stu-id="53501-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="53501-145">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53501-145">JSON representation</span></span>

<span data-ttu-id="53501-146">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53501-146">The following is a JSON representation of the resource.</span></span>

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
