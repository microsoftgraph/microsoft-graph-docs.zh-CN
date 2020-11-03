---
title: 更新 teamsApp
description: '更新之前发布到 Microsoft 团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: c1eb3382053c20e210bd87f96a2bb1bc688f90c2
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48848394"
---
# <a name="update-teamsapp"></a><span data-ttu-id="f2092-103">更新 teamsApp</span><span class="sxs-lookup"><span data-stu-id="f2092-103">Update teamsApp</span></span>

<span data-ttu-id="f2092-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2092-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2092-105">更新之前发布到 Microsoft 团队应用程序目录的 [应用程序](../resources/teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="f2092-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="f2092-106">若要更新应用程序，必须将应用程序的 **distributionMethod** 属性设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="f2092-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="f2092-107">此 API 专门更新 (租户应用程序目录) 发布到组织的应用程序目录中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f2092-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>  

## <a name="permissions"></a><span data-ttu-id="f2092-108">权限</span><span class="sxs-lookup"><span data-stu-id="f2092-108">Permissions</span></span>

<span data-ttu-id="f2092-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2092-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="f2092-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="f2092-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="f2092-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2092-112">Permission Type</span></span>                        | <span data-ttu-id="f2092-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2092-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="f2092-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2092-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f2092-115">AppCatalog、AppCatalog、all 和所有目录。</span><span class="sxs-lookup"><span data-stu-id="f2092-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="f2092-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2092-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2092-117">不支持</span><span class="sxs-lookup"><span data-stu-id="f2092-117">Not supported</span></span>|
| <span data-ttu-id="f2092-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2092-118">Application</span></span>                            | <span data-ttu-id="f2092-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2092-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2092-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2092-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="query-parameters"></a><span data-ttu-id="f2092-121">查询参数</span><span class="sxs-lookup"><span data-stu-id="f2092-121">Query parameters</span></span>

|<span data-ttu-id="f2092-122">属性</span><span class="sxs-lookup"><span data-stu-id="f2092-122">Property</span></span>|<span data-ttu-id="f2092-123">类型</span><span class="sxs-lookup"><span data-stu-id="f2092-123">Type</span></span>|<span data-ttu-id="f2092-124">说明</span><span class="sxs-lookup"><span data-stu-id="f2092-124">Description</span></span>|
|----|----|----|
|<span data-ttu-id="f2092-125">requiresReview</span><span class="sxs-lookup"><span data-stu-id="f2092-125">requiresReview</span></span>| <span data-ttu-id="f2092-126">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2092-126">Boolean</span></span> | <span data-ttu-id="f2092-127">此可选查询参数触发应用程序审阅过程。</span><span class="sxs-lookup"><span data-stu-id="f2092-127">This optional query parameter triggers the app review process.</span></span> <span data-ttu-id="f2092-128">具有管理员权限的用户无需触发评审即可提交应用程序。</span><span class="sxs-lookup"><span data-stu-id="f2092-128">Users with admin privileges can submit apps without triggering a review.</span></span> <span data-ttu-id="f2092-129">如果用户希望在发布之前请求审阅，则必须将其设置  `requiresReview` 为 `true` 。</span><span class="sxs-lookup"><span data-stu-id="f2092-129">If users want to request a review before publishing, they must set  `requiresReview` to `true`.</span></span> <span data-ttu-id="f2092-130">具有管理员权限的用户可以选择不设置 `requiresReview` 或设置值 `false`  ，并且应用将被视为 "已批准"，并将立即发布。</span><span class="sxs-lookup"><span data-stu-id="f2092-130">A user who has admin privileges can opt not to set `requiresReview` or set the value to `false`  and the app will be considered approved and will publish instantly.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="f2092-131">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2092-131">Request headers</span></span>

| <span data-ttu-id="f2092-132">标头</span><span class="sxs-lookup"><span data-stu-id="f2092-132">Header</span></span>        | <span data-ttu-id="f2092-133">值</span><span class="sxs-lookup"><span data-stu-id="f2092-133">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="f2092-134">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2092-134">Authorization</span></span> | <span data-ttu-id="f2092-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2092-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f2092-137">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2092-137">Content-Type</span></span>  | <span data-ttu-id="f2092-138">application/zip。</span><span class="sxs-lookup"><span data-stu-id="f2092-138">application/zip.</span></span> <span data-ttu-id="f2092-139">必填。</span><span class="sxs-lookup"><span data-stu-id="f2092-139">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2092-140">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2092-140">Request body</span></span>

<span data-ttu-id="f2092-141">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="f2092-141">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="f2092-142">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="f2092-142">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>

><span data-ttu-id="f2092-143">**注意：** 使用从 [列表已发布的应用程序](./teamsapp-list.md) 调用中返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f2092-143">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call for to reference the app you'd like to update.</span></span> <span data-ttu-id="f2092-144">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="f2092-144">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="f2092-145">响应</span><span class="sxs-lookup"><span data-stu-id="f2092-145">Response</span></span>

<span data-ttu-id="f2092-146">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2092-146">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="f2092-147">示例</span><span class="sxs-lookup"><span data-stu-id="f2092-147">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="f2092-148">示例1：更新之前发布到 Microsoft 团队应用程序目录的应用程序</span><span class="sxs-lookup"><span data-stu-id="f2092-148">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="f2092-149">请求</span><span class="sxs-lookup"><span data-stu-id="f2092-149">Request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8/appDefinitions
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```

<span data-ttu-id="f2092-150">有关团队应用程序 zip 文件的详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)。</span><span class="sxs-lookup"><span data-stu-id="f2092-150">For details about the Teams application zip file, see [Create app package](/microsoftteams/platform/concepts/apps/apps-package).</span></span>
<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="f2092-151">响应</span><span class="sxs-lookup"><span data-stu-id="f2092-151">Response</span></span>

<span data-ttu-id="f2092-152">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f2092-152">If successful, this method returns a `204 No Content` response code.</span></span>

### <a name="example-2-update-a-new-version-of-an-existing-app-for-admin-review-prior-to-publication-in-the-current-tenant-catalog"></a><span data-ttu-id="f2092-153">示例2：在当前租户目录中发布之前更新现有应用程序的新版本，以供管理员审阅</span><span class="sxs-lookup"><span data-stu-id="f2092-153">Example 2: Update a new version of an existing app for admin review prior to publication in the current tenant catalog</span></span>

### <a name="request"></a><span data-ttu-id="f2092-154">请求</span><span class="sxs-lookup"><span data-stu-id="f2092-154">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="f2092-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2092-155">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="f2092-156">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2092-156">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f2092-157">响应</span><span class="sxs-lookup"><span data-stu-id="f2092-157">Response</span></span>

<span data-ttu-id="f2092-158">如果成功，此方法 `201 Created` `publishingState` `submitted` 在响应正文中返回响应代码和键/值对：。</span><span class="sxs-lookup"><span data-stu-id="f2092-158">If successful, this method returns a `201 Created` response code and the key/value pair `publishingState`: `submitted` in the response body.</span></span> <span data-ttu-id="f2092-159">*请参阅* [teamsappdefinition](../resources/teamsappdefinition.md)。</span><span class="sxs-lookup"><span data-stu-id="f2092-159">*See* [teamsappdefinition](../resources/teamsappdefinition.md).</span></span>

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
