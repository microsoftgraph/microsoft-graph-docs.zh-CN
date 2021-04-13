---
title: appConsentRequest 资源类型
description: 一个代表特定应用程序的 userConsentRequest 对象集合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d9c01fd4e752bca0fe9518553f52312e523da3a3
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51697899"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="a6b63-103">appConsentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="a6b63-103">appConsentRequest resource type</span></span>

<span data-ttu-id="a6b63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6b63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6b63-105">特定应用程序的 [userConsentRequest](../resources/userconsentrequest.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="a6b63-105">A collection of [userConsentRequest](../resources/userconsentrequest.md) objects for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="a6b63-106">方法</span><span class="sxs-lookup"><span data-stu-id="a6b63-106">Methods</span></span>
|<span data-ttu-id="a6b63-107">方法</span><span class="sxs-lookup"><span data-stu-id="a6b63-107">Method</span></span>|<span data-ttu-id="a6b63-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="a6b63-108">Return type</span></span>|<span data-ttu-id="a6b63-109">说明</span><span class="sxs-lookup"><span data-stu-id="a6b63-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a6b63-110">列出 appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="a6b63-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="a6b63-111">[appConsentRequest](../resources/appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b63-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="a6b63-112">检索 [appConsentRequest](appconsentrequest.md) 对象及其属性的集合。</span><span class="sxs-lookup"><span data-stu-id="a6b63-112">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="a6b63-113">获取 appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="a6b63-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="a6b63-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="a6b63-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="a6b63-115">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a6b63-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="a6b63-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="a6b63-116">filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="a6b63-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="a6b63-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="a6b63-118">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性，当前用户是这些对象的审阅者，并且用户同意请求的状态为 `InProgress` 。</span><span class="sxs-lookup"><span data-stu-id="a6b63-118">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a6b63-119">属性</span><span class="sxs-lookup"><span data-stu-id="a6b63-119">Properties</span></span>
|<span data-ttu-id="a6b63-120">属性</span><span class="sxs-lookup"><span data-stu-id="a6b63-120">Property</span></span>|<span data-ttu-id="a6b63-121">类型</span><span class="sxs-lookup"><span data-stu-id="a6b63-121">Type</span></span>|<span data-ttu-id="a6b63-122">说明</span><span class="sxs-lookup"><span data-stu-id="a6b63-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b63-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="a6b63-123">appDisplayName</span></span>|<span data-ttu-id="a6b63-124">String</span><span class="sxs-lookup"><span data-stu-id="a6b63-124">String</span></span>|<span data-ttu-id="a6b63-125">请求显示名称的应用的一部分。</span><span class="sxs-lookup"><span data-stu-id="a6b63-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="a6b63-126">必填。</span><span class="sxs-lookup"><span data-stu-id="a6b63-126">Required.</span></span> <span data-ttu-id="a6b63-127">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="a6b63-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="a6b63-128">appId</span><span class="sxs-lookup"><span data-stu-id="a6b63-128">appId</span></span>|<span data-ttu-id="a6b63-129">String</span><span class="sxs-lookup"><span data-stu-id="a6b63-129">String</span></span>|<span data-ttu-id="a6b63-130">应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b63-130">The identifier of the application.</span></span> <span data-ttu-id="a6b63-131">必填。</span><span class="sxs-lookup"><span data-stu-id="a6b63-131">Required.</span></span> <span data-ttu-id="a6b63-132">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="a6b63-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="a6b63-133">consentType</span><span class="sxs-lookup"><span data-stu-id="a6b63-133">consentType</span></span>|<span data-ttu-id="a6b63-134">String</span><span class="sxs-lookup"><span data-stu-id="a6b63-134">String</span></span>|<span data-ttu-id="a6b63-135">请求的同意类型。</span><span class="sxs-lookup"><span data-stu-id="a6b63-135">The consent type of the request.</span></span> <span data-ttu-id="a6b63-136">可能的值是： `Static`   和  `Dynamic` 。</span><span class="sxs-lookup"><span data-stu-id="a6b63-136">Possible values are: `Static` and `Dynamic`.</span></span> <span data-ttu-id="a6b63-137">它们分别表示在同意工作流中请求的静态和动态权限。</span><span class="sxs-lookup"><span data-stu-id="a6b63-137">These represent static and dynamic permissions, respectively, requested in the consent workflow.</span></span> <span data-ttu-id="a6b63-138">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="a6b63-138">Supports `$filter` (`eq` only) and `$orderby`.</span></span> <span data-ttu-id="a6b63-139">必需。</span><span class="sxs-lookup"><span data-stu-id="a6b63-139">Required.</span></span>|
|<span data-ttu-id="a6b63-140">id</span><span class="sxs-lookup"><span data-stu-id="a6b63-140">id</span></span>|<span data-ttu-id="a6b63-141">String</span><span class="sxs-lookup"><span data-stu-id="a6b63-141">String</span></span>|<span data-ttu-id="a6b63-142">应用同意请求的标识符。</span><span class="sxs-lookup"><span data-stu-id="a6b63-142">The identifier of the app consent request.</span></span> <span data-ttu-id="a6b63-143">必填。</span><span class="sxs-lookup"><span data-stu-id="a6b63-143">Required.</span></span>|
|<span data-ttu-id="a6b63-144">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="a6b63-144">pendingScopes</span></span>|<span data-ttu-id="a6b63-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b63-145">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="a6b63-146">等待审批的挂起范围列表。</span><span class="sxs-lookup"><span data-stu-id="a6b63-146">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="a6b63-147">如果 consentType 为 ，则为空 `Static` 。</span><span class="sxs-lookup"><span data-stu-id="a6b63-147">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="a6b63-148">必填。</span><span class="sxs-lookup"><span data-stu-id="a6b63-148">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a6b63-149">关系</span><span class="sxs-lookup"><span data-stu-id="a6b63-149">Relationships</span></span>
|<span data-ttu-id="a6b63-150">关系</span><span class="sxs-lookup"><span data-stu-id="a6b63-150">Relationship</span></span>|<span data-ttu-id="a6b63-151">类型</span><span class="sxs-lookup"><span data-stu-id="a6b63-151">Type</span></span>|<span data-ttu-id="a6b63-152">说明</span><span class="sxs-lookup"><span data-stu-id="a6b63-152">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6b63-153">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="a6b63-153">userConsentRequests</span></span>|<span data-ttu-id="a6b63-154">[userConsentRequest](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a6b63-154">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="a6b63-155">挂起的用户同意请求列表。</span><span class="sxs-lookup"><span data-stu-id="a6b63-155">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6b63-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a6b63-156">JSON representation</span></span>
<span data-ttu-id="a6b63-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6b63-157">The following is a JSON representation of the resource.</span></span>
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

