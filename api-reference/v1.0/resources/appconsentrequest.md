---
title: appConsentRequest 资源类型
description: 一个代表特定应用程序的 userConsentRequest 对象集合的请求。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 32744ce01f871c82a52710502e7fdc899537cef5
ms.sourcegitcommit: ad1e4d758d4fe6025987c1c3528ce644edb27062
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/13/2021
ms.locfileid: "51698011"
---
# <a name="appconsentrequest-resource-type"></a><span data-ttu-id="4429c-103">appConsentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="4429c-103">appConsentRequest resource type</span></span>

<span data-ttu-id="4429c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4429c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4429c-105">特定应用程序的 [userConsentRequest](../resources/userconsentrequest.md) 对象的集合。</span><span class="sxs-lookup"><span data-stu-id="4429c-105">A collection of [userConsentRequest](../resources/userconsentrequest.md) objects for a specific application.</span></span>

## <a name="methods"></a><span data-ttu-id="4429c-106">方法</span><span class="sxs-lookup"><span data-stu-id="4429c-106">Methods</span></span>

|<span data-ttu-id="4429c-107">方法</span><span class="sxs-lookup"><span data-stu-id="4429c-107">Method</span></span>|<span data-ttu-id="4429c-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="4429c-108">Return type</span></span>|<span data-ttu-id="4429c-109">说明</span><span class="sxs-lookup"><span data-stu-id="4429c-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4429c-110">列出 appConsentRequests</span><span class="sxs-lookup"><span data-stu-id="4429c-110">List appConsentRequests</span></span>](../api/appconsentrequest-list.md)|<span data-ttu-id="4429c-111">[appConsentRequest](../resources/appconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4429c-111">[appConsentRequest](../resources/appconsentrequest.md) collection</span></span>|<span data-ttu-id="4429c-112">检索 [appConsentRequest](appconsentrequest.md) 对象及其属性的集合。</span><span class="sxs-lookup"><span data-stu-id="4429c-112">Retrieve a collection of [appConsentRequest](appconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="4429c-113">获取 appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="4429c-113">Get appConsentRequest</span></span>](../api/appconsentrequest-get.md)|[<span data-ttu-id="4429c-114">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="4429c-114">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="4429c-115">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4429c-115">Read the properties and relationships of an [appConsentRequest](../resources/appconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="4429c-116">filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="4429c-116">filterByCurrentUser</span></span>](../api/appconsentrequest-filterByCurrentUser.md)|[<span data-ttu-id="4429c-117">appConsentRequest</span><span class="sxs-lookup"><span data-stu-id="4429c-117">appConsentRequest</span></span>](../resources/appconsentrequest.md)|<span data-ttu-id="4429c-118">读取 [appConsentRequest](../resources/appconsentrequest.md) 对象的属性，当前用户是这些对象的审阅者，并且用户同意请求的状态为 `InProgress` 。</span><span class="sxs-lookup"><span data-stu-id="4429c-118">Read the properties of [appConsentRequest](../resources/appconsentrequest.md) objects for which the current user is the reviewer and the status of the user consent request is `InProgress`.</span></span> |

## <a name="properties"></a><span data-ttu-id="4429c-119">属性</span><span class="sxs-lookup"><span data-stu-id="4429c-119">Properties</span></span>

|<span data-ttu-id="4429c-120">属性</span><span class="sxs-lookup"><span data-stu-id="4429c-120">Property</span></span>|<span data-ttu-id="4429c-121">类型</span><span class="sxs-lookup"><span data-stu-id="4429c-121">Type</span></span>|<span data-ttu-id="4429c-122">说明</span><span class="sxs-lookup"><span data-stu-id="4429c-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4429c-123">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="4429c-123">appDisplayName</span></span>|<span data-ttu-id="4429c-124">String</span><span class="sxs-lookup"><span data-stu-id="4429c-124">String</span></span>|<span data-ttu-id="4429c-125">请求显示名称的应用的一部分。</span><span class="sxs-lookup"><span data-stu-id="4429c-125">The display name of the app for which consent is requested.</span></span> <span data-ttu-id="4429c-126">必填。</span><span class="sxs-lookup"><span data-stu-id="4429c-126">Required.</span></span> <span data-ttu-id="4429c-127">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="4429c-127">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="4429c-128">appId</span><span class="sxs-lookup"><span data-stu-id="4429c-128">appId</span></span>|<span data-ttu-id="4429c-129">String</span><span class="sxs-lookup"><span data-stu-id="4429c-129">String</span></span>|<span data-ttu-id="4429c-130">应用程序的标识符。</span><span class="sxs-lookup"><span data-stu-id="4429c-130">The identifier of the application.</span></span> <span data-ttu-id="4429c-131">必填。</span><span class="sxs-lookup"><span data-stu-id="4429c-131">Required.</span></span> <span data-ttu-id="4429c-132">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="4429c-132">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |
|<span data-ttu-id="4429c-133">id</span><span class="sxs-lookup"><span data-stu-id="4429c-133">id</span></span>|<span data-ttu-id="4429c-134">String</span><span class="sxs-lookup"><span data-stu-id="4429c-134">String</span></span>|<span data-ttu-id="4429c-135">应用同意请求的标识符。</span><span class="sxs-lookup"><span data-stu-id="4429c-135">The identifier of the app consent request.</span></span> <span data-ttu-id="4429c-136">必填。</span><span class="sxs-lookup"><span data-stu-id="4429c-136">Required.</span></span>|
|<span data-ttu-id="4429c-137">pendingScopes</span><span class="sxs-lookup"><span data-stu-id="4429c-137">pendingScopes</span></span>|<span data-ttu-id="4429c-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4429c-138">[appConsentRequestScope](../resources/appconsentrequestscope.md) collection</span></span>|<span data-ttu-id="4429c-139">等待审批的挂起范围列表。</span><span class="sxs-lookup"><span data-stu-id="4429c-139">A list of pending scopes waiting for approval.</span></span> <span data-ttu-id="4429c-140">必填。</span><span class="sxs-lookup"><span data-stu-id="4429c-140">Required.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4429c-141">关系</span><span class="sxs-lookup"><span data-stu-id="4429c-141">Relationships</span></span>

|<span data-ttu-id="4429c-142">关系</span><span class="sxs-lookup"><span data-stu-id="4429c-142">Relationship</span></span>|<span data-ttu-id="4429c-143">类型</span><span class="sxs-lookup"><span data-stu-id="4429c-143">Type</span></span>|<span data-ttu-id="4429c-144">说明</span><span class="sxs-lookup"><span data-stu-id="4429c-144">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4429c-145">userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="4429c-145">userConsentRequests</span></span>|<span data-ttu-id="4429c-146">[userConsentRequest](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4429c-146">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="4429c-147">挂起的用户同意请求列表。</span><span class="sxs-lookup"><span data-stu-id="4429c-147">A list of pending user consent requests.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4429c-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4429c-148">JSON representation</span></span>

<span data-ttu-id="4429c-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4429c-149">The following is a JSON representation of the resource.</span></span>
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
