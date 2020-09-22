---
title: 更新 teamsApp
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e47ca7c35ddd535ec9809039cc57c4be670ef85a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48076615"
---
# <a name="update-teamsapp"></a><span data-ttu-id="7f1e8-103">更新 teamsApp</span><span class="sxs-lookup"><span data-stu-id="7f1e8-103">Update teamsApp</span></span>

<span data-ttu-id="7f1e8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f1e8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f1e8-105">更新之前发布到 Microsoft 团队应用程序目录的 [应用程序](../resources/teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="7f1e8-106">若要更新应用程序，必须将应用程序的 **distributionMethod** 属性设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="7f1e8-107">此 API 专门更新 (租户应用程序目录) 发布到组织的应用程序目录中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>  

## <a name="permissions"></a><span data-ttu-id="7f1e8-108">权限</span><span class="sxs-lookup"><span data-stu-id="7f1e8-108">Permissions</span></span>

<span data-ttu-id="7f1e8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](https://developer.microsoft.com/graph/docs/concepts/permissions_reference)。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](https://developer.microsoft.com/graph/docs/concepts/permissions_reference).</span></span>

><span data-ttu-id="7f1e8-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="7f1e8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f1e8-112">Permission Type</span></span>                        | <span data-ttu-id="7f1e8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f1e8-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="7f1e8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1e8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f1e8-115">AppCatalog、所有的目录读写。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-115">AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="7f1e8-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1e8-116">Delegated (work or school account)</span></span> | <span data-ttu-id="7f1e8-117">AppCatalog.Submit</span><span class="sxs-lookup"><span data-stu-id="7f1e8-117">AppCatalog.Submit</span></span>|
| <span data-ttu-id="7f1e8-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1e8-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f1e8-119">不支持</span><span class="sxs-lookup"><span data-stu-id="7f1e8-119">Not supported</span></span>|
| <span data-ttu-id="7f1e8-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f1e8-120">Application</span></span>                            | <span data-ttu-id="7f1e8-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-121">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f1e8-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f1e8-122">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="7f1e8-123">查询参数</span><span class="sxs-lookup"><span data-stu-id="7f1e8-123">Query parameters</span></span>

|<span data-ttu-id="7f1e8-124">属性</span><span class="sxs-lookup"><span data-stu-id="7f1e8-124">Property</span></span>|<span data-ttu-id="7f1e8-125">类型</span><span class="sxs-lookup"><span data-stu-id="7f1e8-125">Type</span></span>|<span data-ttu-id="7f1e8-126">说明</span><span class="sxs-lookup"><span data-stu-id="7f1e8-126">Description</span></span>|
|----|----|----|
|<span data-ttu-id="7f1e8-127">requiresReview</span><span class="sxs-lookup"><span data-stu-id="7f1e8-127">requiresReview</span></span>| <span data-ttu-id="7f1e8-128">Boolean</span><span class="sxs-lookup"><span data-stu-id="7f1e8-128">Boolean</span></span> | <span data-ttu-id="7f1e8-129">此可选查询参数触发应用程序审阅过程。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-129">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="7f1e8-130">具有管理员权限的用户无需触发评审即可提交应用程序。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-130">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="7f1e8-131">如果用户希望在发布之前请求审阅，则必须将其设置  `requiresReview` 为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-131">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="7f1e8-132">具有管理员权限的用户可以选择不设置 `requiresReview` 或设置值 `false`  ，并且应用将被视为 "已批准"，并将立即发布。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-132">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="7f1e8-133">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f1e8-133">Request headers</span></span>

| <span data-ttu-id="7f1e8-134">标头</span><span class="sxs-lookup"><span data-stu-id="7f1e8-134">Header</span></span>        | <span data-ttu-id="7f1e8-135">值</span><span class="sxs-lookup"><span data-stu-id="7f1e8-135">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="7f1e8-136">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f1e8-136">Authorization</span></span> | <span data-ttu-id="7f1e8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="7f1e8-139">Content-Type</span><span class="sxs-lookup"><span data-stu-id="7f1e8-139">Content-Type</span></span>  | <span data-ttu-id="7f1e8-140">application/zip。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-140">application/zip.</span></span> <span data-ttu-id="7f1e8-141">必需。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-141">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f1e8-142">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f1e8-142">Request body</span></span>

<span data-ttu-id="7f1e8-143">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-143">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="7f1e8-144">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-144">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

><span data-ttu-id="7f1e8-145">**注意：** 使用从 [列表已发布的应用程序](./teamsapp-list.md) 调用中返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-145">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="7f1e8-146">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-146">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="7f1e8-147">响应</span><span class="sxs-lookup"><span data-stu-id="7f1e8-147">Response</span></span>

<span data-ttu-id="7f1e8-148">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-148">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="7f1e8-149">示例</span><span class="sxs-lookup"><span data-stu-id="7f1e8-149">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="7f1e8-150">示例1：更新之前发布到 Microsoft 团队应用程序目录的应用程序</span><span class="sxs-lookup"><span data-stu-id="7f1e8-150">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="7f1e8-151">请求</span><span class="sxs-lookup"><span data-stu-id="7f1e8-151">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="7f1e8-152">有关团队应用程序 zip 文件的详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-152">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="7f1e8-153">响应</span><span class="sxs-lookup"><span data-stu-id="7f1e8-153">Response</span></span>

<span data-ttu-id="7f1e8-154">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-154">If successful, this method returns a `204 No Content` response code.</span></span>

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="7f1e8-155">示例2：在当前租户目录中发布之前更新现有应用程序的新版本，以供管理员审阅</span><span class="sxs-lookup"><span data-stu-id="7f1e8-155">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

### <a name="request"></a><span data-ttu-id="7f1e8-156">请求</span><span class="sxs-lookup"><span data-stu-id="7f1e8-156">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="7f1e8-157">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f1e8-157">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions?requiresReview=true
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="javascript"></a>[<span data-ttu-id="7f1e8-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f1e8-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f1e8-159">响应</span><span class="sxs-lookup"><span data-stu-id="7f1e8-159">Response</span></span>

<span data-ttu-id="7f1e8-160">如果成功，此方法 `201 Created` `publishingState` `submitted` 在响应正文中返回响应代码和键/值对：。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-160">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="7f1e8-161">*请参阅* [teamsappdefinition](../resources/teamsappdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="7f1e8-161">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
Location: https://graph.microsoft.com/beta/appCatalogs/teamsApps/e3e29acb-8c79-412b-b746-e6c39ff4cd22/appDefinitions/MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#appDefinition",
    "@odata.etag": "158749010",
    "id": "MGQ4MjBlY2QtZGVmMi00Mjk3LWFkYWQtNzgwNTZjZGU3Yzc4IyMxLjAuMA==",
    "teamsAppId": "e3e29acb-8c79-412b-b746-e6c39ff4cd22",
    "displayName": "Test app",
    "version": "1.0.11",
    "azureADAppId": "a651cc7d-ec54-4fb2-9d0e-2c58dc830b0b",
    "requiredResourceSpecificApplicationPermissions":[
         "ChannelMessage.Read.Group",
         "Channel.Create.Group",
         "Tab.ReadWrite.Group",
         "Member.Read.Group"
    ],
    "publishingState": "submitted",
    "lastModifiedDateTime": "2020-02-10 22:48:33.841",
}
```


