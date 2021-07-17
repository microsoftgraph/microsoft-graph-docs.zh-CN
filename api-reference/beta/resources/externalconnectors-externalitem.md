---
title: externalItem 资源类型
description: 添加到 Microsoft Graph项。
localization_priority: Normal
author: snlraju-msft
ms.prod: search
doc_type: resourcePageType
ms.openlocfilehash: 8660365d5d08d0084066cea3349e841269469241
ms.sourcegitcommit: 1940be9846055aa650c6c03982b74a961f1e316a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/17/2021
ms.locfileid: "53467666"
---
# <a name="externalitem-resource-type"></a><span data-ttu-id="b1372-103">externalItem 资源类型</span><span class="sxs-lookup"><span data-stu-id="b1372-103">externalItem resource type</span></span>

<span data-ttu-id="b1372-104">命名空间：microsoft.graph.externalConnectors</span><span class="sxs-lookup"><span data-stu-id="b1372-104">Namespace: microsoft.graph.externalConnectors</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b1372-105">添加到 Microsoft Graph[项](externalconnectors-externalconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="b1372-105">An item added to a Microsoft Graph [connection](externalconnectors-externalconnection.md).</span></span>

## <a name="methods"></a><span data-ttu-id="b1372-106">方法</span><span class="sxs-lookup"><span data-stu-id="b1372-106">Methods</span></span>

| <span data-ttu-id="b1372-107">方法</span><span class="sxs-lookup"><span data-stu-id="b1372-107">Method</span></span>                                                        | <span data-ttu-id="b1372-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="b1372-108">Return Type</span></span>                     | <span data-ttu-id="b1372-109">说明</span><span class="sxs-lookup"><span data-stu-id="b1372-109">Description</span></span> |
|:--------------------------------------------------------------|:--------------------------------|:--|
| [<span data-ttu-id="b1372-110">创建 externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-110">Create externalItem</span></span>](../api/externalconnectors-externalconnection-put-items.md) | [<span data-ttu-id="b1372-111">externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-111">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="b1372-112">创建 externalItem。</span><span class="sxs-lookup"><span data-stu-id="b1372-112">Create an externalItem.</span></span> |
| [<span data-ttu-id="b1372-113">获取 externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-113">Get externalItem</span></span>](../api/externalconnectors-externalitem-get.md)                | [<span data-ttu-id="b1372-114">externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-114">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="b1372-115">获取 externalItem。</span><span class="sxs-lookup"><span data-stu-id="b1372-115">Get an externalItem.</span></span>    |
| [<span data-ttu-id="b1372-116">更新 externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-116">Update externalItem</span></span>](../api/externalconnectors-externalitem-update.md)          | [<span data-ttu-id="b1372-117">externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-117">externalItem</span></span>](externalconnectors-externalitem.md) | <span data-ttu-id="b1372-118">更新 externalItem。</span><span class="sxs-lookup"><span data-stu-id="b1372-118">Update an externalItem.</span></span> |
| [<span data-ttu-id="b1372-119">删除 externalItem</span><span class="sxs-lookup"><span data-stu-id="b1372-119">Delete externalItem</span></span>](../api/externalconnectors-externalitem-delete.md)          | <span data-ttu-id="b1372-120">无</span><span class="sxs-lookup"><span data-stu-id="b1372-120">None</span></span>                            | <span data-ttu-id="b1372-121">删除 externalItem。</span><span class="sxs-lookup"><span data-stu-id="b1372-121">Delete an externalItem.</span></span> |

## <a name="properties"></a><span data-ttu-id="b1372-122">属性</span><span class="sxs-lookup"><span data-stu-id="b1372-122">Properties</span></span>

| <span data-ttu-id="b1372-123">属性</span><span class="sxs-lookup"><span data-stu-id="b1372-123">Property</span></span>   | <span data-ttu-id="b1372-124">类型</span><span class="sxs-lookup"><span data-stu-id="b1372-124">Type</span></span>                     | <span data-ttu-id="b1372-125">说明</span><span class="sxs-lookup"><span data-stu-id="b1372-125">Description</span></span>                          |
|:-----------|:-------------------------|:-------------------------------------|
| <span data-ttu-id="b1372-126">acl</span><span class="sxs-lookup"><span data-stu-id="b1372-126">acl</span></span>        | <span data-ttu-id="b1372-127">[microsoft.graph.externalConnectors.acl](externalconnectors-acl.md) 集合</span><span class="sxs-lookup"><span data-stu-id="b1372-127">[microsoft.graph.externalConnectors.acl](externalconnectors-acl.md) collection</span></span> | <span data-ttu-id="b1372-128">访问控制项数组。</span><span class="sxs-lookup"><span data-stu-id="b1372-128">An array of access control entries.</span></span> <span data-ttu-id="b1372-129">每个条目指定授予用户或组的访问权限。</span><span class="sxs-lookup"><span data-stu-id="b1372-129">Each entry specifies the access granted to a user or group.</span></span> <span data-ttu-id="b1372-130">必需项。</span><span class="sxs-lookup"><span data-stu-id="b1372-130">Required.</span></span> |
| <span data-ttu-id="b1372-131">content</span><span class="sxs-lookup"><span data-stu-id="b1372-131">content</span></span>    | [<span data-ttu-id="b1372-132">microsoft.graph.externalConnectors.externalItemContent</span><span class="sxs-lookup"><span data-stu-id="b1372-132">microsoft.graph.externalConnectors.externalItemContent</span></span>](externalconnectors-externalitemcontent.md) | <span data-ttu-id="b1372-133">项目内容的纯文本表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1372-133">A plain-text  representation of the contents of the item.</span></span> <span data-ttu-id="b1372-134">此属性中的文本已编制全文索引。</span><span class="sxs-lookup"><span data-stu-id="b1372-134">The text in this property is full-text indexed.</span></span> <span data-ttu-id="b1372-135">可选。</span><span class="sxs-lookup"><span data-stu-id="b1372-135">Optional.</span></span> |
| <span data-ttu-id="b1372-136">id</span><span class="sxs-lookup"><span data-stu-id="b1372-136">id</span></span>         | <span data-ttu-id="b1372-137">String</span><span class="sxs-lookup"><span data-stu-id="b1372-137">String</span></span>                   | <span data-ttu-id="b1372-138">开发人员提供的项目在包含[externalConnection 中的唯一 ID。](externalconnectors-externalconnection.md)</span><span class="sxs-lookup"><span data-stu-id="b1372-138">Developer-provided unique ID of the item within the containing [externalConnection](externalconnectors-externalconnection.md).</span></span> <span data-ttu-id="b1372-139">必须为字母数字，最多为 128 个字符。</span><span class="sxs-lookup"><span data-stu-id="b1372-139">Must be alphanumeric and a maximum of 128 characters.</span></span> <span data-ttu-id="b1372-140">必需项。</span><span class="sxs-lookup"><span data-stu-id="b1372-140">Required.</span></span> |
| <span data-ttu-id="b1372-141">properties</span><span class="sxs-lookup"><span data-stu-id="b1372-141">properties</span></span> | <span data-ttu-id="b1372-142">Object</span><span class="sxs-lookup"><span data-stu-id="b1372-142">Object</span></span>                   | <span data-ttu-id="b1372-143">具有项目属性的属性包。</span><span class="sxs-lookup"><span data-stu-id="b1372-143">A property bag with the properties of the item.</span></span> <span data-ttu-id="b1372-144">属性必须符合为[externalConnection](externalconnectors-externalconnection.md)定义的架构。 [](externalconnectors-schema.md)</span><span class="sxs-lookup"><span data-stu-id="b1372-144">The properties MUST conform to the [schema](externalconnectors-schema.md) defined for the [externalConnection](externalconnectors-externalconnection.md).</span></span> <span data-ttu-id="b1372-145">必填。</span><span class="sxs-lookup"><span data-stu-id="b1372-145">Required.</span></span> |

## <a name="relationships"></a><span data-ttu-id="b1372-146">关系</span><span class="sxs-lookup"><span data-stu-id="b1372-146">Relationships</span></span>

<span data-ttu-id="b1372-147">无。</span><span class="sxs-lookup"><span data-stu-id="b1372-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b1372-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b1372-148">JSON representation</span></span>

<span data-ttu-id="b1372-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b1372-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  ],
  "@odata.type": "microsoft.graph.externalConnectors.externalItem",
  "keyProperty": "id"
}-->

```json
{
  "acl": [
    {
      "type": "everyone",
      "value": "67a141d8-cf4e-4528-ba07-bed21bfacd2d",
      "accessType": "grant",
      "identitySource": "azureActiveDirectory"
    }
  ],
  "id": "String (identifier)",
  "properties": "Object",
  "content": { "@odata.type": "microsoft.graph.externalConnectors.externalItemContent" }
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
    "Error: microsoft.graph.externalConnectors.externalItem/properties:\r\n      Referenced type microsoft.graph.object is not defined in the doc set! Potential suggestion: microsoft.graph.directoryObject"
  ]
}-->
