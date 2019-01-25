---
title: 列表订阅
description: " 请参阅下面的方案的详细信息。"
localization_priority: Normal
author: piotrci
ms.openlocfilehash: 20aad712bc49f91bec58a67c0c66ef76bf4653e2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510979"
---
# <a name="list-subscriptions"></a><span data-ttu-id="56f1d-103">列表订阅</span><span class="sxs-lookup"><span data-stu-id="56f1d-103">List subscriptions</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="56f1d-104">检索 webhook 订阅的列表。</span><span class="sxs-lookup"><span data-stu-id="56f1d-104">Retrieve a list of webhook subscriptions.</span></span> <span data-ttu-id="56f1d-105">将响应的内容取决于的上下文中调用应用程序;请参阅下面的方案的详细信息。</span><span class="sxs-lookup"><span data-stu-id="56f1d-105">The content of the response depends on the context in which the app is calling; see the scenarios below for details.</span></span>

## <a name="permissions"></a><span data-ttu-id="56f1d-106">权限</span><span class="sxs-lookup"><span data-stu-id="56f1d-106">Permissions</span></span>

<span data-ttu-id="56f1d-107">此 API 支持以下权限范围;若要了解详细信息，包括如何选择权限，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="56f1d-107">This API supports the following permission scopes; to learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="56f1d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="56f1d-108">Permission type</span></span>  | <span data-ttu-id="56f1d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="56f1d-109">Permissions (from least to most privileged)</span></span>  |
|:---------------- |:-------------------------------------------- |
| <span data-ttu-id="56f1d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="56f1d-110">[Delegated](/graph/auth-v2-user) (work or school account)</span></span> | <span data-ttu-id="56f1d-111">[创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的权限。</span><span class="sxs-lookup"><span data-stu-id="56f1d-111">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| <span data-ttu-id="56f1d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="56f1d-112">[Delegated](/graph/auth-v2-user) (personal Microsoft account)</span></span> | <span data-ttu-id="56f1d-113">[创建订阅](subscription-post-subscriptions.md)或 Subscription.Read.All （见下文） 所需的权限。</span><span class="sxs-lookup"><span data-stu-id="56f1d-113">Permission required to [create subscription](subscription-post-subscriptions.md) or Subscription.Read.All (see below).</span></span> |
| [<span data-ttu-id="56f1d-114">Application</span><span class="sxs-lookup"><span data-stu-id="56f1d-114">Application</span></span>](/graph/auth-v2-service) | <span data-ttu-id="56f1d-115">[创建订阅](subscription-post-subscriptions.md)所需的权限。</span><span class="sxs-lookup"><span data-stu-id="56f1d-115">Permission required to [create subscription](subscription-post-subscriptions.md).</span></span> |

<span data-ttu-id="56f1d-116">响应结果基于调用应用程序的上下文。</span><span class="sxs-lookup"><span data-stu-id="56f1d-116">Response results are based on the context of the calling app.</span></span> <span data-ttu-id="56f1d-117">以下是常见方案的摘要：</span><span class="sxs-lookup"><span data-stu-id="56f1d-117">The following is a summary of the common scenarios:</span></span>

### <a name="basic-scenarios"></a><span data-ttu-id="56f1d-118">基本方案</span><span class="sxs-lookup"><span data-stu-id="56f1d-118">Basic scenarios</span></span>

<span data-ttu-id="56f1d-119">大多数情况下，应用程序要检索其最初创建对当前已登录的用户或 （工作/学校帐户） 的目录中的所有用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-119">Most commonly, an application wants to retrieve subscriptions that it originally created for the currently signed-in user, or for all users in the directory (work/school accounts).</span></span> <span data-ttu-id="56f1d-120">这些方案不需要之外的任何特殊权限最初用于创建其订阅应用程序。</span><span class="sxs-lookup"><span data-stu-id="56f1d-120">These scenarios do not require any special permissions beyond the ones the app used originally to create its subscriptions.</span></span>

| <span data-ttu-id="56f1d-121">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="56f1d-121">Context of the calling app</span></span> | <span data-ttu-id="56f1d-122">响应中包含</span><span class="sxs-lookup"><span data-stu-id="56f1d-122">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="56f1d-123">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="56f1d-123">App is calling on behalf of the signed-in user (delegated permission).</span></span> <br/><span data-ttu-id="56f1d-124">And</span><span class="sxs-lookup"><span data-stu-id="56f1d-124">-and-</span></span><br/><span data-ttu-id="56f1d-125">应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="56f1d-125">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="56f1d-126">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="56f1d-126">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="56f1d-127">创建的**此应用程序**的已登录的用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-127">Subscriptions created by **this app** for the signed-in user only.</span></span> |
| <span data-ttu-id="56f1d-128">应用程序调用代表本身 （应用程序的权限）。</span><span class="sxs-lookup"><span data-stu-id="56f1d-128">App is calling on behalf of itself (application permission).</span></span><br/><span data-ttu-id="56f1d-129">And</span><span class="sxs-lookup"><span data-stu-id="56f1d-129">-and-</span></span><br/><span data-ttu-id="56f1d-130">应用程序具有到[创建订阅，](subscription-post-subscriptions.md)所需的原始权限。</span><span class="sxs-lookup"><span data-stu-id="56f1d-130">App has the original permission required to [create the subscription](subscription-post-subscriptions.md).</span></span><br/><br/><span data-ttu-id="56f1d-131">注意： 这适用于工作/学校仅帐户。</span><span class="sxs-lookup"><span data-stu-id="56f1d-131">Note: This applies to work/school accounts only.</span></span>| <span data-ttu-id="56f1d-132">创建**此**应用程序本身或目录中的任何用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-132">Subscriptions created by **this app** for itself or for any user in the directory.</span></span>|

### <a name="advanced-scenarios"></a><span data-ttu-id="56f1d-133">高级的方案</span><span class="sxs-lookup"><span data-stu-id="56f1d-133">Advanced scenarios</span></span>

<span data-ttu-id="56f1d-134">在某些情况下，希望检索订阅创建其他应用程序的应用程序。</span><span class="sxs-lookup"><span data-stu-id="56f1d-134">In some cases, an app wants to retrieve subscriptions created by other apps.</span></span> <span data-ttu-id="56f1d-135">例如，用户想要查看由其代表任何应用程序创建的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-135">For example, a user wants to see all subscriptions created by any app on their behalf.</span></span> <span data-ttu-id="56f1d-136">或者，管理员可能希望查看其目录中的所有应用程序中的所有订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-136">Or, an administrator may want to see all subscriptions from all apps in their directory.</span></span>
<span data-ttu-id="56f1d-137">如果是这种情况下，对于需要委派的权限 Subscription.Read.All。</span><span class="sxs-lookup"><span data-stu-id="56f1d-137">For such scenarios, a delegated permission Subscription.Read.All is required.</span></span>

| <span data-ttu-id="56f1d-138">调用应用程序的上下文</span><span class="sxs-lookup"><span data-stu-id="56f1d-138">Context of the calling app</span></span> | <span data-ttu-id="56f1d-139">响应中包含</span><span class="sxs-lookup"><span data-stu-id="56f1d-139">Response contains</span></span> |
|:-----|:---------------- |
| <span data-ttu-id="56f1d-140">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="56f1d-140">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="56f1d-141">*用户在处于非管理员*。</span><span class="sxs-lookup"><span data-stu-id="56f1d-141">*The user is a non-admin*.</span></span> <br/><span data-ttu-id="56f1d-142">And</span><span class="sxs-lookup"><span data-stu-id="56f1d-142">-and-</span></span><br/><span data-ttu-id="56f1d-143">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="56f1d-143">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="56f1d-144">注意： 这适用于个人 Microsoft 帐户和工作/学校帐户。</span><span class="sxs-lookup"><span data-stu-id="56f1d-144">Note: This applies to both personal Microsoft accounts and work/school accounts.</span></span> | <span data-ttu-id="56f1d-145">创建的**任何应用程序**的已登录的用户的订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-145">Subscriptions created by **any app** for the signed-in user only.</span></span> |
| <span data-ttu-id="56f1d-146">应用程序代表登录用户 （委派权限） 调用。</span><span class="sxs-lookup"><span data-stu-id="56f1d-146">App is calling on behalf of the signed-in user (delegated permission).</span></span> <span data-ttu-id="56f1d-147">*用户是管理员*。</span><span class="sxs-lookup"><span data-stu-id="56f1d-147">*The user is an admin*.</span></span><br/><span data-ttu-id="56f1d-148">And</span><span class="sxs-lookup"><span data-stu-id="56f1d-148">-and-</span></span><br/><span data-ttu-id="56f1d-149">应用程序具有权限 Subscription.Read.All</span><span class="sxs-lookup"><span data-stu-id="56f1d-149">App has the permission Subscription.Read.All</span></span><br/><br/><span data-ttu-id="56f1d-150">注意： 这适用于工作/学校仅帐户。</span><span class="sxs-lookup"><span data-stu-id="56f1d-150">Note: This applies to work/school accounts only.</span></span> | <span data-ttu-id="56f1d-151">创建的**任何应用程序**目录中的**任何用户**的订阅。</span><span class="sxs-lookup"><span data-stu-id="56f1d-151">Subscriptions created by **any app** for **any user** in the directory.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56f1d-152">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="56f1d-152">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /subscriptions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="56f1d-153">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="56f1d-153">Optional query parameters</span></span>

<span data-ttu-id="56f1d-154">此方法不支持的[OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)以帮助自定义的响应。</span><span class="sxs-lookup"><span data-stu-id="56f1d-154">This method does not support the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="56f1d-155">请求标头</span><span class="sxs-lookup"><span data-stu-id="56f1d-155">Request headers</span></span>

| <span data-ttu-id="56f1d-156">名称</span><span class="sxs-lookup"><span data-stu-id="56f1d-156">Name</span></span>       | <span data-ttu-id="56f1d-157">类型</span><span class="sxs-lookup"><span data-stu-id="56f1d-157">Type</span></span> | <span data-ttu-id="56f1d-158">说明</span><span class="sxs-lookup"><span data-stu-id="56f1d-158">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="56f1d-159">Authorization</span><span class="sxs-lookup"><span data-stu-id="56f1d-159">Authorization</span></span>  | <span data-ttu-id="56f1d-160">string</span><span class="sxs-lookup"><span data-stu-id="56f1d-160">string</span></span>  | <span data-ttu-id="56f1d-p107">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="56f1d-p107">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="56f1d-163">请求正文</span><span class="sxs-lookup"><span data-stu-id="56f1d-163">Request body</span></span>

<span data-ttu-id="56f1d-164">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="56f1d-164">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="56f1d-165">响应</span><span class="sxs-lookup"><span data-stu-id="56f1d-165">Response</span></span>

<span data-ttu-id="56f1d-166">如果成功，此方法返回`200 OK`响应代码和响应正文中的[订阅](../resources/subscription.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="56f1d-166">If successful, this method returns a `200 OK` response code and a list of [subscription](../resources/subscription.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="56f1d-167">示例</span><span class="sxs-lookup"><span data-stu-id="56f1d-167">Example</span></span>

##### <a name="request"></a><span data-ttu-id="56f1d-168">请求</span><span class="sxs-lookup"><span data-stu-id="56f1d-168">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_subscriptions"
}-->

```http
GET https://graph.microsoft.com/beta/subscriptions
```

##### <a name="response"></a><span data-ttu-id="56f1d-169">响应</span><span class="sxs-lookup"><span data-stu-id="56f1d-169">Response</span></span>

<span data-ttu-id="56f1d-170">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="56f1d-170">Here is an example of the response.</span></span> <span data-ttu-id="56f1d-171">注意： 为了简单起见，如下所示的响应可能被截断。</span><span class="sxs-lookup"><span data-stu-id="56f1d-171">Note: The response shown here may be truncated for brevity.</span></span> <span data-ttu-id="56f1d-172">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="56f1d-172">All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List subscriptions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/subscription-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->

<span data-ttu-id="56f1d-173">请求返回的数据的多个页面，响应中包括`@odata.nextLink`属性可帮助您管理结果。</span><span class="sxs-lookup"><span data-stu-id="56f1d-173">When a request returns multiple pages of data, the response includes an `@odata.nextLink` property to help you manage the results.</span></span>  <span data-ttu-id="56f1d-174">若要了解详细信息，请参阅[分页 Microsoft Graph 应用程序中的数据](/graph/paging)。</span><span class="sxs-lookup"><span data-stu-id="56f1d-174">To learn more, see [Paging Microsoft Graph data in your app](/graph/paging).</span></span>
