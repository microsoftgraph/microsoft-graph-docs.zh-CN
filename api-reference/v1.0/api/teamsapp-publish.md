---
title: 发布 teamsapp
description: '将应用程序发布到 Microsoft 团队应用程序目录。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 8a993178cc6735449fc5ce14a8c6d5663d9e9003
ms.sourcegitcommit: dc3bade0c096d5ce716d4bc07cd9c7cabb52477b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/18/2020
ms.locfileid: "46792371"
---
# <a name="publish-teamsapp"></a><span data-ttu-id="c990a-103">发布 teamsapp</span><span class="sxs-lookup"><span data-stu-id="c990a-103">Publish teamsapp</span></span>

<span data-ttu-id="c990a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c990a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c990a-105">将 [应用程序](../resources/teamsapp.md) 发布到 Microsoft 团队应用程序目录。</span><span class="sxs-lookup"><span data-stu-id="c990a-105">Publish an [app](../resources/teamsapp.md) to the Microsoft Teams apps catalog.</span></span>
<span data-ttu-id="c990a-106">具体而言，此 API 会将应用程序发布到 (租户应用程序目录) 的组织目录中。创建的资源的 **distributionMethod** 属性值为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="c990a-106">Specifically, this API publishes the app to your organization's catalog (the tenant app catalog); the created resource will have a **distributionMethod** property value of `organization`.</span></span>

## <a name="permissions"></a><span data-ttu-id="c990a-107">权限</span><span class="sxs-lookup"><span data-stu-id="c990a-107">Permissions</span></span>

<span data-ttu-id="c990a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="c990a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="c990a-110">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c990a-110">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="c990a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c990a-111">Permission Type</span></span>                        | <span data-ttu-id="c990a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c990a-112">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="c990a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c990a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="c990a-114">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="c990a-114">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c990a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c990a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c990a-116">不支持</span><span class="sxs-lookup"><span data-stu-id="c990a-116">Not supported</span></span>|
| <span data-ttu-id="c990a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c990a-117">Application</span></span>                            | <span data-ttu-id="c990a-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c990a-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c990a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c990a-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /appCatalogs/teamsApps
```
<span data-ttu-id="c990a-120">若要发布需要评审的应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c990a-120">To publish an app that requires a review:</span></span>

```http
POST /appCatalogs/teamsApps?requiresReview:{Boolean}
```

## <a name="query-parameters"></a><span data-ttu-id="c990a-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="c990a-121">Query parameters</span></span>

|<span data-ttu-id="c990a-122">属性</span><span class="sxs-lookup"><span data-stu-id="c990a-122">Property</span></span>|<span data-ttu-id="c990a-123">类型</span><span class="sxs-lookup"><span data-stu-id="c990a-123">Type</span></span>|<span data-ttu-id="c990a-124">说明</span><span class="sxs-lookup"><span data-stu-id="c990a-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="c990a-125">requiresReview</span><span class="sxs-lookup"><span data-stu-id="c990a-125">requiresReview</span></span>| <span data-ttu-id="c990a-126">布尔值</span><span class="sxs-lookup"><span data-stu-id="c990a-126">Boolean</span></span> | <span data-ttu-id="c990a-127">此可选查询参数触发应用程序审阅过程。</span><span class="sxs-lookup"><span data-stu-id="c990a-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="c990a-128">具有管理员权限的用户无需触发评审即可提交应用程序。</span><span class="sxs-lookup"><span data-stu-id="c990a-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="c990a-129">如果用户希望在发布之前请求审阅，则必须将其设置  `requiresReview` 为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="c990a-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="c990a-130">具有管理员权限的用户可以选择不设置 `requiresReview` 或设置值 `false`  ，并且应用将被视为 "已批准"，并将立即发布。</span><span class="sxs-lookup"><span data-stu-id="c990a-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="c990a-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="c990a-131">Request headers</span></span>

| <span data-ttu-id="c990a-132">标头</span><span class="sxs-lookup"><span data-stu-id="c990a-132">Header</span></span>        | <span data-ttu-id="c990a-133">值</span><span class="sxs-lookup"><span data-stu-id="c990a-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="c990a-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="c990a-134">Authorization</span></span> | <span data-ttu-id="c990a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c990a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c990a-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c990a-137">Content-Type</span></span>  | <span data-ttu-id="c990a-138">application/zip。</span><span class="sxs-lookup"><span data-stu-id="c990a-138">application/zip.</span></span> <span data-ttu-id="c990a-139">必需。</span><span class="sxs-lookup"><span data-stu-id="c990a-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c990a-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="c990a-140">Request body</span></span>

<span data-ttu-id="c990a-141">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="c990a-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="c990a-142">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="c990a-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

<span data-ttu-id="c990a-143">应用程序目录中的每个应用必须具有唯一的清单 id。</span><span class="sxs-lookup"><span data-stu-id="c990a-143">Each app in the app catalog must have a unique manifest id.</span></span>

## <a name="response"></a><span data-ttu-id="c990a-144">响应</span><span class="sxs-lookup"><span data-stu-id="c990a-144">Response</span></span>

<span data-ttu-id="c990a-145">如果成功，此方法将返回 `200 OK` 响应代码和 [teamsApp](../resources/teamsapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c990a-145">If successful, this method returns a `200 OK` response code and a [teamsApp](../resources/teamsapp.md) object.</span></span>

## <a name="examples"></a><span data-ttu-id="c990a-146">示例</span><span class="sxs-lookup"><span data-stu-id="c990a-146">Examples</span></span>

### <a name="example-1-publish-an-app-to-the-app-catalog"></a><span data-ttu-id="c990a-147">示例1：将应用程序发布到应用程序目录</span><span class="sxs-lookup"><span data-stu-id="c990a-147">Example 1: Publish an app to the app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="c990a-148">请求</span><span class="sxs-lookup"><span data-stu-id="c990a-148">Request</span></span>

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="c990a-149">有关如何创建 Microsoft 团队应用程序 zip 文件的信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="c990a-149">For information about how to create a Microsoft Teams application zip file, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

#### <a name="response"></a><span data-ttu-id="c990a-150">响应</span><span class="sxs-lookup"><span data-stu-id="c990a-150">Response</span></span>

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
### <a name="example-2-upload-a-new-application-for-review-to-an-organizations-app-catalog"></a><span data-ttu-id="c990a-151">示例2：将要审阅的新应用程序上载到组织的应用程序目录</span><span class="sxs-lookup"><span data-stu-id="c990a-151">Example 2: Upload a new application for review to an organization's app catalog</span></span>

#### <a name="request"></a><span data-ttu-id="c990a-152">请求</span><span class="sxs-lookup"><span data-stu-id="c990a-152">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_teamsapp"
}-->

```http
POST https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?requiresReview=true
Content-type: application/zip
Content-length: 244
```

#### <a name="response"></a><span data-ttu-id="c990a-153">响应</span><span class="sxs-lookup"><span data-stu-id="c990a-153">Response</span></span>

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
