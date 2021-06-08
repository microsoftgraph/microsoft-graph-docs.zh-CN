---
title: 删除 teamsApp
description: '从Teams应用程序目录中从组织的应用程序目录中删除 (应用程序) 。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 9952dabb38b1f9849b5df3b3fff3fafdf029c971
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52787728"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="3e3eb-103">删除 teamsApp</span><span class="sxs-lookup"><span data-stu-id="3e3eb-103">Delete teamsApp</span></span>

<span data-ttu-id="3e3eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e3eb-104">Namespace: microsoft.graph</span></span>

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="3e3eb-105">从组织的应用程序目录中删除应用程序</span><span class="sxs-lookup"><span data-stu-id="3e3eb-105">Delete an app from your organization's app catalog</span></span>

<span data-ttu-id="3e3eb-106">从 [租户](../resources/teamsapp.md) 应用程序目录组织的应用程序目录中 (应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-106">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="3e3eb-107">若要删除应用，应用的 **distributionMethod** 属性必须设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-107">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="3e3eb-108">您还可以使用此 API 从评价过程中删除已提交的应用。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-108">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="3e3eb-109">权限</span><span class="sxs-lookup"><span data-stu-id="3e3eb-109">Permissions</span></span>

<span data-ttu-id="3e3eb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="3e3eb-112">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="3e3eb-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="3e3eb-113">Permission Type</span></span>                        | <span data-ttu-id="3e3eb-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3e3eb-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="3e3eb-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3e3eb-115">Delegated (work or school account)</span></span> | <span data-ttu-id="3e3eb-116">AppCatalog.Submit、AppCatalog.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3e3eb-116">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="3e3eb-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3e3eb-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3e3eb-118">不支持</span><span class="sxs-lookup"><span data-stu-id="3e3eb-118">Not supported</span></span>|
| <span data-ttu-id="3e3eb-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="3e3eb-119">Application</span></span>                            | <span data-ttu-id="3e3eb-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="3e3eb-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3e3eb-121">HTTP request</span></span>

<span data-ttu-id="3e3eb-122">若要从应用程序目录中删除应用程序，请运行以下操作：</span><span class="sxs-lookup"><span data-stu-id="3e3eb-122">To delete an app from the app catalog:</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="3e3eb-123">若要删除已提交但尚未批准的应用，请运行：</span><span class="sxs-lookup"><span data-stu-id="3e3eb-123">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="3e3eb-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="3e3eb-124">Request headers</span></span>

| <span data-ttu-id="3e3eb-125">标头</span><span class="sxs-lookup"><span data-stu-id="3e3eb-125">Header</span></span>        | <span data-ttu-id="3e3eb-126">值</span><span class="sxs-lookup"><span data-stu-id="3e3eb-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="3e3eb-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="3e3eb-127">Authorization</span></span> | <span data-ttu-id="3e3eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3e3eb-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="3e3eb-130">Request body</span></span>

<span data-ttu-id="3e3eb-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-131">Do not supply a request body for this method.</span></span>

><span data-ttu-id="3e3eb-132">**注意：** 使用从列表已发布 [的应用](./appcatalogs-list-teamsapps.md) 调用返回的 ID 来引用你要删除的应用。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-132">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="3e3eb-133">请勿使用 zip 应用包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="3e3eb-134">响应</span><span class="sxs-lookup"><span data-stu-id="3e3eb-134">Response</span></span>

<span data-ttu-id="3e3eb-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="3e3eb-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3e3eb-137">示例</span><span class="sxs-lookup"><span data-stu-id="3e3eb-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="3e3eb-138">请求</span><span class="sxs-lookup"><span data-stu-id="3e3eb-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3e3eb-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="3e3eb-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="3e3eb-140">C#</span><span class="sxs-lookup"><span data-stu-id="3e3eb-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3e3eb-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3e3eb-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3e3eb-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3e3eb-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3e3eb-143">Java</span><span class="sxs-lookup"><span data-stu-id="3e3eb-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="3e3eb-144">响应</span><span class="sxs-lookup"><span data-stu-id="3e3eb-144">Response</span></span>

<!-- {
  "blockType": "response"
} -->

```http
HTTP/1.1 204 No Content
```

