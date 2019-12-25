---
title: externalItem 资源类型
description: 通过 Microsoft Search 连接编制索引的项目。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 5a396d41ffaf0e602a586635296586cbdce42f50
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40866824"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="119bb-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="119bb-103">externalItem resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="119bb-104">通过 Microsoft Search[连接](externalconnection.md)编制索引的项目。</span><span class="sxs-lookup"><span data-stu-id="119bb-104">An item indexed via a Microsoft Search [connection](externalconnection.md).</span></span>

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="119bb-105">方法</span><span class="sxs-lookup"><span data-stu-id="119bb-105">Methods</span></span>

| <span data-ttu-id="119bb-106">方法</span><span class="sxs-lookup"><span data-stu-id="119bb-106">Method</span></span>                                                        | <span data-ttu-id="119bb-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="119bb-107">Return Type</span></span>                     | <span data-ttu-id="119bb-108">说明</span><span class="sxs-lookup"><span data-stu-id="119bb-108">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="119bb-109">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="119bb-109">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="119bb-110">externalItem</span><span class="sxs-lookup"><span data-stu-id="119bb-110">externalItem</span></span>](externalitem.md) | <span data-ttu-id="119bb-111">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="119bb-111">Create an externalItem.</span></span> |
| [<span data-ttu-id="119bb-112">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="119bb-112">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="119bb-113">externalItem</span><span class="sxs-lookup"><span data-stu-id="119bb-113">externalItem</span></span>](externalitem.md) | <span data-ttu-id="119bb-114">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="119bb-114">Update an externalItem.</span></span> |
| [<span data-ttu-id="119bb-115">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="119bb-115">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="119bb-116">无</span><span class="sxs-lookup"><span data-stu-id="119bb-116">None</span></span>                            | <span data-ttu-id="119bb-117">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="119bb-117">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="119bb-118">属性</span><span class="sxs-lookup"><span data-stu-id="119bb-118">Properties</span></span>

| <span data-ttu-id="119bb-119">属性</span><span class="sxs-lookup"><span data-stu-id="119bb-119">Property</span></span>   | <span data-ttu-id="119bb-120">类型</span><span class="sxs-lookup"><span data-stu-id="119bb-120">Type</span></span>                     | <span data-ttu-id="119bb-121">说明</span><span class="sxs-lookup"><span data-stu-id="119bb-121">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="119bb-122">acl</span><span class="sxs-lookup"><span data-stu-id="119bb-122">acl</span></span>        | <span data-ttu-id="119bb-123">[acl](acl.md)集合</span><span class="sxs-lookup"><span data-stu-id="119bb-123">[acl](acl.md) collection</span></span> | <span data-ttu-id="119bb-124">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="119bb-124">An array of access control entries.</span></span> <span data-ttu-id="119bb-125">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="119bb-125">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="119bb-126">必需。</span><span class="sxs-lookup"><span data-stu-id="119bb-126">Required.</span></span> |
| <span data-ttu-id="119bb-127">内容</span><span class="sxs-lookup"><span data-stu-id="119bb-127">content</span></span>    | <span data-ttu-id="119bb-128">String</span><span class="sxs-lookup"><span data-stu-id="119bb-128">String</span></span>                   | <span data-ttu-id="119bb-129">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="119bb-129">A plain-text representation of the contents of the item.</span></span> <span data-ttu-id="119bb-130">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="119bb-130">The text in this property is full-text indexed.</span></span> <span data-ttu-id="119bb-131">可选。</span><span class="sxs-lookup"><span data-stu-id="119bb-131">Optional.</span></span> |
| <span data-ttu-id="119bb-132">id</span><span class="sxs-lookup"><span data-stu-id="119bb-132">id</span></span>         | <span data-ttu-id="119bb-133">String</span><span class="sxs-lookup"><span data-stu-id="119bb-133">String</span></span>                   | <span data-ttu-id="119bb-134">开发人员提供的包含[externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="119bb-134">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="119bb-135">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="119bb-135">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="119bb-136">必需。</span><span class="sxs-lookup"><span data-stu-id="119bb-136">Required.</span></span> |
| <span data-ttu-id="119bb-137">properties</span><span class="sxs-lookup"><span data-stu-id="119bb-137">properties</span></span> | <span data-ttu-id="119bb-138">对象</span><span class="sxs-lookup"><span data-stu-id="119bb-138">Object</span></span>                   | <span data-ttu-id="119bb-139">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="119bb-139">A property bag with the properties of the item.</span></span> <span data-ttu-id="119bb-140">属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="119bb-140">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="119bb-141">必需。</span><span class="sxs-lookup"><span data-stu-id="119bb-141">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="119bb-142">关系</span><span class="sxs-lookup"><span data-stu-id="119bb-142">Relationships</span></span>

<span data-ttu-id="119bb-143">无</span><span class="sxs-lookup"><span data-stu-id="119bb-143">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="119bb-144">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="119bb-144">JSON representation</span></span>

<span data-ttu-id="119bb-145">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="119bb-145">The following is a JSON representation of the resource.</span></span>

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
