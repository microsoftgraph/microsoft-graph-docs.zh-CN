---
title: 列出订阅
description: " 有关详细信息, 请参阅以下方案。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 3ffcf78c7df28faba22b92a7389f473f0ea91613
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335811"
---
# <a name="list-subscriptions"></a><span data-ttu-id="deec4-103">列出订阅</span><span class="sxs-lookup"><span data-stu-id="deec4-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deec4-104">检索 webhook 订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="deec4-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="deec4-105">响应的内容取决于在其中调用应用程序的上下文。有关详细信息, 请参阅以下方案。</span><span class="sxs-lookup"><span data-stu-id="deec4-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="deec4-106">权限</span><span class="sxs-lookup"><span data-stu-id="deec4-106">Permissions</span></span>

<span data-ttu-id="deec4-107">此 API 支持以下权限范围;若要了解详细信息, 包括如何选择权限, 请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deec4-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deec4-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="deec4-108">Permission type</span></span>  | <span data-ttu-id="deec4-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deec4-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="deec4-110">[委派](/graph/auth-v2-user)(工作或学校帐户)</span><span class="sxs-lookup"><span data-stu-id="deec4-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="deec4-111">[创建订阅](subscription-post-subscriptions.md)或订阅所需的权限。 Read. 所有 (请参阅下面的)。</span><span class="sxs-lookup"><span data-stu-id="deec4-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="deec4-112">[委派](/graph/auth-v2-user)(个人 Microsoft 帐户)</span><span class="sxs-lookup"><span data-stu-id="deec4-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="deec4-113">[创建订阅](subscription-post-subscriptions.md)或订阅所需的权限。 Read. 所有 (请参阅下面的)。</span><span class="sxs-lookup"><span data-stu-id="deec4-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="deec4-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="deec4-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="deec4-115">[创建订阅](subscription-post-subscriptions.md)所需的权限。</span><span class="sxs-lookup"><span data-stu-id="deec4-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="deec4-116">响应结果基于呼叫应用程序的上下文。</span><span class="sxs-lookup"><span data-stu-id="deec4-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="deec4-117">以下是常见方案的摘要:</span><span class="sxs-lookup"><span data-stu-id="deec4-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="deec4-118">基本方案</span><span class="sxs-lookup"><span data-stu-id="deec4-118">Basic scenarios</span></span>

<span data-ttu-id="deec4-119">通常情况下, 应用程序希望检索它最初为当前登录用户创建的订阅, 或者检索目录 (工作/学校帐户) 中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="deec4-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="deec4-120">这些方案不需要除了最初用于创建订阅的应用程序之外的任何特殊权限。</span><span class="sxs-lookup"><span data-stu-id="deec4-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="deec4-121">呼叫应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="deec4-121">Context of the calling app</span></span> | <span data-ttu-id="deec4-122">响应包含</span><span class="sxs-lookup"><span data-stu-id="deec4-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="deec4-123">应用代表已登录用户 (委派权限) 呼叫。</span><span class="sxs-lookup"><span data-stu-id="deec4-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="deec4-124">并</span><span class="sxs-lookup"><span data-stu-id="deec4-124">-and-</span></span><br/><span data-ttu-id="deec4-125">应用程序具有[创建订阅](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="deec4-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="deec4-126">注意: 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="deec4-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="deec4-127">仅**此应用**为登录用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="deec4-128">应用程序是代表自身调用的 (应用程序权限)。</span><span class="sxs-lookup"><span data-stu-id="deec4-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="deec4-129">并</span><span class="sxs-lookup"><span data-stu-id="deec4-129">-and-</span></span><br/><span data-ttu-id="deec4-130">应用程序具有[创建订阅](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="deec4-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="deec4-131">注意: 这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="deec4-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="deec4-132">**此应用**为自己或目录中的任何用户创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="deec4-133">高级方案</span><span class="sxs-lookup"><span data-stu-id="deec4-133">Advanced scenarios</span></span>

<span data-ttu-id="deec4-134">在某些情况下, 应用想要检索由其他应用程序创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="deec4-135">例如, 用户希望以代表自己的任意方式查看由任何应用程序创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="deec4-136">或者, 管理员可能想要查看其目录中所有应用程序的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="deec4-137">在这种情况下, 委派权限订阅是必需的。 All 是必需的。</span><span class="sxs-lookup"><span data-stu-id="deec4-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="deec4-138">呼叫应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="deec4-138">Context of the calling app</span></span> | <span data-ttu-id="deec4-139">响应包含</span><span class="sxs-lookup"><span data-stu-id="deec4-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="deec4-140">应用代表已登录用户 (委派权限) 呼叫。</span><span class="sxs-lookup"><span data-stu-id="deec4-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="deec4-141">*用户是非管理员*。</span><span class="sxs-lookup"><span data-stu-id="deec4-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="deec4-142">并</span><span class="sxs-lookup"><span data-stu-id="deec4-142">-and-</span></span><br/><span data-ttu-id="deec4-143">应用具有权限订阅。 Read. All</span><span class="sxs-lookup"><span data-stu-id="deec4-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="deec4-144">注意: 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="deec4-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="deec4-145">仅供登录用户使用的**任何应用程序所**创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="deec4-146">应用代表已登录用户 (委派权限) 呼叫。</span><span class="sxs-lookup"><span data-stu-id="deec4-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="deec4-147">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="deec4-147">*The user is an admin*.</span></span><br/><span data-ttu-id="deec4-148">并</span><span class="sxs-lookup"><span data-stu-id="deec4-148">-and-</span></span><br/><span data-ttu-id="deec4-149">应用具有权限订阅。 Read. All</span><span class="sxs-lookup"><span data-stu-id="deec4-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="deec4-150">注意: 这仅适用于工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="deec4-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="deec4-151">由目录中**任何用户**的**任何应用程序**创建的订阅。</span><span class="sxs-lookup"><span data-stu-id="deec4-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="deec4-152">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deec4-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="deec4-153">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="deec4-153">Optional query parameters</span></span>

<span data-ttu-id="deec4-154">此方法不支持[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="deec4-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="deec4-155">请求标头</span><span class="sxs-lookup"><span data-stu-id="deec4-155">Request headers</span></span>

| <span data-ttu-id="deec4-156">名称</span><span class="sxs-lookup"><span data-stu-id="deec4-156">Name</span></span>       | <span data-ttu-id="deec4-157">类型</span><span class="sxs-lookup"><span data-stu-id="deec4-157">Type</span></span> | <span data-ttu-id="deec4-158">说明</span><span class="sxs-lookup"><span data-stu-id="deec4-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="deec4-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="deec4-159">Authorization</span></span>  | <span data-ttu-id="deec4-160">string</span><span class="sxs-lookup"><span data-stu-id="deec4-160">string</span></span>  | <span data-ttu-id="deec4-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="deec4-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="deec4-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="deec4-163">Request body</span></span>

<span data-ttu-id="deec4-164">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="deec4-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="deec4-165">响应</span><span class="sxs-lookup"><span data-stu-id="deec4-165">Response</span></span>

<span data-ttu-id="deec4-166">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[订阅](../resources/subscription.md)对象列表。</span><span class="sxs-lookup"><span data-stu-id="deec4-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="deec4-167">示例</span><span class="sxs-lookup"><span data-stu-id="deec4-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="deec4-168">请求</span><span class="sxs-lookup"><span data-stu-id="deec4-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="deec4-169">响应</span><span class="sxs-lookup"><span data-stu-id="deec4-169">Response</span></span>

<span data-ttu-id="deec4-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="deec4-170">Here is an example of the response.</span></span> <span data-ttu-id="deec4-171">注意: 为简洁起见, 可能会截断此处显示的响应。</span><span class="sxs-lookup"><span data-stu-id="deec4-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="deec4-172">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="deec4-172">All of the properties will be returned from an actual call.</span></span>

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
      "creatorId": "8ee44408-0679-472c-bc2a-692812af3437"
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
  "suppressions": []
}
-->

<span data-ttu-id="deec4-173">当请求返回多个数据页时, 响应中包含一个`@odata.nextLink`可帮助您管理结果的属性。</span><span class="sxs-lookup"><span data-stu-id="deec4-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="deec4-174">若要了解详细信息, 请参阅[在应用中分页 Microsoft Graph 数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="deec4-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
