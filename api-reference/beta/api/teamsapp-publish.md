---
title: 发布 teamsapp
description: 将应用程序发布到 Microsoft 团队应用程序目录。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 92c90df5035ffa26b4a592ff8cc6d2749048308d
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076636"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="99da1-103">发布 teamsApp</span><span class="sxs-lookup"><span data-stu-id="99da1-103">Publish teamsApp</span></span>

<span data-ttu-id="99da1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99da1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99da1-105">将 [应用程序](../resources/teamsapp.md) 发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="99da1-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="99da1-106">具体而言，此 API 会将应用程序发布到 (租户应用程序目录) 的组织目录中。创建的资源的 **distributionMethod** 属性值为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="99da1-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="99da1-107">权限</span><span class="sxs-lookup"><span data-stu-id="99da1-107">Permissions</span></span>

<span data-ttu-id="99da1-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="99da1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="99da1-110">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="99da1-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="99da1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99da1-111">Permission Type</span></span>                        | <span data-ttu-id="99da1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99da1-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="99da1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99da1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="99da1-114">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="99da1-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="99da1-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99da1-115">Delegated (work or school account)</span></span> | <span data-ttu-id="99da1-116">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="99da1-116">AppCatalog.Submit</span></span>|
| <span data-ttu-id="99da1-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99da1-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99da1-118">不支持</span><span class="sxs-lookup"><span data-stu-id="99da1-118">Not supported</span></span>|
| <span data-ttu-id="99da1-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="99da1-119">Application</span></span>                            | <span data-ttu-id="99da1-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="99da1-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="99da1-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99da1-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps
```

<span data-ttu-id="99da1-122">若要发布需要评审的应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="99da1-122">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="99da1-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="99da1-123">Query parameters</span></span>

|<span data-ttu-id="99da1-124">属性</span><span class="sxs-lookup"><span data-stu-id="99da1-124">Property</span></span>|<span data-ttu-id="99da1-125">类型</span><span class="sxs-lookup"><span data-stu-id="99da1-125">Type</span></span>|<span data-ttu-id="99da1-126">说明</span><span class="sxs-lookup"><span data-stu-id="99da1-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="99da1-127">requiresReview</span><span class="sxs-lookup"><span data-stu-id="99da1-127">requiresReview</span></span>| <span data-ttu-id="99da1-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="99da1-128">Boolean</span></span> | <span data-ttu-id="99da1-129">此可选查询参数触发应用程序审阅过程。</span><span class="sxs-lookup"><span data-stu-id="99da1-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="99da1-130">具有管理员权限的用户无需触发评审即可提交应用程序。</span><span class="sxs-lookup"><span data-stu-id="99da1-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="99da1-131">如果用户希望在发布之前请求审阅，则必须将其设置  `requiresReview` 为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="99da1-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="99da1-132">具有管理员权限的用户可以选择不设置 `requiresReview` 或设置值 `false`  ，并且应用将被视为 "已批准"，并将立即发布。</span><span class="sxs-lookup"><span data-stu-id="99da1-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="99da1-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="99da1-133">Request headers</span></span>

| <span data-ttu-id="99da1-134">标头</span><span class="sxs-lookup"><span data-stu-id="99da1-134">Header</span></span>        | <span data-ttu-id="99da1-135">值</span><span class="sxs-lookup"><span data-stu-id="99da1-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="99da1-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="99da1-136">Authorization</span></span> | <span data-ttu-id="99da1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="99da1-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="99da1-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="99da1-139">Content-Type</span></span>  | <span data-ttu-id="99da1-140">application/zip。</span><span class="sxs-lookup"><span data-stu-id="99da1-140">application/zip.</span></span> <span data-ttu-id="99da1-141">必需。</span><span class="sxs-lookup"><span data-stu-id="99da1-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="99da1-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="99da1-142">Request body</span></span>

<span data-ttu-id="99da1-143">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="99da1-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="99da1-144">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="99da1-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>  

<span data-ttu-id="99da1-145">应用程序目录中的每个应用程序都必须有一个唯一的清单 `id` 。</span><span class="sxs-lookup"><span data-stu-id="99da1-145">Each app in the app catalog must have a unique manifest `id`.</span></span>

## <a name="response"></a><span data-ttu-id="99da1-146">响应</span><span class="sxs-lookup"><span data-stu-id="99da1-146">Response</span></span>

<span data-ttu-id="99da1-147">如果成功，此方法将返回 `200 OK` 响应代码和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99da1-147">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="99da1-148">示例</span><span class="sxs-lookup"><span data-stu-id="99da1-148">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="99da1-149">示例1：将应用程序发布到应用程序目录</span><span class="sxs-lookup"><span data-stu-id="99da1-149">Example 1: Publish an app to the app catalog</span></span>
#### <a name="request"></a><span data-ttu-id="99da1-150">请求</span><span class="sxs-lookup"><span data-stu-id="99da1-150">Request</span></span>

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

<span data-ttu-id="99da1-151">有关如何创建 Microsoft 团队应用程序 zip 文件的信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="99da1-151">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->
#### <a name="response"></a><span data-ttu-id="99da1-152">响应</span><span class="sxs-lookup"><span data-stu-id="99da1-152">Response</span></span>

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

### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="99da1-153">示例2：将要审阅的新应用程序上载到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="99da1-153">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="99da1-154">请求</span><span class="sxs-lookup"><span data-stu-id="99da1-154">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

#### <a name="response"></a><span data-ttu-id="99da1-155">响应</span><span class="sxs-lookup"><span data-stu-id="99da1-155">Response</span></span>

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


