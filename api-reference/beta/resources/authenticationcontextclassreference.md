---
title: authenticationContextClassReference 资源类型
description: 表示一Azure Active Directory身份验证上下文类引用。
localization_priority: Normal
author: calebb
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 1397545d7b102d05b8c71957cea88f9c131f0e09
ms.sourcegitcommit: d700b7e3b411e3226b5adf1f213539f05fe802e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52547412"
---
# <a name="authenticationcontextclassreference-resource-type"></a><span data-ttu-id="4abf7-103">authenticationContextClassReference 资源类型</span><span class="sxs-lookup"><span data-stu-id="4abf7-103">authenticationContextClassReference resource type</span></span>

<span data-ttu-id="4abf7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4abf7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4abf7-105">表示一Azure Active Directory身份验证上下文类引用。</span><span class="sxs-lookup"><span data-stu-id="4abf7-105">Represents an Azure Active Directory authentication context class reference.</span></span> <span data-ttu-id="4abf7-106">身份验证上下文类引用是定义条件访问身份验证要求的自定义值。</span><span class="sxs-lookup"><span data-stu-id="4abf7-106">Authentication context class references are custom values that define a Conditional Access authentication requirement.</span></span>

## <a name="methods"></a><span data-ttu-id="4abf7-107">方法</span><span class="sxs-lookup"><span data-stu-id="4abf7-107">Methods</span></span>

| <span data-ttu-id="4abf7-108">方法</span><span class="sxs-lookup"><span data-stu-id="4abf7-108">Method</span></span>       | <span data-ttu-id="4abf7-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="4abf7-109">Return Type</span></span> | <span data-ttu-id="4abf7-110">说明</span><span class="sxs-lookup"><span data-stu-id="4abf7-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="4abf7-111">列出 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-111">List authenticationContextClassReference</span></span>](../api/conditionalaccessroot-list-authenticationcontextclassreferences.md) | <span data-ttu-id="4abf7-112">[authenticationContextClassReference](authenticationContextClassReference.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4abf7-112">[authenticationContextClassReference](authenticationContextClassReference.md) collection</span></span> | <span data-ttu-id="4abf7-113">获取组织的所有 authenticationContextClassReference 对象。</span><span class="sxs-lookup"><span data-stu-id="4abf7-113">Get all of the authenticationContextClassReference objects in the organization.</span></span> |
| [<span data-ttu-id="4abf7-114">创建 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-114">Create authenticationContextClassReference</span></span>](../api/conditionalaccessroot-post-authenticationcontextclassreferences.md) | [<span data-ttu-id="4abf7-115">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-115">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="4abf7-116">创建新的 authenticationContextClassReference 对象。</span><span class="sxs-lookup"><span data-stu-id="4abf7-116">Create a new authenticationContextClassReference object.</span></span> |
| [<span data-ttu-id="4abf7-117">获取 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-117">Get authenticationContextClassReference</span></span>](../api/authenticationcontextclassreference-get.md) | [<span data-ttu-id="4abf7-118">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-118">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="4abf7-119">读取 authenticationContextClassReference 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4abf7-119">Read properties and relationships of a authenticationContextClassReference object.</span></span> |
| [<span data-ttu-id="4abf7-120">更新 authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-120">Update authenticationContextClassReference</span></span>](../api/authenticationcontextclassreference-update.md) | [<span data-ttu-id="4abf7-121">authenticationContextClassReference</span><span class="sxs-lookup"><span data-stu-id="4abf7-121">authenticationContextClassReference</span></span>](authenticationContextClassReference.md) | <span data-ttu-id="4abf7-122">更新 authenticationContextClassReference 对象。</span><span class="sxs-lookup"><span data-stu-id="4abf7-122">Update a authenticationContextClassReference object.</span></span> |


## <a name="properties"></a><span data-ttu-id="4abf7-123">属性</span><span class="sxs-lookup"><span data-stu-id="4abf7-123">Properties</span></span>

| <span data-ttu-id="4abf7-124">属性</span><span class="sxs-lookup"><span data-stu-id="4abf7-124">Property</span></span>     | <span data-ttu-id="4abf7-125">类型</span><span class="sxs-lookup"><span data-stu-id="4abf7-125">Type</span></span>        | <span data-ttu-id="4abf7-126">说明</span><span class="sxs-lookup"><span data-stu-id="4abf7-126">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="4abf7-127">id</span><span class="sxs-lookup"><span data-stu-id="4abf7-127">id</span></span>|<span data-ttu-id="4abf7-128">String</span><span class="sxs-lookup"><span data-stu-id="4abf7-128">String</span></span>| <span data-ttu-id="4abf7-129">用于引用身份验证上下文类的标识符。</span><span class="sxs-lookup"><span data-stu-id="4abf7-129">Identifier used to reference the authentication context class.</span></span> <span data-ttu-id="4abf7-130">id 用于触发引用的身份验证要求的逐步身份验证，它是将在 acrs 声明中发出的值。</span><span class="sxs-lookup"><span data-stu-id="4abf7-130">The id is used to trigger step-up authentication for the referenced authentication requirements and is the value that will be issued in the acrs claim.</span></span> <span data-ttu-id="4abf7-131">声明中的此值用于验证是否满足所需的身份验证上下文。</span><span class="sxs-lookup"><span data-stu-id="4abf7-131">This value in the claim is used to verify the required authentication context has been satisfied.</span></span> <span data-ttu-id="4abf7-132">允许的 id 值为"c1"到"c25"。</span><span class="sxs-lookup"><span data-stu-id="4abf7-132">The allowed id values are "c1" through "c25".</span></span> |
|<span data-ttu-id="4abf7-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4abf7-133">displayName</span></span>|<span data-ttu-id="4abf7-134">String</span><span class="sxs-lookup"><span data-stu-id="4abf7-134">String</span></span>| <span data-ttu-id="4abf7-135">the 显示名称 is the friendly name of the authenticationContextClassReference.</span><span class="sxs-lookup"><span data-stu-id="4abf7-135">The display name is the friendly name of the authenticationContextClassReference.</span></span> <span data-ttu-id="4abf7-136">此值应该用于在构建面向用户的管理员体验时标识身份验证上下文类引用。</span><span class="sxs-lookup"><span data-stu-id="4abf7-136">This value should be used to identify the authentication context class reference when building user facing admin experiences.</span></span> <span data-ttu-id="4abf7-137">例如，选择 UX。</span><span class="sxs-lookup"><span data-stu-id="4abf7-137">For example, selection UX.</span></span> |
|<span data-ttu-id="4abf7-138">说明</span><span class="sxs-lookup"><span data-stu-id="4abf7-138">description</span></span>|<span data-ttu-id="4abf7-139">String</span><span class="sxs-lookup"><span data-stu-id="4abf7-139">String</span></span>| <span data-ttu-id="4abf7-140">authenticationContextClassReference 强制执行的策略的简短说明。</span><span class="sxs-lookup"><span data-stu-id="4abf7-140">A short explanation of the policies that are enforced by authenticationContextClassReference.</span></span> <span data-ttu-id="4abf7-141">此值应该用于提供辅助文本，以在构建面向用户的管理员体验时描述身份验证上下文类引用。</span><span class="sxs-lookup"><span data-stu-id="4abf7-141">This value should be used to provide secondary text to describe the authentication context class reference when building user facing admin experiences.</span></span> <span data-ttu-id="4abf7-142">例如，选择 UX。</span><span class="sxs-lookup"><span data-stu-id="4abf7-142">For example, selection UX.</span></span>|
|<span data-ttu-id="4abf7-143">isAvailable</span><span class="sxs-lookup"><span data-stu-id="4abf7-143">isAvailable</span></span>|<span data-ttu-id="4abf7-144">boolean</span><span class="sxs-lookup"><span data-stu-id="4abf7-144">boolean</span></span>| <span data-ttu-id="4abf7-145">指示 authenticationContextClassReference 是否已由安全管理员发布，并可供应用使用。</span><span class="sxs-lookup"><span data-stu-id="4abf7-145">Indicates whether the authenticationContextClassReference has been published by the security admin and is ready for use by apps.</span></span> <span data-ttu-id="4abf7-146">如果设置为 ，则不应在管理员 UX 体验中显示该值，因为该值 `false` 当前不能用于选择。</span><span class="sxs-lookup"><span data-stu-id="4abf7-146">When it is set to `false` it should not be shown in admin UX experiences because the value is not currently available for selection.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4abf7-147">关系</span><span class="sxs-lookup"><span data-stu-id="4abf7-147">Relationships</span></span>

<span data-ttu-id="4abf7-148">无。</span><span class="sxs-lookup"><span data-stu-id="4abf7-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="4abf7-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4abf7-149">JSON representation</span></span>

<span data-ttu-id="4abf7-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4abf7-150">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "displayName",
    "description",
    "sessionControls",
    "grantControls"
  ],
  "@odata.type": "microsoft.graph.authenticationContextClassReference",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id"
}-->

```json
    {
      "id": "String",
      "displayName": "String",
      "description": "String",
      "isAvailable": "boolean",
    }

```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "authenticationContextClassReference resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
