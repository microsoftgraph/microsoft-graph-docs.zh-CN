---
<span data-ttu-id="e374e-101">title： "List subscriptions" description： "Retrieve the properties and relationships of webhook subscriptions， based on the app ID， the user， and the user's role with a tenant."</span><span class="sxs-lookup"><span data-stu-id="e374e-101">title: "List subscriptions" description: "Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant."</span></span>
<span data-ttu-id="e374e-102">localization_priority： Priority author： "Jumaodhiss" ms.prod： ""change-notifications" doc_type： apiPageType</span><span class="sxs-lookup"><span data-stu-id="e374e-102">localization_priority: Priority author: "Jumaodhiss" ms.prod: ""change-notifications" doc_type: apiPageType</span></span>
---

# <a name="list-subscriptions"></a><span data-ttu-id="e374e-103">列出订阅</span><span class="sxs-lookup"><span data-stu-id="e374e-103">List subscriptions</span></span>

<span data-ttu-id="e374e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e374e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e374e-105">根据应用程序 ID、用户和用户的角色（含租户）检索 webhook 订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e374e-105">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="e374e-106">权限</span><span class="sxs-lookup"><span data-stu-id="e374e-106">Permissions</span></span>

<span data-ttu-id="e374e-107">此 API 支持以下权限范围；要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e374e-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="e374e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e374e-108">Permission type</span></span>  | <span data-ttu-id="e374e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e374e-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="e374e-110">[委派权限](/graph/auth-v2-user)（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e374e-110">[Delegated permission](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="e374e-111">[create subscription](subscription-post-subscriptions.md) 或 Subscription.Read.All 所需的角色（请参阅下文）。</span><span class="sxs-lookup"><span data-stu-id="e374e-111">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="e374e-112">[委派权限](/graph/auth-v2-user)（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e374e-112">[Delegated permission](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="e374e-113">[create subscription](subscription-post-subscriptions.md) 或 Subscription.Read.All 所需的角色（请参阅下文）。</span><span class="sxs-lookup"><span data-stu-id="e374e-113">Role required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="e374e-114">应用程序权限</span><span class="sxs-lookup"><span data-stu-id="e374e-114">Application permission</span></span>](/graph/auth-v2-service) | <span data-ttu-id="e374e-115">[创建订阅](subscription-post-subscriptions.md)所需的角色。</span><span class="sxs-lookup"><span data-stu-id="e374e-115">Role required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="e374e-116">响应结果基于调用应用的上下文。</span><span class="sxs-lookup"><span data-stu-id="e374e-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="e374e-117">以下是常见方案的摘要：</span><span class="sxs-lookup"><span data-stu-id="e374e-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="e374e-118">基本方案</span><span class="sxs-lookup"><span data-stu-id="e374e-118">Basic scenarios</span></span>

<span data-ttu-id="e374e-119">最常见的情况是，应用程序希望检索最初为当前登录用户或者检索目录中的所有用户（工作/学校帐户）创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="e374e-120">除了应用最初用于创建订阅的权限外，这些方案不需要任何特殊权限。</span><span class="sxs-lookup"><span data-stu-id="e374e-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="e374e-121">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="e374e-121">Context of the calling app</span></span> | <span data-ttu-id="e374e-122">响应包含</span><span class="sxs-lookup"><span data-stu-id="e374e-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="e374e-123">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="e374e-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="e374e-124">-且-</span><span class="sxs-lookup"><span data-stu-id="e374e-124">-and-</span></span><br/><span data-ttu-id="e374e-125">应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。</span><span class="sxs-lookup"><span data-stu-id="e374e-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="e374e-126">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="e374e-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="e374e-127">**此应用** 仅为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="e374e-128">应用程序代表本身（应用程序权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="e374e-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="e374e-129">-且-</span><span class="sxs-lookup"><span data-stu-id="e374e-129">-and-</span></span><br/><span data-ttu-id="e374e-130">应用程序具有[创建该订阅](subscription-post-subscriptions.md)所需的初始权限。</span><span class="sxs-lookup"><span data-stu-id="e374e-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="e374e-131">注意：这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="e374e-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="e374e-132">**此应用** 仅为自己或者目录中的任何用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="e374e-133">高级方案</span><span class="sxs-lookup"><span data-stu-id="e374e-133">Advanced scenarios</span></span>

<span data-ttu-id="e374e-134">在某些情况下，应用想要检索其他应用创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="e374e-135">例如，用户希望看到任何应用程序代表他们创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="e374e-136">或者，管理员可能希望查看其目录中所有应用的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="e374e-137">对于此类方案，委派权限 Subscription.Read.All 是必需的。</span><span class="sxs-lookup"><span data-stu-id="e374e-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="e374e-138">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="e374e-138">Context of the calling app</span></span> | <span data-ttu-id="e374e-139">响应包含</span><span class="sxs-lookup"><span data-stu-id="e374e-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="e374e-140">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="e374e-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="e374e-141">*用户是非管理员*。</span><span class="sxs-lookup"><span data-stu-id="e374e-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="e374e-142">-且-</span><span class="sxs-lookup"><span data-stu-id="e374e-142">-and-</span></span><br/><span data-ttu-id="e374e-143">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="e374e-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="e374e-144">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="e374e-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="e374e-145">**任何应用** 仅为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="e374e-146">应用程序代表已登录用户（委派权限）进行调用。</span><span class="sxs-lookup"><span data-stu-id="e374e-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="e374e-147">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="e374e-147">*The user is an admin*.</span></span><br/><span data-ttu-id="e374e-148">-且-</span><span class="sxs-lookup"><span data-stu-id="e374e-148">-and-</span></span><br/><span data-ttu-id="e374e-149">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="e374e-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="e374e-150">注意：这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="e374e-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="e374e-151">**任何应用** 为目录中的 **任何用户** 创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="e374e-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e374e-152">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e374e-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e374e-153">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e374e-153">Optional query parameters</span></span>

<span data-ttu-id="e374e-154">此方法不支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e374e-154">This method does not support the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e374e-155">请求标头</span><span class="sxs-lookup"><span data-stu-id="e374e-155">Request headers</span></span>

| <span data-ttu-id="e374e-156">名称</span><span class="sxs-lookup"><span data-stu-id="e374e-156">Name</span></span>       | <span data-ttu-id="e374e-157">类型</span><span class="sxs-lookup"><span data-stu-id="e374e-157">Type</span></span> | <span data-ttu-id="e374e-158">说明</span><span class="sxs-lookup"><span data-stu-id="e374e-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="e374e-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="e374e-159">Authorization</span></span>  | <span data-ttu-id="e374e-160">string</span><span class="sxs-lookup"><span data-stu-id="e374e-160">string</span></span>  | <span data-ttu-id="e374e-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e374e-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e374e-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="e374e-163">Request body</span></span>

<span data-ttu-id="e374e-164">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e374e-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e374e-165">响应</span><span class="sxs-lookup"><span data-stu-id="e374e-165">Response</span></span>

<span data-ttu-id="e374e-166">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [subscription](../resources/subscription.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e374e-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e374e-167">示例</span><span class="sxs-lookup"><span data-stu-id="e374e-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="e374e-168">请求</span><span class="sxs-lookup"><span data-stu-id="e374e-168">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e374e-169">HTTP</span><span class="sxs-lookup"><span data-stu-id="e374e-169">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/subscriptions
```
# <a name="c"></a>[<span data-ttu-id="e374e-170">C#</span><span class="sxs-lookup"><span data-stu-id="e374e-170">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-subscriptions-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e374e-171">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e374e-171">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-subscriptions-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e374e-172">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e374e-172">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-subscriptions-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e374e-173">Java</span><span class="sxs-lookup"><span data-stu-id="e374e-173">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-subscriptions-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="e374e-174">响应</span><span class="sxs-lookup"><span data-stu-id="e374e-174">Response</span></span>

<span data-ttu-id="e374e-175">以下是响应示例。</span><span class="sxs-lookup"><span data-stu-id="e374e-175">Here's an example of the response.</span></span>  <span data-ttu-id="e374e-176">请注意为简洁起见它可能被截断。</span><span class="sxs-lookup"><span data-stu-id="e374e-176">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="e374e-177">适用于请求和调用上下文的所有支持的属性将从实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e374e-177">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#subscriptions",
  "value": [
    {
      "id": "0fc0d6db-0073-42e5-a186-853da75fb308",
      "resource": "Users",
      "applicationId": "24d3b144-21ae-4080-943f-7067b395b913",
      "changeType": "updated,deleted",
      "clientState": null,
      "notificationUrl": "https://webhookappexample.azurewebsites.net/api/notifications",
      "lifecycleNotificationUrl":"https://webhook.azurewebsites.net/api/send/lifecycleNotifications",
      "expirationDateTime": "2018-03-12T05:00:00Z",
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437",
      "latestSupportedTlsVersion": "v1_2",
      "encryptionCertificate": "",
      "encryptionCertificateId": "",
      "includeResourceData": false,
      "notificationContentType": "application/json"
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
  "tocPath": "",
  "suppressions": [
  ]
}-->

> <span data-ttu-id="e374e-178">**注意：** 出于安全目的，不会返回 `clientState` 属性值。</span><span class="sxs-lookup"><span data-stu-id="e374e-178">**Note:** the `clientState` property value is not returned for security purposes.</span></span>  

<span data-ttu-id="e374e-179">当请求返回多页数据时，响应中包含一个 `@odata.nextLink` 属性，可帮助你管理结果。</span><span class="sxs-lookup"><span data-stu-id="e374e-179">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="e374e-180">若要了解详细信息，请参阅[在应用中对 Microsoft Graph 数据进行分页](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="e374e-180">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
