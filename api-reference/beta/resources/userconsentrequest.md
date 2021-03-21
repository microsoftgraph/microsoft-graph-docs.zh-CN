---
title: userConsentRequest 资源类型
description: 用户创建以使用需要访问组织数据的应用的请求，用户未经授权向自身授予同意。
author: psignoret
localization_priority: Normal
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: d3d91688a0a385ea319dee6df90b45c52bd4ec89
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965053"
---
# <a name="userconsentrequest-resource-type"></a><span data-ttu-id="73b2e-103">userConsentRequest 资源类型</span><span class="sxs-lookup"><span data-stu-id="73b2e-103">userConsentRequest resource type</span></span>

<span data-ttu-id="73b2e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73b2e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="73b2e-105">[userConsentRequest](../resources/userconsentrequest.md)是由用户请求访问需要管理员授权才能访问的应用程序时创建的。</span><span class="sxs-lookup"><span data-stu-id="73b2e-105">A [userConsentRequest](../resources/userconsentrequest.md) is created by an user when they are requesting access to an application which requires an admin authorization to access.</span></span> 

## <a name="methods"></a><span data-ttu-id="73b2e-106">Methods</span><span class="sxs-lookup"><span data-stu-id="73b2e-106">Methods</span></span>
|<span data-ttu-id="73b2e-107">方法</span><span class="sxs-lookup"><span data-stu-id="73b2e-107">Method</span></span>|<span data-ttu-id="73b2e-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="73b2e-108">Return type</span></span>|<span data-ttu-id="73b2e-109">说明</span><span class="sxs-lookup"><span data-stu-id="73b2e-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73b2e-110">列出 userConsentRequests</span><span class="sxs-lookup"><span data-stu-id="73b2e-110">List userConsentRequests</span></span>](../api/userconsentrequest-list.md)|<span data-ttu-id="73b2e-111">[userConsentRequest](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73b2e-111">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="73b2e-112">获取 [userConsentRequest](../resources/userconsentrequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="73b2e-112">Get a list of the [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>|
|[<span data-ttu-id="73b2e-113">获取 userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="73b2e-113">Get userConsentRequest</span></span>](../api/userconsentrequest-get.md)|[<span data-ttu-id="73b2e-114">userConsentRequest</span><span class="sxs-lookup"><span data-stu-id="73b2e-114">userConsentRequest</span></span>](../resources/userconsentrequest.md)|<span data-ttu-id="73b2e-115">读取 [userConsentRequest](../resources/userconsentrequest.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="73b2e-115">Read the properties and relationships of a [userConsentRequest](../resources/userconsentrequest.md) object.</span></span>|
|[<span data-ttu-id="73b2e-116">列出 userConsentRequests：filterByCurrentUser</span><span class="sxs-lookup"><span data-stu-id="73b2e-116">List userConsentRequests: filterByCurrentUser</span></span>](../api/userconsentrequest-filterByCurrentUser.md)|<span data-ttu-id="73b2e-117">[userConsentRequest](../resources/userconsentrequest.md) 集合</span><span class="sxs-lookup"><span data-stu-id="73b2e-117">[userConsentRequest](../resources/userconsentrequest.md) collection</span></span>|<span data-ttu-id="73b2e-118">获取 [userConsentRequest](../resources/userconsentrequest.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="73b2e-118">Get a list of the [userConsentRequest](../resources/userconsentrequest.md) objects and their properties.</span></span>|

## <a name="properties"></a><span data-ttu-id="73b2e-119">属性</span><span class="sxs-lookup"><span data-stu-id="73b2e-119">Properties</span></span>
|<span data-ttu-id="73b2e-120">属性</span><span class="sxs-lookup"><span data-stu-id="73b2e-120">Property</span></span>|<span data-ttu-id="73b2e-121">类型</span><span class="sxs-lookup"><span data-stu-id="73b2e-121">Type</span></span>|<span data-ttu-id="73b2e-122">说明</span><span class="sxs-lookup"><span data-stu-id="73b2e-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b2e-123">approvalId</span><span class="sxs-lookup"><span data-stu-id="73b2e-123">approvalId</span></span>|<span data-ttu-id="73b2e-124">String</span><span class="sxs-lookup"><span data-stu-id="73b2e-124">String</span></span>|<span data-ttu-id="73b2e-125">审批的 ID。</span><span class="sxs-lookup"><span data-stu-id="73b2e-125">The id of the approval.</span></span> <span data-ttu-id="73b2e-126">此值等于 的值 `id` 。</span><span class="sxs-lookup"><span data-stu-id="73b2e-126">This value is equal to the value of the `id`.</span></span>|
|<span data-ttu-id="73b2e-127">completedDateTime</span><span class="sxs-lookup"><span data-stu-id="73b2e-127">completedDateTime</span></span>|<span data-ttu-id="73b2e-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73b2e-128">DateTimeOffset</span></span>|<span data-ttu-id="73b2e-129">将请求状态 **标记为** 的日期和时间 `Completed` 。</span><span class="sxs-lookup"><span data-stu-id="73b2e-129">The date and time when the **status** of the request was marked as `Completed`.</span></span> <span data-ttu-id="73b2e-130">日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="73b2e-130">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73b2e-131">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="73b2e-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span>|
|<span data-ttu-id="73b2e-132">createdBy</span><span class="sxs-lookup"><span data-stu-id="73b2e-132">createdBy</span></span>|[<span data-ttu-id="73b2e-133">identitySet</span><span class="sxs-lookup"><span data-stu-id="73b2e-133">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="73b2e-134">创建请求的用户。</span><span class="sxs-lookup"><span data-stu-id="73b2e-134">The user who created the request.</span></span>|
|<span data-ttu-id="73b2e-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73b2e-135">createdDateTime</span></span>|<span data-ttu-id="73b2e-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73b2e-136">DateTimeOffset</span></span>|<span data-ttu-id="73b2e-137">创建请求的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="73b2e-137">The date and time when the request was created.</span></span> <span data-ttu-id="73b2e-138">日期和时间信息采用 ISO 8601 格式，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="73b2e-138">The date and time information uses ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="73b2e-139">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="73b2e-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="73b2e-140">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="73b2e-140">Supports `$filter` (`eq` only) and `$orderby`.</span></span>|
|<span data-ttu-id="73b2e-141">customData</span><span class="sxs-lookup"><span data-stu-id="73b2e-141">customData</span></span>|<span data-ttu-id="73b2e-142">String</span><span class="sxs-lookup"><span data-stu-id="73b2e-142">String</span></span>|<span data-ttu-id="73b2e-143">自由文本字段，用于定义用户同意请求的任何自定义数据。</span><span class="sxs-lookup"><span data-stu-id="73b2e-143">Free text field to define any custom data for the user consent request.</span></span> <span data-ttu-id="73b2e-144">未使用。</span><span class="sxs-lookup"><span data-stu-id="73b2e-144">Not used.</span></span>|
|<span data-ttu-id="73b2e-145">id</span><span class="sxs-lookup"><span data-stu-id="73b2e-145">id</span></span>|<span data-ttu-id="73b2e-146">String</span><span class="sxs-lookup"><span data-stu-id="73b2e-146">String</span></span>|<span data-ttu-id="73b2e-147">请求的标识符。</span><span class="sxs-lookup"><span data-stu-id="73b2e-147">Identifier of the request.</span></span> |
|<span data-ttu-id="73b2e-148">reason</span><span class="sxs-lookup"><span data-stu-id="73b2e-148">reason</span></span>|<span data-ttu-id="73b2e-149">String</span><span class="sxs-lookup"><span data-stu-id="73b2e-149">String</span></span>|<span data-ttu-id="73b2e-150">用户要求访问应用的理由。</span><span class="sxs-lookup"><span data-stu-id="73b2e-150">The user's justification for requiring access to the app.</span></span> <span data-ttu-id="73b2e-151">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="73b2e-151">Supports `$filter` (`eq` only) and `$orderby`.</span></span>  |
|<span data-ttu-id="73b2e-152">状态</span><span class="sxs-lookup"><span data-stu-id="73b2e-152">status</span></span>|<span data-ttu-id="73b2e-153">String</span><span class="sxs-lookup"><span data-stu-id="73b2e-153">String</span></span>|<span data-ttu-id="73b2e-154">用户的应用同意请求的状态。</span><span class="sxs-lookup"><span data-stu-id="73b2e-154">The status of the user's app consent request.</span></span> <span data-ttu-id="73b2e-155">可能的值是 `Initializing` ：、 `InProgress` 和 `Completed` 。</span><span class="sxs-lookup"><span data-stu-id="73b2e-155">Possible values are: `Initializing`, `InProgress`, and `Completed`.</span></span> <span data-ttu-id="73b2e-156">仅 `$filter` (和 `eq` `$orderby`) 。</span><span class="sxs-lookup"><span data-stu-id="73b2e-156">Supports `$filter` (`eq` only) and `$orderby`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="73b2e-157">关系</span><span class="sxs-lookup"><span data-stu-id="73b2e-157">Relationships</span></span>
|<span data-ttu-id="73b2e-158">关系</span><span class="sxs-lookup"><span data-stu-id="73b2e-158">Relationship</span></span>|<span data-ttu-id="73b2e-159">类型</span><span class="sxs-lookup"><span data-stu-id="73b2e-159">Type</span></span>|<span data-ttu-id="73b2e-160">说明</span><span class="sxs-lookup"><span data-stu-id="73b2e-160">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73b2e-161">审批</span><span class="sxs-lookup"><span data-stu-id="73b2e-161">approval</span></span>|[<span data-ttu-id="73b2e-162">审批</span><span class="sxs-lookup"><span data-stu-id="73b2e-162">approval</span></span>](../resources/approval.md)|<span data-ttu-id="73b2e-163">与请求相关的审批决策。</span><span class="sxs-lookup"><span data-stu-id="73b2e-163">Approval decisions associated with a request.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73b2e-164">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73b2e-164">JSON representation</span></span>
<span data-ttu-id="73b2e-165">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73b2e-165">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.userConsentRequest",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.userConsentRequest",
  "id": "String (identifier)",
  "status": "String",
  "completedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "approvalId": "String",
  "customData": "String",
  "createdBy": {
    "@odata.type": "microsoft.graph.identitySet"
  },
  "reason": "String"
}
```

