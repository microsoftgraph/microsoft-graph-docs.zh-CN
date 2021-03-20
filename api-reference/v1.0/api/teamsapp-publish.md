---
title: 发布 teamsapp
description: '将应用发布到 Microsoft Teams 应用目录。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1d746d4733301d8fcace84a0dba82a9a7234f320
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50948673"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="6c0b1-103">发布 teamsapp</span><span class="sxs-lookup"><span data-stu-id="6c0b1-103">Publish teamsapp</span></span>

<span data-ttu-id="6c0b1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c0b1-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6c0b1-105">将 [应用发布到](../resources/teamsapp.md) Microsoft Teams 应用目录。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="6c0b1-106">具体而言，此 API 将应用程序发布到组织的目录 (租户应用程序目录) ;创建的资源将 **具有 的 distributionMethod** 属性值 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="6c0b1-107">**requiresReview** 属性允许任何用户提交应用供管理员审阅。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="6c0b1-108">管理员可以通过此 API 或 Microsoft Teams 管理中心批准或拒绝这些应用。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="6c0b1-109">权限</span><span class="sxs-lookup"><span data-stu-id="6c0b1-109">Permissions</span></span>

<span data-ttu-id="6c0b1-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6c0b1-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c0b1-112">Permission Type</span></span>                        | <span data-ttu-id="6c0b1-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c0b1-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="6c0b1-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c0b1-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6c0b1-115">AppCatalog.Submit、AppCatalog.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c0b1-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="6c0b1-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c0b1-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6c0b1-117">不支持</span><span class="sxs-lookup"><span data-stu-id="6c0b1-117">Not supported</span></span>|
| <span data-ttu-id="6c0b1-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c0b1-118">Application</span></span>                            | <span data-ttu-id="6c0b1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6c0b1-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c0b1-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="6c0b1-121">若要发布需要审阅的应用：</span><span class="sxs-lookup"><span data-stu-id="6c0b1-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="6c0b1-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="6c0b1-122">Query parameters</span></span>

|<span data-ttu-id="6c0b1-123">属性</span><span class="sxs-lookup"><span data-stu-id="6c0b1-123">Property</span></span>|<span data-ttu-id="6c0b1-124">类型</span><span class="sxs-lookup"><span data-stu-id="6c0b1-124">Type</span></span>|<span data-ttu-id="6c0b1-125">说明</span><span class="sxs-lookup"><span data-stu-id="6c0b1-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="6c0b1-126">requiresReview</span><span class="sxs-lookup"><span data-stu-id="6c0b1-126">requiresReview</span></span>| <span data-ttu-id="6c0b1-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="6c0b1-127">Boolean</span></span> | <span data-ttu-id="6c0b1-128">此可选查询参数将触发应用评审过程。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="6c0b1-129">具有管理员权限的用户无需触发审查即可提交应用。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="6c0b1-130">如果用户想要在发布之前请求审阅，则必须将 设置为  `requiresReview` `true` 。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="6c0b1-131">具有管理员权限的用户可以选择不设置或将值设置为 ，应用将被视为已批准， `requiresReview` `false`  并且将立即发布。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="6c0b1-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c0b1-132">Request headers</span></span>

| <span data-ttu-id="6c0b1-133">标头</span><span class="sxs-lookup"><span data-stu-id="6c0b1-133">Header</span></span>        | <span data-ttu-id="6c0b1-134">值</span><span class="sxs-lookup"><span data-stu-id="6c0b1-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6c0b1-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c0b1-135">Authorization</span></span> | <span data-ttu-id="6c0b1-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6c0b1-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6c0b1-138">Content-Type</span></span>  | <span data-ttu-id="6c0b1-139">application/zip。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-139">application/zip.</span></span> <span data-ttu-id="6c0b1-140">必填。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6c0b1-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c0b1-141">Request body</span></span>

<span data-ttu-id="6c0b1-142">在请求正文中，包括 Teams zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="6c0b1-143">有关详细信息，请参阅 [创建应用包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="6c0b1-144">应用程序目录中的每个应用程序必须具有唯一的清单 ID。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-144">Each app in the app catalog must have a unique manifest ID.</span></span>

## <a name="response"></a><span data-ttu-id="6c0b1-145">响应</span><span class="sxs-lookup"><span data-stu-id="6c0b1-145">Response</span></span>

<span data-ttu-id="6c0b1-146">如果成功，此方法返回 响应 `200 OK` 代码和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="6c0b1-147">示例</span><span class="sxs-lookup"><span data-stu-id="6c0b1-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="6c0b1-148">示例 1：将应用程序发布到应用程序目录</span><span class="sxs-lookup"><span data-stu-id="6c0b1-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="6c0b1-149">请求</span><span class="sxs-lookup"><span data-stu-id="6c0b1-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c0b1-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c0b1-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp_1"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[<span data-ttu-id="6c0b1-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c0b1-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---
<span data-ttu-id="6c0b1-152">若要了解如何创建 Microsoft Teams 应用程序 zip 文件，请参阅 [创建应用包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="6c0b1-152">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="6c0b1-153">响应</span><span class="sxs-lookup"><span data-stu-id="6c0b1-153">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="6c0b1-154">示例 2：将新应用程序上载到组织的应用程序目录进行审阅</span><span class="sxs-lookup"><span data-stu-id="6c0b1-154">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="6c0b1-155">请求</span><span class="sxs-lookup"><span data-stu-id="6c0b1-155">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6c0b1-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="6c0b1-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp_2"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```
# <a name="javascript"></a>[<span data-ttu-id="6c0b1-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6c0b1-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6c0b1-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6c0b1-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


---

#### <a name="response"></a><span data-ttu-id="6c0b1-159">响应</span><span class="sxs-lookup"><span data-stu-id="6c0b1-159">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="6c0b1-160">示例 3：批准或拒绝应用待审阅</span><span class="sxs-lookup"><span data-stu-id="6c0b1-160">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="6c0b1-161">请求</span><span class="sxs-lookup"><span data-stu-id="6c0b1-161">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp_3"
}-->

```http
PATCH https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
  "publishingState":"published"
}
```

---

#### <a name="response"></a><span data-ttu-id="6c0b1-162">响应</span><span class="sxs-lookup"><span data-stu-id="6c0b1-162">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortDescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```
