---
title: continuousAccessEvaluationPolicy 资源类型
description: CAE (连续访问) 有助于实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问权限。
author: jerrysai
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: f34fdacf75b991ff339f4b7cdd823290438e8fea
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50962635"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="69071-104">continuousAccessEvaluationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="69071-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="69071-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="69071-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="69071-106">CAE (持续访问) 实时管理身份验证会话。</span><span class="sxs-lookup"><span data-stu-id="69071-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="69071-107">CAE 允许客户通过支持即时吊销事件来处理对资源的访问权限。</span><span class="sxs-lookup"><span data-stu-id="69071-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="69071-108">有关详细信息，请参阅连续 [访问评估](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)。</span><span class="sxs-lookup"><span data-stu-id="69071-108">For more information, see the [Continuous access evaluation](/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="69071-109">Methods</span><span class="sxs-lookup"><span data-stu-id="69071-109">Methods</span></span>
|<span data-ttu-id="69071-110">方法</span><span class="sxs-lookup"><span data-stu-id="69071-110">Method</span></span>|<span data-ttu-id="69071-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="69071-111">Return type</span></span>|<span data-ttu-id="69071-112">说明</span><span class="sxs-lookup"><span data-stu-id="69071-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="69071-113">获取 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="69071-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="69071-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="69071-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="69071-115">读取 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="69071-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="69071-116">更新 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="69071-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="69071-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="69071-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="69071-118">更新 [continuousAccessEvaluationPolicy 对象](../resources/continuousaccessevaluationpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="69071-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="69071-119">属性</span><span class="sxs-lookup"><span data-stu-id="69071-119">Properties</span></span>
|<span data-ttu-id="69071-120">属性</span><span class="sxs-lookup"><span data-stu-id="69071-120">Property</span></span>|<span data-ttu-id="69071-121">类型</span><span class="sxs-lookup"><span data-stu-id="69071-121">Type</span></span>|<span data-ttu-id="69071-122">说明</span><span class="sxs-lookup"><span data-stu-id="69071-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69071-123">说明</span><span class="sxs-lookup"><span data-stu-id="69071-123">description</span></span>|<span data-ttu-id="69071-124">String</span><span class="sxs-lookup"><span data-stu-id="69071-124">String</span></span>|<span data-ttu-id="69071-125">当用户的访问被删除或客户端 IP 地址更改时，连续访问评估将自动阻止对资源和应用程序的访问。</span><span class="sxs-lookup"><span data-stu-id="69071-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="69071-126">只读。</span><span class="sxs-lookup"><span data-stu-id="69071-126">Read-only.</span></span>|
|<span data-ttu-id="69071-127">displayName</span><span class="sxs-lookup"><span data-stu-id="69071-127">displayName</span></span>|<span data-ttu-id="69071-128">String</span><span class="sxs-lookup"><span data-stu-id="69071-128">String</span></span>| <span data-ttu-id="69071-129">该值始终为 `Continuous Access Evaluation` 。</span><span class="sxs-lookup"><span data-stu-id="69071-129">The value is always `Continuous Access Evaluation`.</span></span> <span data-ttu-id="69071-130">只读。</span><span class="sxs-lookup"><span data-stu-id="69071-130">Read-only.</span></span>|
|<span data-ttu-id="69071-131">groups</span><span class="sxs-lookup"><span data-stu-id="69071-131">groups</span></span>|<span data-ttu-id="69071-132">String collection</span><span class="sxs-lookup"><span data-stu-id="69071-132">String collection</span></span>|<span data-ttu-id="69071-133">作用域中用于评估的组标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="69071-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="69071-134">当集合为空时，所有组都位于范围内。</span><span class="sxs-lookup"><span data-stu-id="69071-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="69071-135">id</span><span class="sxs-lookup"><span data-stu-id="69071-135">id</span></span>|<span data-ttu-id="69071-136">String</span><span class="sxs-lookup"><span data-stu-id="69071-136">String</span></span>|<span data-ttu-id="69071-137">指定 [continuousAccessEvaluationPolicy 对象的](#continuousaccessevaluationpolicy-resource-type) 标识符。</span><span class="sxs-lookup"><span data-stu-id="69071-137">Specifies the identifier of a [continuousAccessEvaluationPolicy](#continuousaccessevaluationpolicy-resource-type) object.</span></span> <span data-ttu-id="69071-138">只读。</span><span class="sxs-lookup"><span data-stu-id="69071-138">Read-only.</span></span>|
|<span data-ttu-id="69071-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="69071-139">isEnabled</span></span>|<span data-ttu-id="69071-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="69071-140">Boolean</span></span>| <span data-ttu-id="69071-141">`true` 指示是否应该执行连续访问评估;否则 `false` 为 。</span><span class="sxs-lookup"><span data-stu-id="69071-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="69071-142">users</span><span class="sxs-lookup"><span data-stu-id="69071-142">users</span></span>|<span data-ttu-id="69071-143">String collection</span><span class="sxs-lookup"><span data-stu-id="69071-143">String collection</span></span>|<span data-ttu-id="69071-144">评估范围内用户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="69071-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="69071-145">当集合为空时，所有用户都位于范围内。</span><span class="sxs-lookup"><span data-stu-id="69071-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="69071-146">关系</span><span class="sxs-lookup"><span data-stu-id="69071-146">Relationships</span></span>
<span data-ttu-id="69071-147">无。</span><span class="sxs-lookup"><span data-stu-id="69071-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="69071-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="69071-148">JSON representation</span></span>
<span data-ttu-id="69071-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="69071-149">The following is a JSON representation of the resource.</span></span>
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
