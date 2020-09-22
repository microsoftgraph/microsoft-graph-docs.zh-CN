---
title: externalItem 资源类型
description: 添加到 Microsoft Graph 连接的项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: ec2c66c91612738295ac4ba49524593d61ff70e4
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193400"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="130cf-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="130cf-103">externalItem resource type</span></span>

<span data-ttu-id="130cf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="130cf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="130cf-105">添加到 Microsoft Graph [连接](externalconnection.md)的项。</span><span class="sxs-lookup"><span data-stu-id="130cf-105">An item added to a Microsoft Graph [connection](externalconnection.md).</span></span> 

[!INCLUDE [search-api-preview](../../includes/search-api-preview-signup.md)]

## <a name="methods"></a><span data-ttu-id="130cf-106">方法</span><span class="sxs-lookup"><span data-stu-id="130cf-106">Methods</span></span>

| <span data-ttu-id="130cf-107">方法</span><span class="sxs-lookup"><span data-stu-id="130cf-107">Method</span></span>                                                        | <span data-ttu-id="130cf-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="130cf-108">Return Type</span></span>                     | <span data-ttu-id="130cf-109">说明</span><span class="sxs-lookup"><span data-stu-id="130cf-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="130cf-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-110">Create externalItem</span></span>](../api/externalconnection-put-items.md) | [<span data-ttu-id="130cf-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-111">externalItem</span></span>](externalitem.md) | <span data-ttu-id="130cf-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="130cf-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="130cf-113">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-113">Get externalItem</span></span>](../api/externalitem-get.md)                | [<span data-ttu-id="130cf-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-114">externalItem</span></span>](externalitem.md) | <span data-ttu-id="130cf-115">获取 externalItem。</span><span class="sxs-lookup"><span data-stu-id="130cf-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="130cf-116">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-116">Update externalItem</span></span>](../api/externalitem-update.md)          | [<span data-ttu-id="130cf-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-117">externalItem</span></span>](externalitem.md) | <span data-ttu-id="130cf-118">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="130cf-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="130cf-119">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="130cf-119">Delete externalItem</span></span>](../api/externalitem-delete.md)          | <span data-ttu-id="130cf-120">无</span><span class="sxs-lookup"><span data-stu-id="130cf-120">None</span></span>                            | <span data-ttu-id="130cf-121">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="130cf-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="130cf-122">属性</span><span class="sxs-lookup"><span data-stu-id="130cf-122">Properties</span></span>

| <span data-ttu-id="130cf-123">属性</span><span class="sxs-lookup"><span data-stu-id="130cf-123">Property</span></span>   | <span data-ttu-id="130cf-124">类型</span><span class="sxs-lookup"><span data-stu-id="130cf-124">Type</span></span>                     | <span data-ttu-id="130cf-125">描述</span><span class="sxs-lookup"><span data-stu-id="130cf-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="130cf-126">acl</span><span class="sxs-lookup"><span data-stu-id="130cf-126">acl</span></span>        | <span data-ttu-id="130cf-127">[acl](acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="130cf-127">[acl](acl.md) collection</span></span> | <span data-ttu-id="130cf-128">一组访问控制项。</span><span class="sxs-lookup"><span data-stu-id="130cf-128">An array of access control entries.</span></span> <span data-ttu-id="130cf-129">每个条目指定向用户或组授予的访问权限。</span><span class="sxs-lookup"><span data-stu-id="130cf-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="130cf-130">必需。</span><span class="sxs-lookup"><span data-stu-id="130cf-130">Required.</span></span> |
| <span data-ttu-id="130cf-131">content</span><span class="sxs-lookup"><span data-stu-id="130cf-131">content</span></span>    | [<span data-ttu-id="130cf-132">externalItemContent</span><span class="sxs-lookup"><span data-stu-id="130cf-132">externalItemContent</span></span>](externalitemcontent.md) | <span data-ttu-id="130cf-133">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="130cf-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="130cf-134">此属性中的文本为全文检索的文本。</span><span class="sxs-lookup"><span data-stu-id="130cf-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="130cf-135">可选。</span><span class="sxs-lookup"><span data-stu-id="130cf-135">Optional.</span></span> |
| <span data-ttu-id="130cf-136">id</span><span class="sxs-lookup"><span data-stu-id="130cf-136">id</span></span>         | <span data-ttu-id="130cf-137">字符串</span><span class="sxs-lookup"><span data-stu-id="130cf-137">String</span></span>                   | <span data-ttu-id="130cf-138">开发人员提供的包含 [externalConnection](externalconnection.md)中的项的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="130cf-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="130cf-139">必须为字母数字，最多为128个字符。</span><span class="sxs-lookup"><span data-stu-id="130cf-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="130cf-140">必需。</span><span class="sxs-lookup"><span data-stu-id="130cf-140">Required.</span></span> |
| <span data-ttu-id="130cf-141">properties</span><span class="sxs-lookup"><span data-stu-id="130cf-141">properties</span></span> | <span data-ttu-id="130cf-142">Object</span><span class="sxs-lookup"><span data-stu-id="130cf-142">Object</span></span>                   | <span data-ttu-id="130cf-143">包含项属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="130cf-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="130cf-144">属性必须符合为[externalConnection](externalconnection.md)定义的[架构](schema.md)。</span><span class="sxs-lookup"><span data-stu-id="130cf-144">The properties MUST conform to the [schema](schema.md) defined for the [externalConnection](externalconnection.md).</span></span> <span data-ttu-id="130cf-145">必填。</span><span class="sxs-lookup"><span data-stu-id="130cf-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="130cf-146">关系</span><span class="sxs-lookup"><span data-stu-id="130cf-146">Relationships</span></span>

<span data-ttu-id="130cf-147">无。</span><span class="sxs-lookup"><span data-stu-id="130cf-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="130cf-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="130cf-148">JSON representation</span></span>

<span data-ttu-id="130cf-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="130cf-149">The following is a JSON representation of the resource.</span></span>

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
