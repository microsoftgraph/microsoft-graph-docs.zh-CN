---
title: 列出订阅
description: 根据应用程序 ID、用户和用户的角色（含租户）检索 webhook 订阅的属性和关系。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: c2e9446721f4390341c33f8b976893e4b1ab14be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32560996"
---
# <a name="list-subscriptions"></a><span data-ttu-id="ea0ff-103">列出订阅</span><span class="sxs-lookup"><span data-stu-id="ea0ff-103">List subscriptions</span></span>

<span data-ttu-id="ea0ff-104">根据应用程序 ID、用户和用户的角色（含租户）检索 webhook 订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="ea0ff-105">权限</span><span class="sxs-lookup"><span data-stu-id="ea0ff-105">Permissions</span></span>

<span data-ttu-id="ea0ff-106">此 API 支持以下权限范围；要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="ea0ff-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea0ff-107">Permission type</span></span>  | <span data-ttu-id="ea0ff-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea0ff-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="ea0ff-109">[委派权限](/graph/auth-v2-user)（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea0ff-109">Delegated (work or school account)</span></span> | <span data-ttu-id="ea0ff-110">[create subscription](subscription-post-subscriptions.md) 或 Subscription.Read.All 所需的角色（请参阅下文）。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="ea0ff-111">[委派权限](/graph/auth-v2-user)（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea0ff-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea0ff-112">[create subscription](subscription-post-subscriptions.md) 或 Subscription.Read.All 所需的角色（请参阅下文）。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="ea0ff-113">应用程序权限</span><span class="sxs-lookup"><span data-stu-id="ea0ff-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="ea0ff-114">[创建订阅](subscription-post-subscriptions.md)所需的角色。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="ea0ff-115">响应结果基于调用应用的上下文。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="ea0ff-116">以下是常见方案的摘要：</span><span class="sxs-lookup"><span data-stu-id="ea0ff-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="ea0ff-117">基本方案</span><span class="sxs-lookup"><span data-stu-id="ea0ff-117">Basic planning scenarios</span></span>

<span data-ttu-id="ea0ff-118">最常见的情况是，应用程序希望检索最初为当前登录用户或者检索目录中的所有用户（工作/学校帐户）创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="ea0ff-119">除了应用最初用于创建订阅的权限外，这些方案不需要任何特殊权限。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="ea0ff-120">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="ea0ff-120">Context of the calling app</span></span> | <span data-ttu-id="ea0ff-121">响应包含</span><span class="sxs-lookup"><span data-stu-id="ea0ff-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="ea0ff-122">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="ea0ff-123">-且-</span><span class="sxs-lookup"><span data-stu-id="ea0ff-123">AND</span></span><br/><span data-ttu-id="ea0ff-124">应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="ea0ff-125">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="ea0ff-126">**此应用**仅为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="ea0ff-127">应用程序代表本身（应用程序权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="ea0ff-128">-且-</span><span class="sxs-lookup"><span data-stu-id="ea0ff-128">AND</span></span><br/><span data-ttu-id="ea0ff-129">应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="ea0ff-130">注意：这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="ea0ff-131">**此应用**仅为自己或者目录中的任何用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="ea0ff-132">高级方案</span><span class="sxs-lookup"><span data-stu-id="ea0ff-132">Advanced save scenarios</span></span>

<span data-ttu-id="ea0ff-133">在某些情况下，应用想要检索其他应用创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="ea0ff-134">例如，用户希望看到任何应用程序代表他们创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="ea0ff-135">或者，管理员可能希望查看其目录中所有应用的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="ea0ff-136">对于此类方案，委派权限 Subscription.Read.All 是必需的。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="ea0ff-137">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="ea0ff-137">Context of the calling app</span></span> | <span data-ttu-id="ea0ff-138">响应包含</span><span class="sxs-lookup"><span data-stu-id="ea0ff-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="ea0ff-139">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="ea0ff-140">*用户是非管理员*。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="ea0ff-141">-且-</span><span class="sxs-lookup"><span data-stu-id="ea0ff-141">AND</span></span><br/><span data-ttu-id="ea0ff-142">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea0ff-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="ea0ff-143">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="ea0ff-144">**任何应用**仅为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="ea0ff-145">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="ea0ff-146">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-146">*The user is an admin*.</span></span><br/><span data-ttu-id="ea0ff-147">-且-</span><span class="sxs-lookup"><span data-stu-id="ea0ff-147">AND</span></span><br/><span data-ttu-id="ea0ff-148">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="ea0ff-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="ea0ff-149">注意：这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="ea0ff-150">**任何应用**为目录中的**任何用户**创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ea0ff-151">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea0ff-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ea0ff-152">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ea0ff-152">Optional query parameters</span></span>

<span data-ttu-id="ea0ff-153">此方法不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="ea0ff-154">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea0ff-154">Request headers</span></span>

| <span data-ttu-id="ea0ff-155">名称</span><span class="sxs-lookup"><span data-stu-id="ea0ff-155">Name</span></span>       | <span data-ttu-id="ea0ff-156">类型</span><span class="sxs-lookup"><span data-stu-id="ea0ff-156">Type</span></span> | <span data-ttu-id="ea0ff-157">说明</span><span class="sxs-lookup"><span data-stu-id="ea0ff-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ea0ff-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea0ff-158">Authorization</span></span>  | <span data-ttu-id="ea0ff-159">string</span><span class="sxs-lookup"><span data-stu-id="ea0ff-159">string</span></span>  | <span data-ttu-id="ea0ff-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ea0ff-162">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea0ff-162">Request body</span></span>

<span data-ttu-id="ea0ff-163">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea0ff-164">响应</span><span class="sxs-lookup"><span data-stu-id="ea0ff-164">Response</span></span>

<span data-ttu-id="ea0ff-165">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-165">If successful, this method returns a `200 OK` response code and collection of [directoryAudit](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea0ff-166">示例</span><span class="sxs-lookup"><span data-stu-id="ea0ff-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ea0ff-167">请求</span><span class="sxs-lookup"><span data-stu-id="ea0ff-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="ea0ff-168">响应</span><span class="sxs-lookup"><span data-stu-id="ea0ff-168">Response</span></span>

<span data-ttu-id="ea0ff-169">以下是响应的一个示例。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-169">Here's an excerpt of the response:</span></span>  <span data-ttu-id="ea0ff-170">请注意为简洁起见它可能被截断。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="ea0ff-171">适用于请求和调用上下文的所有支持的属性将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.subscription",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 586

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

<span data-ttu-id="ea0ff-172">当请求返回多页数据时，响应中包含一个 `@odata.nextLink` 属性，可帮助你管理结果。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="ea0ff-173">若要了解详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="ea0ff-173">For more information, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
