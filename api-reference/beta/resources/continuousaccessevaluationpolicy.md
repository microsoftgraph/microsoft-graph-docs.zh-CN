---
title: continuousAccessEvaluationPolicy 资源类型
description: 连续访问评估 (CAE) 有助于实时管理身份验证会话。 CAE 允许客户通过支持即时吊销事件来处理对资源的访问。
author: jerrysai
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 6a3027dea9a6c264b7af0ab805253946ebda8c97
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48023489"
---
# <a name="continuousaccessevaluationpolicy-resource-type"></a><span data-ttu-id="8c94b-104">continuousAccessEvaluationPolicy 资源类型</span><span class="sxs-lookup"><span data-stu-id="8c94b-104">continuousAccessEvaluationPolicy resource type</span></span>

<span data-ttu-id="8c94b-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c94b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c94b-106">连续访问评估 (CAE) 实时管理身份验证会话。</span><span class="sxs-lookup"><span data-stu-id="8c94b-106">Continuous Access Evaluation (CAE) manages authentication sessions in real time.</span></span> <span data-ttu-id="8c94b-107">CAE 允许客户通过支持即时吊销事件来处理对资源的访问。</span><span class="sxs-lookup"><span data-stu-id="8c94b-107">CAE allows customers to handle access to resources by supporting instant revocation events.</span></span>  <span data-ttu-id="8c94b-108">有关详细信息，请参阅 [连续访问评估](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation)。</span><span class="sxs-lookup"><span data-stu-id="8c94b-108">For more information, see the [Continuous access evaluation](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-continuous-access-evaluation).</span></span>

## <a name="methods"></a><span data-ttu-id="8c94b-109">方法</span><span class="sxs-lookup"><span data-stu-id="8c94b-109">Methods</span></span>
|<span data-ttu-id="8c94b-110">方法</span><span class="sxs-lookup"><span data-stu-id="8c94b-110">Method</span></span>|<span data-ttu-id="8c94b-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="8c94b-111">Return type</span></span>|<span data-ttu-id="8c94b-112">说明</span><span class="sxs-lookup"><span data-stu-id="8c94b-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8c94b-113">获取 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="8c94b-113">Get continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-get.md)|[<span data-ttu-id="8c94b-114">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="8c94b-114">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="8c94b-115">读取 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c94b-115">Read the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|[<span data-ttu-id="8c94b-116">更新 continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="8c94b-116">Update continuousAccessEvaluationPolicy</span></span>](../api/continuousaccessevaluationpolicy-update.md)|[<span data-ttu-id="8c94b-117">continuousAccessEvaluationPolicy</span><span class="sxs-lookup"><span data-stu-id="8c94b-117">continuousAccessEvaluationPolicy</span></span>](../resources/continuousaccessevaluationpolicy.md)|<span data-ttu-id="8c94b-118">更新 [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="8c94b-118">Update the properties of a [continuousAccessEvaluationPolicy](../resources/continuousaccessevaluationpolicy.md) object.</span></span>|
|
## <a name="properties"></a><span data-ttu-id="8c94b-119">属性</span><span class="sxs-lookup"><span data-stu-id="8c94b-119">Properties</span></span>
|<span data-ttu-id="8c94b-120">属性</span><span class="sxs-lookup"><span data-stu-id="8c94b-120">Property</span></span>|<span data-ttu-id="8c94b-121">类型</span><span class="sxs-lookup"><span data-stu-id="8c94b-121">Type</span></span>|<span data-ttu-id="8c94b-122">说明</span><span class="sxs-lookup"><span data-stu-id="8c94b-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8c94b-123">说明</span><span class="sxs-lookup"><span data-stu-id="8c94b-123">description</span></span>|<span data-ttu-id="8c94b-124">String</span><span class="sxs-lookup"><span data-stu-id="8c94b-124">String</span></span>|<span data-ttu-id="8c94b-125">连续访问评估会在用户的访问被删除或客户端 IP 地址更改时，自动阻止对资源和应用程序的即时访问。</span><span class="sxs-lookup"><span data-stu-id="8c94b-125">Continuous access evaluation automatically blocks access to resources and applications in near real time when a user's access is removed or a client IP address changes.</span></span> <span data-ttu-id="8c94b-126">只读。</span><span class="sxs-lookup"><span data-stu-id="8c94b-126">Read-only.</span></span>|
|<span data-ttu-id="8c94b-127">displayName</span><span class="sxs-lookup"><span data-stu-id="8c94b-127">displayName</span></span>|<span data-ttu-id="8c94b-128">String</span><span class="sxs-lookup"><span data-stu-id="8c94b-128">String</span></span>| <span data-ttu-id="8c94b-129">值始终为 "连续访问评估"。</span><span class="sxs-lookup"><span data-stu-id="8c94b-129">The value is always 'Continuous Access Evaluation'.</span></span> <span data-ttu-id="8c94b-130">只读。</span><span class="sxs-lookup"><span data-stu-id="8c94b-130">Read-only.</span></span>|
|<span data-ttu-id="8c94b-131">groups</span><span class="sxs-lookup"><span data-stu-id="8c94b-131">groups</span></span>|<span data-ttu-id="8c94b-132">String 集合</span><span class="sxs-lookup"><span data-stu-id="8c94b-132">String collection</span></span>|<span data-ttu-id="8c94b-133">用于评估的范围内的组标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="8c94b-133">The collection of group identifiers in scope for evaluation.</span></span> <span data-ttu-id="8c94b-134">当集合为空时，所有组都在范围内。</span><span class="sxs-lookup"><span data-stu-id="8c94b-134">All groups are in scope when the collection is empty.</span></span>|
|<span data-ttu-id="8c94b-135">id</span><span class="sxs-lookup"><span data-stu-id="8c94b-135">id</span></span>|<span data-ttu-id="8c94b-136">String</span><span class="sxs-lookup"><span data-stu-id="8c94b-136">String</span></span>|<span data-ttu-id="8c94b-137">指定 continuousAccessEvaluationPolicy 对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="8c94b-137">Specifies the identifier of a continuousAccessEvaluationPolicy object.</span></span> <span data-ttu-id="8c94b-138">只读。</span><span class="sxs-lookup"><span data-stu-id="8c94b-138">Read-only.</span></span>|
|<span data-ttu-id="8c94b-139">isEnabled</span><span class="sxs-lookup"><span data-stu-id="8c94b-139">isEnabled</span></span>|<span data-ttu-id="8c94b-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="8c94b-140">Boolean</span></span>| <span data-ttu-id="8c94b-141">`true` 以指示是否应执行连续访问评估;否则为 `false` 。</span><span class="sxs-lookup"><span data-stu-id="8c94b-141">`true` to indicate whether continuous access evaluation should be performed; otherwise `false`.</span></span> |
|<span data-ttu-id="8c94b-142">users</span><span class="sxs-lookup"><span data-stu-id="8c94b-142">users</span></span>|<span data-ttu-id="8c94b-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="8c94b-143">String collection</span></span>|<span data-ttu-id="8c94b-144">评估范围内的用户标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="8c94b-144">The collection of user identifiers in scope for evaluation.</span></span> <span data-ttu-id="8c94b-145">当集合为空时，所有用户都在范围内。</span><span class="sxs-lookup"><span data-stu-id="8c94b-145">All users are in scope when the collection is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8c94b-146">关系</span><span class="sxs-lookup"><span data-stu-id="8c94b-146">Relationships</span></span>
<span data-ttu-id="8c94b-147">无。</span><span class="sxs-lookup"><span data-stu-id="8c94b-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8c94b-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8c94b-148">JSON representation</span></span>
<span data-ttu-id="8c94b-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8c94b-149">The following is a JSON representation of the resource.</span></span>
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
