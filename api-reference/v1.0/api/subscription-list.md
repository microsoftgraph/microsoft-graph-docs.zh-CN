---
title: 列表订阅
description: 检索的属性和 webhook 订阅，基于应用程序 ID、 用户和与租户的用户的角色的关系。
localization_priority: Priority
author: piotrci
ms.openlocfilehash: c2e9446721f4390341c33f8b976893e4b1ab14be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972934"
---
# <a name="list-subscriptions"></a><span data-ttu-id="5638d-103">列表订阅</span><span class="sxs-lookup"><span data-stu-id="5638d-103">List subscriptions</span></span>

<span data-ttu-id="5638d-104">检索的属性和 webhook 订阅，基于应用程序 ID、 用户和与租户的用户的角色的关系。</span><span class="sxs-lookup"><span data-stu-id="5638d-104">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="5638d-105">权限</span><span class="sxs-lookup"><span data-stu-id="5638d-105">Permissions</span></span>

<span data-ttu-id="5638d-106">此 API 支持以下权限范围;若要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5638d-106">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5638d-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="5638d-107">Permission type</span></span>  | <span data-ttu-id="5638d-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5638d-108">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="5638d-109">[委派权限](/graph/auth-v2-user)（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5638d-109">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="5638d-110">[创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的角色。</span><span class="sxs-lookup"><span data-stu-id="5638d-110">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="5638d-111">[委派权限](/graph/auth-v2-user)（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5638d-111">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="5638d-112">[创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的角色。</span><span class="sxs-lookup"><span data-stu-id="5638d-112">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="5638d-113">应用程序的权限</span><span class="sxs-lookup"><span data-stu-id="5638d-113">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="5638d-114">[创建订阅](subscription-post-subscriptions.md)所需的角色。</span><span class="sxs-lookup"><span data-stu-id="5638d-114">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="5638d-115">响应结果基于调用应用程序的上下文。</span><span class="sxs-lookup"><span data-stu-id="5638d-115">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="5638d-116">以下是常见方案的摘要：</span><span class="sxs-lookup"><span data-stu-id="5638d-116">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="5638d-117">基本方案</span><span class="sxs-lookup"><span data-stu-id="5638d-117">Basic scenarios</span></span>

<span data-ttu-id="5638d-118">大多数情况下，应用程序要检索其最初创建对当前已登录的用户或 （工作/学校帐户） 的目录中的所有用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-118">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="5638d-119">这些方案不需要之外的任何特殊权限最初用于创建其订阅应用程序。</span><span class="sxs-lookup"><span data-stu-id="5638d-119">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="5638d-120">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="5638d-120">Context of the calling app</span></span> | <span data-ttu-id="5638d-121">响应中包含</span><span class="sxs-lookup"><span data-stu-id="5638d-121">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="5638d-122">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="5638d-122">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="5638d-123">-和-</span><span class="sxs-lookup"><span data-stu-id="5638d-123">-and-</span></span><br/><span data-ttu-id="5638d-124">应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="5638d-124">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="5638d-125">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="5638d-125">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="5638d-126">创建的**此应用程序**的已登录的用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-126">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="5638d-127">应用程序调用代表本身 （应用程序的权限）。</span><span class="sxs-lookup"><span data-stu-id="5638d-127">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="5638d-128">-和-</span><span class="sxs-lookup"><span data-stu-id="5638d-128">-and-</span></span><br/><span data-ttu-id="5638d-129">应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="5638d-129">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="5638d-130">注意： 这适用于工作/学校仅帐户。</span><span class="sxs-lookup"><span data-stu-id="5638d-130">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="5638d-131">创建**此**应用程序本身或目录中的任何用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-131">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="5638d-132">高级的方案</span><span class="sxs-lookup"><span data-stu-id="5638d-132">Advanced scenarios</span></span>

<span data-ttu-id="5638d-133">在某些情况下，希望检索订阅创建其他应用程序的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5638d-133">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="5638d-134">例如，用户想要查看由其代表任何应用程序创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-134">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="5638d-135">或者，管理员可能希望查看其目录中的所有应用程序中的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-135">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="5638d-136">如果是这种情况下，对于需要委派的权限 Subscription.Read.All。</span><span class="sxs-lookup"><span data-stu-id="5638d-136">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="5638d-137">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="5638d-137">Context of the calling app</span></span> | <span data-ttu-id="5638d-138">响应中包含</span><span class="sxs-lookup"><span data-stu-id="5638d-138">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="5638d-139">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="5638d-139">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="5638d-140">*用户在处于非管理员*。</span><span class="sxs-lookup"><span data-stu-id="5638d-140">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="5638d-141">-和-</span><span class="sxs-lookup"><span data-stu-id="5638d-141">-and-</span></span><br/><span data-ttu-id="5638d-142">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="5638d-142">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="5638d-143">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="5638d-143">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="5638d-144">创建的**任何应用程序**的已登录的用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-144">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="5638d-145">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="5638d-145">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="5638d-146">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="5638d-146">*The user is an admin*.</span></span><br/><span data-ttu-id="5638d-147">-和-</span><span class="sxs-lookup"><span data-stu-id="5638d-147">-and-</span></span><br/><span data-ttu-id="5638d-148">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="5638d-148">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="5638d-149">注意： 这适用于工作/学校仅帐户。</span><span class="sxs-lookup"><span data-stu-id="5638d-149">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="5638d-150">创建的**任何应用程序**目录中的**任何用户**的订阅。</span><span class="sxs-lookup"><span data-stu-id="5638d-150">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5638d-151">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5638d-151">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5638d-152">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5638d-152">Optional query parameters</span></span>

<span data-ttu-id="5638d-153">此方法不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="5638d-153">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5638d-154">请求标头</span><span class="sxs-lookup"><span data-stu-id="5638d-154">Request headers</span></span>

| <span data-ttu-id="5638d-155">名称</span><span class="sxs-lookup"><span data-stu-id="5638d-155">Name</span></span>       | <span data-ttu-id="5638d-156">类型</span><span class="sxs-lookup"><span data-stu-id="5638d-156">Type</span></span> | <span data-ttu-id="5638d-157">说明</span><span class="sxs-lookup"><span data-stu-id="5638d-157">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="5638d-158">Authorization</span><span class="sxs-lookup"><span data-stu-id="5638d-158">Authorization</span></span>  | <span data-ttu-id="5638d-159">string</span><span class="sxs-lookup"><span data-stu-id="5638d-159">string</span></span>  | <span data-ttu-id="5638d-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5638d-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5638d-162">请求正文</span><span class="sxs-lookup"><span data-stu-id="5638d-162">Request body</span></span>

<span data-ttu-id="5638d-163">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5638d-163">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5638d-164">响应</span><span class="sxs-lookup"><span data-stu-id="5638d-164">Response</span></span>

<span data-ttu-id="5638d-165">如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="5638d-165">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5638d-166">示例</span><span class="sxs-lookup"><span data-stu-id="5638d-166">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5638d-167">请求</span><span class="sxs-lookup"><span data-stu-id="5638d-167">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="5638d-168">响应</span><span class="sxs-lookup"><span data-stu-id="5638d-168">Response</span></span>

<span data-ttu-id="5638d-169">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="5638d-169">Here's an an example of the response.</span></span>  <span data-ttu-id="5638d-170">请注意，它可能会被截断为简便起见。</span><span class="sxs-lookup"><span data-stu-id="5638d-170">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="5638d-171">支持所有适用于请求的属性和将从实际的调用返回调用上下文。</span><span class="sxs-lookup"><span data-stu-id="5638d-171">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="5638d-172">请求返回的数据的多个页面，响应中包括`@odata.nextLink`属性可帮助您管理结果。</span><span class="sxs-lookup"><span data-stu-id="5638d-172">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="5638d-173">若要了解详细信息，请参阅[分页 Microsoft Graph 应用程序中的数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="5638d-173">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
