# <a name="list-subscriptions"></a><span data-ttu-id="cafd9-101">订阅列表</span><span class="sxs-lookup"><span data-stu-id="cafd9-101">List subscriptions</span></span>

<span data-ttu-id="cafd9-102">基于应用程序ID、用户和用户与租户的角色，检索webhook订阅的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cafd9-102">Retrieve the properties and relationships of webhook subscriptions, based on the app ID, the user, and the user's role with a tenant.</span></span>

## <a name="permissions"></a><span data-ttu-id="cafd9-103">权限</span><span class="sxs-lookup"><span data-stu-id="cafd9-103">Permissions</span></span>

<span data-ttu-id="cafd9-104">此API支持以下权限范围；若要了解详细信息，包括如何选择权限，请参阅 [权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cafd9-104">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

| <span data-ttu-id="cafd9-105">权限类型</span><span class="sxs-lookup"><span data-stu-id="cafd9-105">Permission type</span></span>  | <span data-ttu-id="cafd9-106">权限（从最低权限到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cafd9-106">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="cafd9-107">[委派的](../../../concepts/auth_v2_user.md) （工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cafd9-107">Delegated (work or school account)</span></span> | <span data-ttu-id="cafd9-108"> [创建订阅](subscription_get.md) 或 Subscriptions.Read.All （见下文） 所需的角色。</span><span class="sxs-lookup"><span data-stu-id="cafd9-108">Role required to [create subscription](subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| <span data-ttu-id="cafd9-109">[委派的](../../../concepts/auth_v2_user.md) （个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cafd9-109">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cafd9-110"> [创建订阅](./subscription_get.md) 或 Subscriptions.Read.All （见下文） 所需的角色。</span><span class="sxs-lookup"><span data-stu-id="cafd9-110">Role required to [create subscription](./subscription_get.md) or Subscriptions.Read.All (see below).</span></span> |
| [<span data-ttu-id="cafd9-111">应用程序</span><span class="sxs-lookup"><span data-stu-id="cafd9-111">Application</span></span>](../../../concepts/auth_v2_service.md) | <span data-ttu-id="cafd9-112">[创建订阅](./subscription_get.md)所需的角色。</span><span class="sxs-lookup"><span data-stu-id="cafd9-112">Role required to [create subscription](./subscription_get.md).</span></span> |

<span data-ttu-id="cafd9-113">响应结果基于调用应用程序的上下文。</span><span class="sxs-lookup"><span data-stu-id="cafd9-113">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="cafd9-114">以下是常见方案的总结：</span><span class="sxs-lookup"><span data-stu-id="cafd9-114">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="cafd9-115">基本方案</span><span class="sxs-lookup"><span data-stu-id="cafd9-115">Basic planning scenarios</span></span>

<span data-ttu-id="cafd9-116">大多数情况下，应用程序要检索其最初创建对当前已登录的用户或目录中所有用户（工作/学校帐户）的订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-116">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="cafd9-117">这些方案不需要最初用以创建其订阅的应用程序之外的任何特殊权限。</span><span class="sxs-lookup"><span data-stu-id="cafd9-117">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="cafd9-118">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="cafd9-118">Context of the calling app</span></span> | <span data-ttu-id="cafd9-119">响应中包含</span><span class="sxs-lookup"><span data-stu-id="cafd9-119">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="cafd9-120">应用程序代表登录用户调用（委派权限）。</span><span class="sxs-lookup"><span data-stu-id="cafd9-120">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="cafd9-121">-和-</span><span class="sxs-lookup"><span data-stu-id="cafd9-121">and</span></span><br/><span data-ttu-id="cafd9-122">应用程序具有[创建订阅](subscription_post_subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="cafd9-122">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="cafd9-123">注意：这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="cafd9-123">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="cafd9-124">只为已登录用户创建的 **此应用程序** 的订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-124">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="cafd9-125">应用程序调用代表本身 （应用程序的权限）。</span><span class="sxs-lookup"><span data-stu-id="cafd9-125">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="cafd9-126">-和-</span><span class="sxs-lookup"><span data-stu-id="cafd9-126">and</span></span><br/><span data-ttu-id="cafd9-127">应用程序具有[创建订阅](subscription_post_subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="cafd9-127">App has the original permission required to [create the subscription](subscription_post_subscriptions.md).</span></span><br/><br/><span data-ttu-id="cafd9-128">注意：这只适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="cafd9-128">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="cafd9-129">创建 **此应用程序** 本身或目录中任何用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-129">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="cafd9-130">高级方案</span><span class="sxs-lookup"><span data-stu-id="cafd9-130">Advanced save scenarios</span></span>

<span data-ttu-id="cafd9-131">在某些情况下，应用程序希望检索其他应用程序创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-131">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="cafd9-132">例如，用户想要查看由任何应用程序代表其创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-132">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="cafd9-133">或者，管理员可能希望查看其目录中所有应用程序的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-133">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="cafd9-134">如果是这种情况下，需要委派权限 Subscription.Read.All。</span><span class="sxs-lookup"><span data-stu-id="cafd9-134">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="cafd9-135">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="cafd9-135">Context of the calling app</span></span> | <span data-ttu-id="cafd9-136">响应中包含</span><span class="sxs-lookup"><span data-stu-id="cafd9-136">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="cafd9-137">应用程序代表登录用户调用（委派权限）。</span><span class="sxs-lookup"><span data-stu-id="cafd9-137">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="cafd9-138">*用户非管理员*。</span><span class="sxs-lookup"><span data-stu-id="cafd9-138">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="cafd9-139">-和-</span><span class="sxs-lookup"><span data-stu-id="cafd9-139">and</span></span><br/><span data-ttu-id="cafd9-140">应用程序具有 Subscription.Read.All 权限</span><span class="sxs-lookup"><span data-stu-id="cafd9-140">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="cafd9-141">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="cafd9-141">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="cafd9-142">只为已登录用户创建的 **任何应用程序** 的订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-142">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="cafd9-143">应用程序代表登录用户调用（委派权限）。</span><span class="sxs-lookup"><span data-stu-id="cafd9-143">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="cafd9-144">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="cafd9-144">*The user is an admin*.</span></span><br/><span data-ttu-id="cafd9-145">-和-</span><span class="sxs-lookup"><span data-stu-id="cafd9-145">and</span></span><br/><span data-ttu-id="cafd9-146">应用程序具有 Subscription.Read.All 权限</span><span class="sxs-lookup"><span data-stu-id="cafd9-146">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="cafd9-147">注意：这只适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="cafd9-147">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="cafd9-148">创建的 **任何应用程序** 目录中 **任何用户** 的订阅。</span><span class="sxs-lookup"><span data-stu-id="cafd9-148">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cafd9-149">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cafd9-149">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cafd9-150">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cafd9-150">Optional query parameters</span></span>

<span data-ttu-id="cafd9-151">此方法不支持帮助适应于响应的 [OData 查询参数](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) 。</span><span class="sxs-lookup"><span data-stu-id="cafd9-151">This method does not support the [OData Query Parameters](http://developer.microsoft.com/en-us/graph/docs/overview/query_parameters) to help customize the response (e.g. $filter is not supported here).</span></span>

## <a name="request-headers"></a><span data-ttu-id="cafd9-152">请求的标头</span><span class="sxs-lookup"><span data-stu-id="cafd9-152">Request headers</span></span>

| <span data-ttu-id="cafd9-153">名称</span><span class="sxs-lookup"><span data-stu-id="cafd9-153">Name</span></span>       | <span data-ttu-id="cafd9-154">类型</span><span class="sxs-lookup"><span data-stu-id="cafd9-154">Type</span></span> | <span data-ttu-id="cafd9-155">说明</span><span class="sxs-lookup"><span data-stu-id="cafd9-155">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cafd9-156">授权</span><span class="sxs-lookup"><span data-stu-id="cafd9-156">Authorization</span></span>  | <span data-ttu-id="cafd9-157">字符串</span><span class="sxs-lookup"><span data-stu-id="cafd9-157">string</span></span>  | <span data-ttu-id="cafd9-p106">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cafd9-p106">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cafd9-160">请求正文</span><span class="sxs-lookup"><span data-stu-id="cafd9-160">Request body</span></span>

<span data-ttu-id="cafd9-161">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cafd9-161">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cafd9-162">响应</span><span class="sxs-lookup"><span data-stu-id="cafd9-162">Response</span></span>

<span data-ttu-id="cafd9-163">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [订阅](../resources/subscription.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="cafd9-163">If successful, this method returns a `200 OK` response code and collection of [groupSettingTemplate](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cafd9-164">示例</span><span class="sxs-lookup"><span data-stu-id="cafd9-164">Example</span></span>

##### <a name="request"></a><span data-ttu-id="cafd9-165">请求</span><span class="sxs-lookup"><span data-stu-id="cafd9-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/v1.0/subscriptions
```

##### <a name="response"></a><span data-ttu-id="cafd9-166">响应</span><span class="sxs-lookup"><span data-stu-id="cafd9-166">Response</span></span>

<span data-ttu-id="cafd9-167">下面是响应的示例。</span><span class="sxs-lookup"><span data-stu-id="cafd9-167">Here's an excerpt of the response:</span></span>  <span data-ttu-id="cafd9-168">请注意，它可能会为了简便而被截断。</span><span class="sxs-lookup"><span data-stu-id="cafd9-168">Note that it may be truncated for brevity.</span></span>  <span data-ttu-id="cafd9-169">支持所有适用于请求的属性并从实际的调用返回调用上下文。</span><span class="sxs-lookup"><span data-stu-id="cafd9-169">All supported properties appropriate for the request and the calling context will be returned from an actual call.</span></span>

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

<span data-ttu-id="cafd9-170">请求返回多个页面的数据时，响应中包括 `@odata.nextLink` 属性可帮助您管理结果。</span><span class="sxs-lookup"><span data-stu-id="cafd9-170">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="cafd9-171">若要了解详细信息，请参阅 [Paging Microsoft Graph 应用程序中的数据](../../../concepts/paging.md)。</span><span class="sxs-lookup"><span data-stu-id="cafd9-171">To learn more, see [Paging Microsoft Graph data in your app](../../../concepts/paging.md).</span></span>
