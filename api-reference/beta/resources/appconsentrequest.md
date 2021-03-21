---
title: appConsentRequest 资源类型
description: 表示特定应用程序的 userConsentRequests 聚合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: f823f64d4c0324aeca74c3268d6fc95d313e2f00
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965115"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="2215e-103">appConsentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="2215e-103">appConsentRequest resource type</span></span>

<span data-ttu-id="2215e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2215e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2215e-105">特定应用程序的 [userConsentRequests](../resources/userconsentrequest.md) 聚合。</span><span class="sxs-lookup"><span data-stu-id="2215e-105">An aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="2215e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="2215e-106">Methods</span></span>
|<span data-ttu-id="2215e-107">方法</span><span class="sxs-lookup"><span data-stu-id="2215e-107">Method</span></span>|<span data-ttu-id="2215e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="2215e-108">Return type</span></span>|<span data-ttu-id="2215e-109">说明</span><span class="sxs-lookup"><span data-stu-id="2215e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2215e-110">列出 appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="2215e-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="2215e-111">[appConsentRequest](../resources/appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2215e-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="2215e-112">获取 [appConsentRequest](../resources/appconsentrequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="2215e-112">Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="2215e-113">获取 appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="2215e-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="2215e-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="2215e-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="2215e-115">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2215e-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="2215e-116">列出 appConsentRequests：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="2215e-116">List appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="2215e-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="2215e-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="2215e-118">当前用户是审阅者的 [appConsentRequests](../resources/appconsentrequest.md) 的列表</span><span class="sxs-lookup"><span data-stu-id="2215e-118">A list of the [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer</span></span>|

## <a name="properties"></a><span data-ttu-id="2215e-119">属性</span><span class="sxs-lookup"><span data-stu-id="2215e-119">Properties</span></span>
|<span data-ttu-id="2215e-120">属性</span><span class="sxs-lookup"><span data-stu-id="2215e-120">Property</span></span>|<span data-ttu-id="2215e-121">类型</span><span class="sxs-lookup"><span data-stu-id="2215e-121">Type</span></span>|<span data-ttu-id="2215e-122">说明</span><span class="sxs-lookup"><span data-stu-id="2215e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2215e-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2215e-123">appDisplayName</span></span>|<span data-ttu-id="2215e-124">String</span><span class="sxs-lookup"><span data-stu-id="2215e-124">String</span></span>|<span data-ttu-id="2215e-125">请求显示名称的应用的一部分。</span><span class="sxs-lookup"><span data-stu-id="2215e-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="2215e-126">必填。</span><span class="sxs-lookup"><span data-stu-id="2215e-126">Required.</span></span> <span data-ttu-id="2215e-127">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="2215e-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="2215e-128">appId</span><span class="sxs-lookup"><span data-stu-id="2215e-128">appId</span></span>|<span data-ttu-id="2215e-129">String</span><span class="sxs-lookup"><span data-stu-id="2215e-129">String</span></span>|<span data-ttu-id="2215e-130">应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="2215e-130">The identifier of the application.</span></span> <span data-ttu-id="2215e-131">必填。</span><span class="sxs-lookup"><span data-stu-id="2215e-131">Required.</span></span> <span data-ttu-id="2215e-132">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="2215e-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="2215e-133">consentType</span><span class="sxs-lookup"><span data-stu-id="2215e-133">consentType</span></span>|<span data-ttu-id="2215e-134">String</span><span class="sxs-lookup"><span data-stu-id="2215e-134">String</span></span>|<span data-ttu-id="2215e-135">请求的同意类型。</span><span class="sxs-lookup"><span data-stu-id="2215e-135">The consent type of the request.</span></span> <span data-ttu-id="2215e-136">可能的值是： `Static`   和  `Dynamic` 。</span><span class="sxs-lookup"><span data-stu-id="2215e-136">Possible values are: `Static` and `Dynamic`.</span></span> <span data-ttu-id="2215e-137">它们分别表示在同意工作流中请求的静态和动态权限。</span><span class="sxs-lookup"><span data-stu-id="2215e-137">These represent static and dynamic permissions, respectively, requested in the consent workflow.</span></span> <span data-ttu-id="2215e-138">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="2215e-138">Supports `$filter` (`eq` only) and `$orderby`.</span></span> <span data-ttu-id="2215e-139">必需。</span><span class="sxs-lookup"><span data-stu-id="2215e-139">Required.</span></span>|
|<span data-ttu-id="2215e-140">id</span><span class="sxs-lookup"><span data-stu-id="2215e-140">id</span></span>|<span data-ttu-id="2215e-141">String</span><span class="sxs-lookup"><span data-stu-id="2215e-141">String</span></span>|<span data-ttu-id="2215e-142">应用同意请求的标识符。</span><span class="sxs-lookup"><span data-stu-id="2215e-142">The identifier of the app consent request.</span></span> <span data-ttu-id="2215e-143">必填。</span><span class="sxs-lookup"><span data-stu-id="2215e-143">Required.</span></span>|
|<span data-ttu-id="2215e-144">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="2215e-144">pendingScopes</span></span>|<span data-ttu-id="2215e-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2215e-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="2215e-146">等待审批的挂起范围列表。</span><span class="sxs-lookup"><span data-stu-id="2215e-146">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="2215e-147">如果 consentType 为 ，则为空 `Static` 。</span><span class="sxs-lookup"><span data-stu-id="2215e-147">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="2215e-148">必填。</span><span class="sxs-lookup"><span data-stu-id="2215e-148">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2215e-149">关系</span><span class="sxs-lookup"><span data-stu-id="2215e-149">Relationships</span></span>
|<span data-ttu-id="2215e-150">关系</span><span class="sxs-lookup"><span data-stu-id="2215e-150">Relationship</span></span>|<span data-ttu-id="2215e-151">类型</span><span class="sxs-lookup"><span data-stu-id="2215e-151">Type</span></span>|<span data-ttu-id="2215e-152">说明</span><span class="sxs-lookup"><span data-stu-id="2215e-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2215e-153">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="2215e-153">userConsentRequests</span></span>|<span data-ttu-id="2215e-154">[userConsentRequest](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2215e-154">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="2215e-155">挂起的用户同意请求列表。</span><span class="sxs-lookup"><span data-stu-id="2215e-155">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2215e-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2215e-156">JSON representation</span></span>
<span data-ttu-id="2215e-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2215e-157">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.appConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.appConsentRequest",
  "id": "String (identifier)",
  "appId": "String",
  "appDisplayName": "String",
  "consentType": "String",
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```

