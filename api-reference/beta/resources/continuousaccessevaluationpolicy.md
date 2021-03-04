---
title: continuousAccessEvaluationPolicy 资源类型
description: CAE (连续访问) 有助于实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问权限。
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 58c4f913c8a5fc3b4f7c1c129c7126437035cbe7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50444262"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="03acc-104">continuousAccessEvaluationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="03acc-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="03acc-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03acc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="03acc-106">CAE (连续) 实时管理身份验证会话。</span><span class="sxs-lookup"><span data-stu-id="03acc-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="03acc-107">CAE 允许客户通过支持即时吊销事件来处理对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="03acc-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="03acc-108">有关详细信息，请参阅连续 [访问评估](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)。</span><span class="sxs-lookup"><span data-stu-id="03acc-108">For more information, see the [Continuous access evaluation](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="03acc-109">Methods</span><span class="sxs-lookup"><span data-stu-id="03acc-109">Methods</span></span>
|<span data-ttu-id="03acc-110">方法</span><span class="sxs-lookup"><span data-stu-id="03acc-110">Method</span></span>|<span data-ttu-id="03acc-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="03acc-111">Return type</span></span>|<span data-ttu-id="03acc-112">说明</span><span class="sxs-lookup"><span data-stu-id="03acc-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="03acc-113">获取 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="03acc-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="03acc-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="03acc-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="03acc-115">读取 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="03acc-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="03acc-116">更新 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="03acc-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="03acc-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="03acc-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="03acc-118">更新 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="03acc-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="03acc-119">属性</span><span class="sxs-lookup"><span data-stu-id="03acc-119">Properties</span></span>
|<span data-ttu-id="03acc-120">属性</span><span class="sxs-lookup"><span data-stu-id="03acc-120">Property</span></span>|<span data-ttu-id="03acc-121">类型</span><span class="sxs-lookup"><span data-stu-id="03acc-121">Type</span></span>|<span data-ttu-id="03acc-122">说明</span><span class="sxs-lookup"><span data-stu-id="03acc-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03acc-123">说明</span><span class="sxs-lookup"><span data-stu-id="03acc-123">description</span></span>|<span data-ttu-id="03acc-124">String</span><span class="sxs-lookup"><span data-stu-id="03acc-124">String</span></span>|<span data-ttu-id="03acc-125">当删除用户访问或客户端 IP 地址更改时，连续访问评估会自动阻止对资源和应用程序的近实时访问。</span><span class="sxs-lookup"><span data-stu-id="03acc-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="03acc-126">只读。</span><span class="sxs-lookup"><span data-stu-id="03acc-126">Read-only.</span></span>|
|<span data-ttu-id="03acc-127">displayName</span><span class="sxs-lookup"><span data-stu-id="03acc-127">displayName</span></span>|<span data-ttu-id="03acc-128">String</span><span class="sxs-lookup"><span data-stu-id="03acc-128">String</span></span>| <span data-ttu-id="03acc-129">该值始终为"连续访问评估"。</span><span class="sxs-lookup"><span data-stu-id="03acc-129">The value is always 'Continuous Access Evaluation'.</span></span> <span data-ttu-id="03acc-130">只读。</span><span class="sxs-lookup"><span data-stu-id="03acc-130">Read-only.</span></span>|
|<span data-ttu-id="03acc-131">groups</span><span class="sxs-lookup"><span data-stu-id="03acc-131">groups</span></span>|<span data-ttu-id="03acc-132">字符串集合</span><span class="sxs-lookup"><span data-stu-id="03acc-132">String collection</span></span>|<span data-ttu-id="03acc-133">评估范围内组标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="03acc-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="03acc-134">当集合为空时，所有组都位于范围内。</span><span class="sxs-lookup"><span data-stu-id="03acc-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="03acc-135">id</span><span class="sxs-lookup"><span data-stu-id="03acc-135">id</span></span>|<span data-ttu-id="03acc-136">String</span><span class="sxs-lookup"><span data-stu-id="03acc-136">String</span></span>|<span data-ttu-id="03acc-137">指定 continuousAccessEvaluationPolicy 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="03acc-137">Specifies the identifier of a continuousAccessEvaluationPolicy object.</span></span> <span data-ttu-id="03acc-138">只读。</span><span class="sxs-lookup"><span data-stu-id="03acc-138">Read-only.</span></span>|
|<span data-ttu-id="03acc-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="03acc-139">isEnabled</span></span>|<span data-ttu-id="03acc-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="03acc-140">Boolean</span></span>| <span data-ttu-id="03acc-141">`true` 指示是否应该执行连续访问评估;否则 `false` 。</span><span class="sxs-lookup"><span data-stu-id="03acc-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="03acc-142">users</span><span class="sxs-lookup"><span data-stu-id="03acc-142">users</span></span>|<span data-ttu-id="03acc-143">字符串集合</span><span class="sxs-lookup"><span data-stu-id="03acc-143">String collection</span></span>|<span data-ttu-id="03acc-144">评估范围内用户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="03acc-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="03acc-145">当集合为空时，所有用户都位于范围内。</span><span class="sxs-lookup"><span data-stu-id="03acc-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="03acc-146">关系</span><span class="sxs-lookup"><span data-stu-id="03acc-146">Relationships</span></span>
<span data-ttu-id="03acc-147">无。</span><span class="sxs-lookup"><span data-stu-id="03acc-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="03acc-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="03acc-148">JSON representation</span></span>
<span data-ttu-id="03acc-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03acc-149">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.continuousAccessEvaluationPolicy",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.continuousAccessEvaluationPolicy",
  "id": "String (identifier)",
  "description": "String",
  "displayName": "String",
  "isEnabled": "Boolean",
  "users": [
    "String"
  ],
  "groups": [
    "String"
  ]
}
```
