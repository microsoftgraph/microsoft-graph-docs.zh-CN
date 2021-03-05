---
title: 发布 teamsapp
description: '将应用发布到 Microsoft Teams 应用目录。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 1984ed7226da71ba1baf1bf15a7d83df4e6609a0
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471647"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="5d0e7-103">发布 teamsapp</span><span class="sxs-lookup"><span data-stu-id="5d0e7-103">Publish teamsapp</span></span>

<span data-ttu-id="5d0e7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d0e7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5d0e7-105">将 [应用发布到](../resources/teamsapp.md) Microsoft Teams 应用目录。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="5d0e7-106">具体而言，此 API 将应用发布到组织的目录 (租户应用程序目录) ;创建的资源的 **distributionMethod** 属性值为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

<span data-ttu-id="5d0e7-107">**requiresReview** 属性允许任何用户提交应用供管理员审阅。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-107">The **requiresReview** property allows any user to submit an app for review by an administrator.</span></span> <span data-ttu-id="5d0e7-108">管理员可以通过此 API 或 Microsoft Teams 管理中心批准或拒绝这些应用。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-108">Admins can approve or reject these apps via this API or the Microsoft Teams admin center.</span></span>

## <a name="permissions"></a><span data-ttu-id="5d0e7-109">权限</span><span class="sxs-lookup"><span data-stu-id="5d0e7-109">Permissions</span></span>

<span data-ttu-id="5d0e7-p103">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5d0e7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="5d0e7-112">Permission Type</span></span>                        | <span data-ttu-id="5d0e7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5d0e7-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="5d0e7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5d0e7-114">Delegated (work or school account)</span></span> | <span data-ttu-id="5d0e7-115">AppCatalog.Submit、AppCatalog.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5d0e7-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="5d0e7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5d0e7-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5d0e7-117">不支持</span><span class="sxs-lookup"><span data-stu-id="5d0e7-117">Not supported</span></span>|
| <span data-ttu-id="5d0e7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="5d0e7-118">Application</span></span>                            | <span data-ttu-id="5d0e7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5d0e7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5d0e7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="5d0e7-121">若要发布需要审阅的应用：</span><span class="sxs-lookup"><span data-stu-id="5d0e7-121">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="5d0e7-122">查询参数</span><span class="sxs-lookup"><span data-stu-id="5d0e7-122">Query parameters</span></span>

|<span data-ttu-id="5d0e7-123">属性</span><span class="sxs-lookup"><span data-stu-id="5d0e7-123">Property</span></span>|<span data-ttu-id="5d0e7-124">类型</span><span class="sxs-lookup"><span data-stu-id="5d0e7-124">Type</span></span>|<span data-ttu-id="5d0e7-125">说明</span><span class="sxs-lookup"><span data-stu-id="5d0e7-125">Description</span></span>|
|----|----|----|
|<span data-ttu-id="5d0e7-126">requiresReview</span><span class="sxs-lookup"><span data-stu-id="5d0e7-126">requiresReview</span></span>| <span data-ttu-id="5d0e7-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="5d0e7-127">Boolean</span></span> | <span data-ttu-id="5d0e7-128">此可选查询参数触发应用审阅过程。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-128">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="5d0e7-129">具有管理员权限的用户无需触发评价即可提交应用。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-129">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="5d0e7-130">如果用户想要在发布之前请求审阅，则必须设置为  `requiresReview` `true` 。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-130">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="5d0e7-131">具有管理员权限的用户可以选择不设置或设置值，并且应用将被视为已批准 `requiresReview` `false`  ，并且将立即发布。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-131">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="5d0e7-132">请求标头</span><span class="sxs-lookup"><span data-stu-id="5d0e7-132">Request headers</span></span>

| <span data-ttu-id="5d0e7-133">标头</span><span class="sxs-lookup"><span data-stu-id="5d0e7-133">Header</span></span>        | <span data-ttu-id="5d0e7-134">值</span><span class="sxs-lookup"><span data-stu-id="5d0e7-134">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="5d0e7-135">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d0e7-135">Authorization</span></span> | <span data-ttu-id="5d0e7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="5d0e7-138">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5d0e7-138">Content-Type</span></span>  | <span data-ttu-id="5d0e7-139">application/zip。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-139">application/zip.</span></span> <span data-ttu-id="5d0e7-140">必填。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-140">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5d0e7-141">请求正文</span><span class="sxs-lookup"><span data-stu-id="5d0e7-141">Request body</span></span>

<span data-ttu-id="5d0e7-142">在请求正文中，包括 Teams zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-142">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="5d0e7-143">有关详细信息，请参阅["创建应用包"。](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="5d0e7-143">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="5d0e7-144">应用程序目录中的每个应用必须具有唯一的清单 ID。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-144">Each app in the app catalog must have a unique manifest ID.</span></span>

## <a name="response"></a><span data-ttu-id="5d0e7-145">响应</span><span class="sxs-lookup"><span data-stu-id="5d0e7-145">Response</span></span>

<span data-ttu-id="5d0e7-146">如果成功，此方法将返回 `200 OK` 响应代码和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5d0e7-146">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="5d0e7-147">示例</span><span class="sxs-lookup"><span data-stu-id="5d0e7-147">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="5d0e7-148">示例 1：将应用发布到应用程序目录</span><span class="sxs-lookup"><span data-stu-id="5d0e7-148">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="5d0e7-149">请求</span><span class="sxs-lookup"><span data-stu-id="5d0e7-149">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

---
<span data-ttu-id="5d0e7-150">若要了解如何创建 Microsoft Teams 应用程序 zip 文件，请参阅["创建应用包"。](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="5d0e7-150">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="5d0e7-151">响应</span><span class="sxs-lookup"><span data-stu-id="5d0e7-151">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="5d0e7-152">示例 2：将新应用程序上载到组织的应用程序目录进行审阅</span><span class="sxs-lookup"><span data-stu-id="5d0e7-152">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="5d0e7-153">请求</span><span class="sxs-lookup"><span data-stu-id="5d0e7-153">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

---

#### <a name="response"></a><span data-ttu-id="5d0e7-154">响应</span><span class="sxs-lookup"><span data-stu-id="5d0e7-154">Response</span></span>

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

### <a name="example-3-approve-or-reject-an-app-pending-review"></a><span data-ttu-id="5d0e7-155">示例 3：批准或拒绝等待审阅的应用</span><span class="sxs-lookup"><span data-stu-id="5d0e7-155">Example 3: Approve or reject an app pending review</span></span>

#### <a name="request"></a><span data-ttu-id="5d0e7-156">请求</span><span class="sxs-lookup"><span data-stu-id="5d0e7-156">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
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

#### <a name="response"></a><span data-ttu-id="5d0e7-157">响应</span><span class="sxs-lookup"><span data-stu-id="5d0e7-157">Response</span></span>

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