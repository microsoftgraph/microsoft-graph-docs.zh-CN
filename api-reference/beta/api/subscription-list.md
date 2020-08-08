---
title: 列出订阅
description: " 有关详细信息，请参阅以下方案。"
localization_priority: Normal
author: davidmu1
doc_type: apiPageType
ms.prod: ''
ms.openlocfilehash: 6c04d7bb51fa5f99694d01d703b18e5073450cf9
ms.sourcegitcommit: bbff139eea483faaa2d1dd08af39314f35ef48ce
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/08/2020
ms.locfileid: "46598141"
---
# <a name="list-subscriptions"></a><span data-ttu-id="9b5bb-103">列出订阅</span><span class="sxs-lookup"><span data-stu-id="9b5bb-103">List subscriptions</span></span>

<span data-ttu-id="9b5bb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9b5bb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9b5bb-105">检索 webhook 订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-105">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="9b5bb-106">响应的内容取决于在其中调用应用程序的上下文。有关详细信息，请参阅以下方案。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-106">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="9b5bb-107">权限</span><span class="sxs-lookup"><span data-stu-id="9b5bb-107">Permissions</span></span>

<span data-ttu-id="9b5bb-108">此 API 支持以下权限范围；要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-108">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="9b5bb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9b5bb-109">Permission type</span></span>  | <span data-ttu-id="9b5bb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9b5bb-110">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="9b5bb-111">[委派](/graph/auth-v2-user) (工作或学校帐户) </span><span class="sxs-lookup"><span data-stu-id="9b5bb-111">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="9b5bb-112">[创建订阅](subscription-post-subscriptions.md)或订阅所需的权限。读取。所有 (请参阅下面) 。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-112">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="9b5bb-113">[委派](/graph/auth-v2-user) (个人 Microsoft 帐户) </span><span class="sxs-lookup"><span data-stu-id="9b5bb-113">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="9b5bb-114">[创建订阅](subscription-post-subscriptions.md)或订阅所需的权限。读取。所有 (请参阅下面) 。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-114">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="9b5bb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9b5bb-115">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="9b5bb-116">[创建订阅](subscription-post-subscriptions.md)所需的权限。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-116">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="9b5bb-117">响应结果基于调用应用的上下文。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-117">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="9b5bb-118">以下是常见方案的摘要：</span><span class="sxs-lookup"><span data-stu-id="9b5bb-118">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="9b5bb-119">基本方案</span><span class="sxs-lookup"><span data-stu-id="9b5bb-119">Basic scenarios</span></span>

<span data-ttu-id="9b5bb-120">最常见的情况是，应用程序希望检索最初为当前登录用户或者检索目录中的所有用户（工作/学校帐户）创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-120">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="9b5bb-121">除了应用最初用于创建订阅的权限外，这些方案不需要任何特殊权限。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-121">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="9b5bb-122">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="9b5bb-122">Context of the calling app</span></span> | <span data-ttu-id="9b5bb-123">响应包含</span><span class="sxs-lookup"><span data-stu-id="9b5bb-123">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="9b5bb-124">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-124">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="9b5bb-125">-且-</span><span class="sxs-lookup"><span data-stu-id="9b5bb-125">-and-</span></span><br/><span data-ttu-id="9b5bb-126">应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-126">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="9b5bb-127">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-127">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="9b5bb-128">**此应用**仅为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-128">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="9b5bb-129">应用程序代表本身（应用程序权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-129">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="9b5bb-130">-且-</span><span class="sxs-lookup"><span data-stu-id="9b5bb-130">-and-</span></span><br/><span data-ttu-id="9b5bb-131">应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-131">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="9b5bb-132">注意：这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-132">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="9b5bb-133">**此应用**仅为自己或者目录中的任何用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-133">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="9b5bb-134">高级方案</span><span class="sxs-lookup"><span data-stu-id="9b5bb-134">Advanced scenarios</span></span>

<span data-ttu-id="9b5bb-135">在某些情况下，应用想要检索其他应用创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-135">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="9b5bb-136">例如，用户希望看到任何应用程序代表他们创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-136">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="9b5bb-137">或者，管理员可能希望查看其目录中所有应用的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-137">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="9b5bb-138">对于此类方案，委派权限 Subscription.Read.All 是必需的。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-138">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="9b5bb-139">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="9b5bb-139">Context of the calling app</span></span> | <span data-ttu-id="9b5bb-140">响应包含</span><span class="sxs-lookup"><span data-stu-id="9b5bb-140">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="9b5bb-141">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-141">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="9b5bb-142">*用户是非管理员*。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-142">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="9b5bb-143">-且-</span><span class="sxs-lookup"><span data-stu-id="9b5bb-143">-and-</span></span><br/><span data-ttu-id="9b5bb-144">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b5bb-144">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="9b5bb-145">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-145">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="9b5bb-146">**任何应用**仅为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-146">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="9b5bb-147">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-147">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="9b5bb-148">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-148">*The user is an admin*.</span></span><br/><span data-ttu-id="9b5bb-149">-且-</span><span class="sxs-lookup"><span data-stu-id="9b5bb-149">-and-</span></span><br/><span data-ttu-id="9b5bb-150">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="9b5bb-150">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="9b5bb-151">注意：这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-151">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="9b5bb-152">**任何应用**为目录中的**任何用户**创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-152">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9b5bb-153">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9b5bb-153">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9b5bb-154">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9b5bb-154">Optional query parameters</span></span>

<span data-ttu-id="9b5bb-155">此方法不支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-155">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="9b5bb-156">请求标头</span><span class="sxs-lookup"><span data-stu-id="9b5bb-156">Request headers</span></span>

| <span data-ttu-id="9b5bb-157">名称</span><span class="sxs-lookup"><span data-stu-id="9b5bb-157">Name</span></span>       | <span data-ttu-id="9b5bb-158">类型</span><span class="sxs-lookup"><span data-stu-id="9b5bb-158">Type</span></span> | <span data-ttu-id="9b5bb-159">说明</span><span class="sxs-lookup"><span data-stu-id="9b5bb-159">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9b5bb-160">Authorization</span><span class="sxs-lookup"><span data-stu-id="9b5bb-160">Authorization</span></span>  | <span data-ttu-id="9b5bb-161">string</span><span class="sxs-lookup"><span data-stu-id="9b5bb-161">string</span></span>  | <span data-ttu-id="9b5bb-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9b5bb-164">请求正文</span><span class="sxs-lookup"><span data-stu-id="9b5bb-164">Request body</span></span>

<span data-ttu-id="9b5bb-165">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-165">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9b5bb-166">响应</span><span class="sxs-lookup"><span data-stu-id="9b5bb-166">Response</span></span>

<span data-ttu-id="9b5bb-167">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-167">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9b5bb-168">示例</span><span class="sxs-lookup"><span data-stu-id="9b5bb-168">Example</span></span>

##### <a name="request"></a><span data-ttu-id="9b5bb-169">请求</span><span class="sxs-lookup"><span data-stu-id="9b5bb-169">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9b5bb-170">HTTP</span><span class="sxs-lookup"><span data-stu-id="9b5bb-170">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/subscriptions
```
# <a name="c"></a>[<span data-ttu-id="9b5bb-171">C#</span><span class="sxs-lookup"><span data-stu-id="9b5bb-171">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9b5bb-172">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9b5bb-172">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9b5bb-173">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9b5bb-173">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9b5bb-174">响应</span><span class="sxs-lookup"><span data-stu-id="9b5bb-174">Response</span></span>

<span data-ttu-id="9b5bb-175">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-175">Here is an example of the response.</span></span> <span data-ttu-id="9b5bb-176">注意：为简洁起见，可能会截断此处显示的响应。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-176">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="9b5bb-177">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-177">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
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
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

> <span data-ttu-id="9b5bb-178">**注意：** 出于安全目的，不会返回 `clientState` 属性值。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-178">**Note:** the `clientState` property value is not returned for security purposes.</span></span>  

<span data-ttu-id="9b5bb-179">当请求返回多页数据时，响应中包含一个 `@odata.nextLink` 属性，可帮助你管理结果。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-179">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="9b5bb-180">若要了解详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="9b5bb-180">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
