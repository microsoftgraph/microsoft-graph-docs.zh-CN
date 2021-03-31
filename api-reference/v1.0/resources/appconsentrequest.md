---
title: appConsentRequest 资源类型
description: 表示特定应用程序的 userConsentRequests 聚合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: ac7e9f2ea8e727a285016641bac10ea3d2e38f9b
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51469534"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="56b49-103">appConsentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="56b49-103">appConsentRequest resource type</span></span>

<span data-ttu-id="56b49-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56b49-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="56b49-105">特定应用程序的 [userConsentRequests](../resources/userconsentrequest.md) 聚合。</span><span class="sxs-lookup"><span data-stu-id="56b49-105">An aggregation of [userConsentRequests](../resources/userconsentrequest.md) for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="56b49-106">方法</span><span class="sxs-lookup"><span data-stu-id="56b49-106">Methods</span></span>

|<span data-ttu-id="56b49-107">方法</span><span class="sxs-lookup"><span data-stu-id="56b49-107">Method</span></span>|<span data-ttu-id="56b49-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="56b49-108">Return type</span></span>|<span data-ttu-id="56b49-109">说明</span><span class="sxs-lookup"><span data-stu-id="56b49-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="56b49-110">列出 appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="56b49-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="56b49-111">[appConsentRequest](../resources/appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56b49-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="56b49-112">获取 [appConsentRequest](../resources/appconsentrequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="56b49-112">Get a list of the [appConsentRequest](../resources/appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="56b49-113">获取 appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="56b49-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="56b49-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="56b49-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="56b49-115">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="56b49-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="56b49-116">appConsentRequests：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="56b49-116">appConsentRequests: filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="56b49-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="56b49-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="56b49-118">当前用户是审阅者的 [appConsentRequests](../resources/appconsentrequest.md) 的列表</span><span class="sxs-lookup"><span data-stu-id="56b49-118">A list of the [appConsentRequests](../resources/appconsentrequest.md) for which the current user is the reviewer</span></span>|

## <a name="properties"></a><span data-ttu-id="56b49-119">属性</span><span class="sxs-lookup"><span data-stu-id="56b49-119">Properties</span></span>

|<span data-ttu-id="56b49-120">属性</span><span class="sxs-lookup"><span data-stu-id="56b49-120">Property</span></span>|<span data-ttu-id="56b49-121">类型</span><span class="sxs-lookup"><span data-stu-id="56b49-121">Type</span></span>|<span data-ttu-id="56b49-122">说明</span><span class="sxs-lookup"><span data-stu-id="56b49-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56b49-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="56b49-123">appDisplayName</span></span>|<span data-ttu-id="56b49-124">String</span><span class="sxs-lookup"><span data-stu-id="56b49-124">String</span></span>|<span data-ttu-id="56b49-125">请求显示名称的应用的一部分。</span><span class="sxs-lookup"><span data-stu-id="56b49-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="56b49-126">必需。</span><span class="sxs-lookup"><span data-stu-id="56b49-126">Required.</span></span> <span data-ttu-id="56b49-127">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="56b49-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="56b49-128">appId</span><span class="sxs-lookup"><span data-stu-id="56b49-128">appId</span></span>|<span data-ttu-id="56b49-129">String</span><span class="sxs-lookup"><span data-stu-id="56b49-129">String</span></span>|<span data-ttu-id="56b49-130">应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="56b49-130">The identifier of the application.</span></span> <span data-ttu-id="56b49-131">必需。</span><span class="sxs-lookup"><span data-stu-id="56b49-131">Required.</span></span> <span data-ttu-id="56b49-132">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="56b49-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="56b49-133">id</span><span class="sxs-lookup"><span data-stu-id="56b49-133">id</span></span>|<span data-ttu-id="56b49-134">String</span><span class="sxs-lookup"><span data-stu-id="56b49-134">String</span></span>|<span data-ttu-id="56b49-135">应用同意请求的标识符。</span><span class="sxs-lookup"><span data-stu-id="56b49-135">The identifier of the app consent request.</span></span> <span data-ttu-id="56b49-136">必需。</span><span class="sxs-lookup"><span data-stu-id="56b49-136">Required.</span></span>|
|<span data-ttu-id="56b49-137">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="56b49-137">pendingScopes</span></span>|<span data-ttu-id="56b49-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56b49-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="56b49-139">等待审批的挂起范围列表。</span><span class="sxs-lookup"><span data-stu-id="56b49-139">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="56b49-140">如果 consentType 为 ，则为空 `Static` 。</span><span class="sxs-lookup"><span data-stu-id="56b49-140">This is empty if the consentType is `Static`.</span></span> <span data-ttu-id="56b49-141">必填。</span><span class="sxs-lookup"><span data-stu-id="56b49-141">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56b49-142">关系</span><span class="sxs-lookup"><span data-stu-id="56b49-142">Relationships</span></span>

|<span data-ttu-id="56b49-143">关系</span><span class="sxs-lookup"><span data-stu-id="56b49-143">Relationship</span></span>|<span data-ttu-id="56b49-144">类型</span><span class="sxs-lookup"><span data-stu-id="56b49-144">Type</span></span>|<span data-ttu-id="56b49-145">说明</span><span class="sxs-lookup"><span data-stu-id="56b49-145">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56b49-146">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="56b49-146">userConsentRequests</span></span>|<span data-ttu-id="56b49-147">[userConsentRequest](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="56b49-147">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="56b49-148">挂起的用户同意请求列表。</span><span class="sxs-lookup"><span data-stu-id="56b49-148">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="56b49-149">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56b49-149">JSON representation</span></span>

<span data-ttu-id="56b49-150">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56b49-150">The following is a JSON representation of the resource.</span></span>
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
  "pendingScopes": [
    {
      "@odata.type": "microsoft.graph.appConsentRequestScope"
    }
  ]
}
```
