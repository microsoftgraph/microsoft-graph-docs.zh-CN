---
title: 更新 teamsApp
description: '更新之前发布到团队应用程序目录的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6f54f7938e448d83a9ac2ff70e1dfb215e1b71d6
ms.sourcegitcommit: d1e72c8d36aad78732133f9ecefaf66c433b8530
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2020
ms.locfileid: "48849149"
---
# <a name="update-teamsapp"></a><span data-ttu-id="113a8-103">更新 teamsApp</span><span class="sxs-lookup"><span data-stu-id="113a8-103">Update teamsApp</span></span>

<span data-ttu-id="113a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="113a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="113a8-105">更新之前发布到 Microsoft 团队应用程序目录的 [应用程序](../resources/teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="113a8-105">Update an [app](../resources/teamsapp.md) previously published to the Microsoft Teams app catalog.</span></span> <span data-ttu-id="113a8-106">若要更新应用程序，必须将应用程序的 **distributionMethod** 属性设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="113a8-106">To update an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="113a8-107">此 API 专门更新 (租户应用程序目录) 发布到组织的应用程序目录中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="113a8-107">This API specifically updates an app published to your organization's app catalog (the tenant app catalog).</span></span>

## <a name="permissions"></a><span data-ttu-id="113a8-108">权限</span><span class="sxs-lookup"><span data-stu-id="113a8-108">Permissions</span></span>

<span data-ttu-id="113a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="113a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="113a8-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="113a8-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="113a8-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="113a8-112">Permission Type</span></span>                        | <span data-ttu-id="113a8-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="113a8-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="113a8-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="113a8-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="113a8-115">AppCatalog、AppCatalog、all 和所有目录。</span><span class="sxs-lookup"><span data-stu-id="113a8-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="113a8-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="113a8-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="113a8-117">不支持</span><span class="sxs-lookup"><span data-stu-id="113a8-117">Not supported</span></span>|
| <span data-ttu-id="113a8-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="113a8-118">Application</span></span>                            | <span data-ttu-id="113a8-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="113a8-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="113a8-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="113a8-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /appCatalogs/teamsApps/{id}/appDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="113a8-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="113a8-121">Request headers</span></span>

| <span data-ttu-id="113a8-122">标头</span><span class="sxs-lookup"><span data-stu-id="113a8-122">Header</span></span>        | <span data-ttu-id="113a8-123">值</span><span class="sxs-lookup"><span data-stu-id="113a8-123">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="113a8-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="113a8-124">Authorization</span></span> | <span data-ttu-id="113a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="113a8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="113a8-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="113a8-127">Content-Type</span></span>  | <span data-ttu-id="113a8-128">application/zip。</span><span class="sxs-lookup"><span data-stu-id="113a8-128">application/zip.</span></span> <span data-ttu-id="113a8-129">必填。</span><span class="sxs-lookup"><span data-stu-id="113a8-129">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="113a8-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="113a8-130">Request body</span></span>

<span data-ttu-id="113a8-131">在请求正文中，包括团队 zip 清单有效负载。</span><span class="sxs-lookup"><span data-stu-id="113a8-131">In the request body, include a Teams zip manifest payload.</span></span> <span data-ttu-id="113a8-132">有关详细信息，请参阅 [创建应用程序包](/microsoftteams/platform/concepts/apps/apps-package)</span><span class="sxs-lookup"><span data-stu-id="113a8-132">For details, see [Create an app package](/microsoftteams/platform/concepts/apps/apps-package)</span></span>

><span data-ttu-id="113a8-133">**注意：** 使用从 [列表已发布的应用程序](./teamsapp-list.md) 调用返回的 ID 引用要更新的应用程序。</span><span class="sxs-lookup"><span data-stu-id="113a8-133">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to update.</span></span> <span data-ttu-id="113a8-134">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="113a8-134">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="113a8-135">响应</span><span class="sxs-lookup"><span data-stu-id="113a8-135">Response</span></span>

<span data-ttu-id="113a8-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="113a8-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="113a8-137">示例</span><span class="sxs-lookup"><span data-stu-id="113a8-137">Examples</span></span>

### <a name="example-1-update-an-application-previously-published-to-the-microsoft-teams-app-catalog"></a><span data-ttu-id="113a8-138">示例1：更新之前发布到 Microsoft 团队应用程序目录的应用程序</span><span class="sxs-lookup"><span data-stu-id="113a8-138">Example 1: Update an application previously published to the Microsoft Teams app catalog</span></span>

### <a name="request"></a><span data-ttu-id="113a8-139">请求</span><span class="sxs-lookup"><span data-stu-id="113a8-139">Request</span></span>

<!-- markdownlint-disable MD034 -->

# <a name="http"></a>[<span data-ttu-id="113a8-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="113a8-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_teamsapp"
}-->

```http
PUT https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
Content-type: application/zip
Content-length: 244

[Zip file containing a Teams app package]
```
# <a name="c"></a>[<span data-ttu-id="113a8-141">C#</span><span class="sxs-lookup"><span data-stu-id="113a8-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="113a8-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="113a8-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="113a8-143">响应</span><span class="sxs-lookup"><span data-stu-id="113a8-143">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
