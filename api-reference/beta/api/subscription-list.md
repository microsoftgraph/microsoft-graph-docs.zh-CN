---
title: 列表订阅
description: " 请参阅下面的方案的详细信息。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: e7b6c618c35aa9952673b79f238777a71bc41f6a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928778"
---
# <a name="list-subscriptions"></a><span data-ttu-id="97095-103">列表订阅</span><span class="sxs-lookup"><span data-stu-id="97095-103">List subscriptions</span></span>

> <span data-ttu-id="97095-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97095-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97095-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97095-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97095-106">检索 webhook 订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="97095-106">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="97095-107">将响应的内容取决于的上下文中调用应用程序;请参阅下面的方案的详细信息。</span><span class="sxs-lookup"><span data-stu-id="97095-107">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="97095-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="97095-108">Permissions</span></span>

<span data-ttu-id="97095-109">此 API 支持以下权限范围;若要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97095-109">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="97095-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97095-110">Permission type</span></span>  | <span data-ttu-id="97095-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="97095-111">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="97095-112">[委派](/graph/auth-v2-user)（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97095-112">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="97095-113">[创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的权限。</span><span class="sxs-lookup"><span data-stu-id="97095-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="97095-114">[委派](/graph/auth-v2-user)（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97095-114">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="97095-115">[创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的权限。</span><span class="sxs-lookup"><span data-stu-id="97095-115">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="97095-116">Application</span><span class="sxs-lookup"><span data-stu-id="97095-116">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="97095-117">[创建订阅](subscription-post-subscriptions.md)所需的权限。</span><span class="sxs-lookup"><span data-stu-id="97095-117">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="97095-118">响应结果基于调用应用程序的上下文。</span><span class="sxs-lookup"><span data-stu-id="97095-118">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="97095-119">以下是常见方案的摘要：</span><span class="sxs-lookup"><span data-stu-id="97095-119">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="97095-120">基本方案</span><span class="sxs-lookup"><span data-stu-id="97095-120">Basic scenarios</span></span>

<span data-ttu-id="97095-121">大多数情况下，应用程序要检索其最初创建对当前已登录的用户或 （工作/学校帐户） 的目录中的所有用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-121">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="97095-122">这些方案不需要之外的任何特殊权限最初用于创建其订阅应用程序。</span><span class="sxs-lookup"><span data-stu-id="97095-122">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="97095-123">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="97095-123">Context of the calling app</span></span> | <span data-ttu-id="97095-124">响应中包含</span><span class="sxs-lookup"><span data-stu-id="97095-124">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="97095-125">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="97095-125">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="97095-126">-和-</span><span class="sxs-lookup"><span data-stu-id="97095-126">-and-</span></span><br/><span data-ttu-id="97095-127">应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="97095-127">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="97095-128">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="97095-128">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="97095-129">创建的**此应用程序**的已登录的用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-129">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="97095-130">应用程序调用代表本身 （应用程序的权限）。</span><span class="sxs-lookup"><span data-stu-id="97095-130">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="97095-131">-和-</span><span class="sxs-lookup"><span data-stu-id="97095-131">-and-</span></span><br/><span data-ttu-id="97095-132">应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="97095-132">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="97095-133">注意： 这适用于工作/学校仅帐户。</span><span class="sxs-lookup"><span data-stu-id="97095-133">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="97095-134">创建**此**应用程序本身或目录中的任何用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-134">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="97095-135">高级的方案</span><span class="sxs-lookup"><span data-stu-id="97095-135">Advanced scenarios</span></span>

<span data-ttu-id="97095-136">在某些情况下，希望检索订阅创建其他应用程序的应用程序。</span><span class="sxs-lookup"><span data-stu-id="97095-136">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="97095-137">例如，用户想要查看由其代表任何应用程序创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-137">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="97095-138">或者，管理员可能希望查看其目录中的所有应用程序中的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-138">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="97095-139">如果是这种情况下，对于需要委派的权限 Subscription.Read.All。</span><span class="sxs-lookup"><span data-stu-id="97095-139">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="97095-140">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="97095-140">Context of the calling app</span></span> | <span data-ttu-id="97095-141">响应中包含</span><span class="sxs-lookup"><span data-stu-id="97095-141">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="97095-142">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="97095-142">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="97095-143">*用户在处于非管理员*。</span><span class="sxs-lookup"><span data-stu-id="97095-143">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="97095-144">-和-</span><span class="sxs-lookup"><span data-stu-id="97095-144">-and-</span></span><br/><span data-ttu-id="97095-145">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="97095-145">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="97095-146">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="97095-146">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="97095-147">创建的**任何应用程序**的已登录的用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-147">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="97095-148">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="97095-148">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="97095-149">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="97095-149">*The user is an admin*.</span></span><br/><span data-ttu-id="97095-150">-和-</span><span class="sxs-lookup"><span data-stu-id="97095-150">-and-</span></span><br/><span data-ttu-id="97095-151">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="97095-151">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="97095-152">注意： 这适用于工作/学校仅帐户。</span><span class="sxs-lookup"><span data-stu-id="97095-152">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="97095-153">创建的**任何应用程序**目录中的**任何用户**的订阅。</span><span class="sxs-lookup"><span data-stu-id="97095-153">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97095-154">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97095-154">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97095-155">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97095-155">Optional query parameters</span></span>

<span data-ttu-id="97095-156">此方法不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="97095-156">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97095-157">请求标头</span><span class="sxs-lookup"><span data-stu-id="97095-157">Request headers</span></span>

| <span data-ttu-id="97095-158">名称</span><span class="sxs-lookup"><span data-stu-id="97095-158">Name</span></span>       | <span data-ttu-id="97095-159">类型</span><span class="sxs-lookup"><span data-stu-id="97095-159">Type</span></span> | <span data-ttu-id="97095-160">说明</span><span class="sxs-lookup"><span data-stu-id="97095-160">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="97095-161">Authorization</span><span class="sxs-lookup"><span data-stu-id="97095-161">Authorization</span></span>  | <span data-ttu-id="97095-162">string</span><span class="sxs-lookup"><span data-stu-id="97095-162">string</span></span>  | <span data-ttu-id="97095-p108">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="97095-p108">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="97095-165">请求正文</span><span class="sxs-lookup"><span data-stu-id="97095-165">Request body</span></span>

<span data-ttu-id="97095-166">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97095-166">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97095-167">响应</span><span class="sxs-lookup"><span data-stu-id="97095-167">Response</span></span>

<span data-ttu-id="97095-168">如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="97095-168">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97095-169">示例</span><span class="sxs-lookup"><span data-stu-id="97095-169">Example</span></span>

##### <a name="request"></a><span data-ttu-id="97095-170">请求</span><span class="sxs-lookup"><span data-stu-id="97095-170">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="97095-171">响应</span><span class="sxs-lookup"><span data-stu-id="97095-171">Response</span></span>

<span data-ttu-id="97095-172">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="97095-172">Here is an example of the response.</span></span> <span data-ttu-id="97095-173">注意： 为了简单起见，如下所示的响应可能被截断。</span><span class="sxs-lookup"><span data-stu-id="97095-173">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="97095-174">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97095-174">All of the properties will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#subscriptions",
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

<span data-ttu-id="97095-175">请求返回的数据的多个页面，响应中包括`@odata.nextLink`属性可帮助您管理结果。</span><span class="sxs-lookup"><span data-stu-id="97095-175">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="97095-176">若要了解详细信息，请参阅[分页 Microsoft Graph 应用程序中的数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="97095-176">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
