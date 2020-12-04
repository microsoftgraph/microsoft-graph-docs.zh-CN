---
title: 发布 teamsapp
description: 将应用程序发布到 Microsoft 团队应用程序目录。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9e8579bb2da482e18d2524c82bee985b9eb8ae39
ms.sourcegitcommit: c419bb8901b7766af193196f80bc1d497643fcb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49572182"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="5a83f-103">发布 teamsApp</span><span class="sxs-lookup"><span data-stu-id="5a83f-103">Publish teamsApp</span></span>

<span data-ttu-id="5a83f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5a83f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5a83f-105">将 [应用程序](../resources/teamsapp.md) 发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="5a83f-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="5a83f-106">具体而言，此 API 会将应用程序发布到 (租户应用程序目录) 的组织目录中。创建的资源的 **distributionMethod** 属性值为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="5a83f-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="5a83f-107">**RequiresReview** 属性允许任何用户提交由管理员审阅的应用程序。</span><span class="sxs-lookup"><span data-stu-id="5a83f-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="5a83f-108">管理员可以通过此 API 或 Microsoft 团队管理中心批准或拒绝这些应用。</span><span class="sxs-lookup"><span data-stu-id="5a83f-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="5a83f-109">权限</span><span class="sxs-lookup"><span data-stu-id="5a83f-109">Permissions</span></span>

<span data-ttu-id="5a83f-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5a83f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5a83f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5a83f-112">Permission Type</span></span>                        | <span data-ttu-id="5a83f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5a83f-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="5a83f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5a83f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5a83f-115">AppCatalog、AppCatalog、all 和所有目录。</span><span class="sxs-lookup"><span data-stu-id="5a83f-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="5a83f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5a83f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5a83f-117">不支持</span><span class="sxs-lookup"><span data-stu-id="5a83f-117">Not supported</span></span>|
| <span data-ttu-id="5a83f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5a83f-118">Application</span></span>                            | <span data-ttu-id="5a83f-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5a83f-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5a83f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5a83f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="5a83f-121">若要发布需要评审的应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="5a83f-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="5a83f-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="5a83f-122">Query parameters</span></span>

|<span data-ttu-id="5a83f-123">属性</span><span class="sxs-lookup"><span data-stu-id="5a83f-123">Property</span></span>|<span data-ttu-id="5a83f-124">类型</span><span class="sxs-lookup"><span data-stu-id="5a83f-124">Type</span></span>|<span data-ttu-id="5a83f-125">说明</span><span class="sxs-lookup"><span data-stu-id="5a83f-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="5a83f-126">requiresReview</span><span class="sxs-lookup"><span data-stu-id="5a83f-126">requiresReview</span></span>| <span data-ttu-id="5a83f-127">布尔值</span><span class="sxs-lookup"><span data-stu-id="5a83f-127">Boolean</span></span> | <span data-ttu-id="5a83f-128">此可选查询参数触发应用程序审阅过程。</span><span class="sxs-lookup"><span data-stu-id="5a83f-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="5a83f-129">具有管理员权限的用户无需触发评审即可提交应用程序。</span><span class="sxs-lookup"><span data-stu-id="5a83f-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="5a83f-130">如果用户希望在发布之前请求审阅，则必须将其设置  `requiresReview` 为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="5a83f-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="5a83f-131">具有管理员权限的用户可以选择不设置 `requiresReview` 或设置值 `false`  ，并且应用将被视为 "已批准"，并将立即发布。</span><span class="sxs-lookup"><span data-stu-id="5a83f-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5a83f-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="5a83f-132">Request headers</span></span>

| <span data-ttu-id="5a83f-133">标头</span><span class="sxs-lookup"><span data-stu-id="5a83f-133">Header</span></span>        | <span data-ttu-id="5a83f-134">值</span><span class="sxs-lookup"><span data-stu-id="5a83f-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="5a83f-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5a83f-135">Authorization</span></span> | <span data-ttu-id="5a83f-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5a83f-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5a83f-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5a83f-138">Content-Type</span></span>  | <span data-ttu-id="5a83f-139">application/zip。</span><span class="sxs-lookup"><span data-stu-id="5a83f-139">application/zip.</span></span> <span data-ttu-id="5a83f-140">必需。</span><span class="sxs-lookup"><span data-stu-id="5a83f-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5a83f-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="5a83f-141">Request body</span></span>

<span data-ttu-id="5a83f-142">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="5a83f-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="5a83f-143">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="5a83f-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="5a83f-144">应用程序目录中的每个应用程序都必须有一个唯一的清单 `id` 。</span><span class="sxs-lookup"><span data-stu-id="5a83f-144">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="5a83f-145">响应</span><span class="sxs-lookup"><span data-stu-id="5a83f-145">Response</span></span>

<span data-ttu-id="5a83f-146">如果成功，此方法将返回 `200 OK` 响应代码和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5a83f-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="5a83f-147">示例</span><span class="sxs-lookup"><span data-stu-id="5a83f-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="5a83f-148">示例1：将应用程序发布到应用程序目录</span><span class="sxs-lookup"><span data-stu-id="5a83f-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="5a83f-149">请求</span><span class="sxs-lookup"><span data-stu-id="5a83f-149">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a83f-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a83f-150">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

# <a name="javascript"></a>[<span data-ttu-id="5a83f-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a83f-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a83f-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a83f-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="5a83f-153">有关如何创建 Microsoft 团队应用程序 zip 文件的信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="5a83f-153">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="5a83f-154">响应</span><span class="sxs-lookup"><span data-stu-id="5a83f-154">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="5a83f-155">示例2：将要审阅的新应用程序上载到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="5a83f-155">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="5a83f-156">请求</span><span class="sxs-lookup"><span data-stu-id="5a83f-156">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5a83f-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="5a83f-157">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

# <a name="javascript"></a>[<span data-ttu-id="5a83f-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5a83f-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5a83f-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5a83f-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="5a83f-160">响应</span><span class="sxs-lookup"><span data-stu-id="5a83f-160">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps/$entity",
  "id": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
  "externalId": "b5561ec9-8cab-4aa3-8aa2-d8d7172e4311",
  "name": "Test App",
  "version": "1.0.0",
  "distributionMethod": "organization"
}
```

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="5a83f-161">示例3：批准或拒绝正在等待审阅的应用程序</span><span class="sxs-lookup"><span data-stu-id="5a83f-161">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="5a83f-162">请求</span><span class="sxs-lookup"><span data-stu-id="5a83f-162">Request</span></span>

<span data-ttu-id="5a83f-163">**HTTP**</span><span class="sxs-lookup"><span data-stu-id="5a83f-163">**HTTP**</span></span>
<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
PATCH https://graph.microsoft.com/beta/appCatalogs/teamsApps/a761ad07-22ef-4a53-9feb-2837c8ad4a84/appDefinitions/YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjU3VibWl0dGVk
Content-type: application/json
If-Match: InFtSStsNVJHVWdzWUJRU2ZVWGp4RWc9PSI=

{
  "publishingState":"published"
}
```

---

#### <a name="response"></a><span data-ttu-id="5a83f-164">响应</span><span class="sxs-lookup"><span data-stu-id="5a83f-164">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appCatalogs/teamsApps('a761ad07-22ef-4a53-9feb-2837c8ad4a84')/appDefinitions/$entity",
    "id": "YTc2MWFkMDctMjJlZi00YTUzLTlmZWItMjgzN2M4YWQ0YTg0IyMxLjEuOCMjUHVibGlzaGVk",
    "teamsAppId": "a761ad07-22ef-4a53-9feb-2837c8ad4a84",
    "azureADAppId": null,
    "displayName": "Ducks",
    "version": "1.1.8",
    "requiredResourceSpecificApplicationPermissions": [],
    "publishingState": "published",
    "shortdescription": "quaerat quasi magnam. slight change. 5",
    "description": "Aliquid placeat animi debitis accusamus. Non perferendis ullam. Quis est consequuntur vitae provident. Sunt laudantium id aut. slight change 5",
    "lastModifiedDateTime": null,
    "createdBy": null
}
```
