---
title: 删除 teamsApp
description: '从组织的应用程序目录中删除 Teams 应用 (租户应用程序目录) 。 '
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: bbaf69d70a73626a550356e0ca235d693be7f3a6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471661"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="c2246-103">删除 teamsApp</span><span class="sxs-lookup"><span data-stu-id="c2246-103">Delete teamsApp</span></span>

<span data-ttu-id="c2246-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2246-104">Namespace: microsoft.graph</span></span>

<!-- markdownlint-disable MD001 -->
### <a name="delete-an-app-from-your-organizations-app-catalog"></a><span data-ttu-id="c2246-105">从组织的应用程序目录中删除应用</span><span class="sxs-lookup"><span data-stu-id="c2246-105">Delete an app from your organization's app catalog</span></span>

<span data-ttu-id="c2246-106">从 [组织](../resources/teamsapp.md) 的应用程序目录中删除应用程序 (租户应用程序目录) 。</span><span class="sxs-lookup"><span data-stu-id="c2246-106">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="c2246-107">若要删除应用，应用的 **distributionMethod** 属性必须设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="c2246-107">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="c2246-108">您还可以使用此 API 从审阅过程中删除已提交的应用。</span><span class="sxs-lookup"><span data-stu-id="c2246-108">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2246-109">权限</span><span class="sxs-lookup"><span data-stu-id="c2246-109">Permissions</span></span>

<span data-ttu-id="c2246-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2246-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="c2246-112">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="c2246-112">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="c2246-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2246-113">Permission Type</span></span>                        | <span data-ttu-id="c2246-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2246-114">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="c2246-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2246-115">Delegated (work or school account)</span></span> | <span data-ttu-id="c2246-116">AppCatalog.Submit、AppCatalog.ReadWrite.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2246-116">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="c2246-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2246-117">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2246-118">不支持</span><span class="sxs-lookup"><span data-stu-id="c2246-118">Not supported</span></span>|
| <span data-ttu-id="c2246-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2246-119">Application</span></span>                            | <span data-ttu-id="c2246-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2246-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c2246-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2246-121">HTTP request</span></span>

<span data-ttu-id="c2246-122">若要从应用程序目录中删除应用程序，请运行以下操作：</span><span class="sxs-lookup"><span data-stu-id="c2246-122">To delete an app from the app catalog:</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="c2246-123">若要删除已提交但尚未批准的应用：</span><span class="sxs-lookup"><span data-stu-id="c2246-123">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="c2246-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2246-124">Request headers</span></span>

| <span data-ttu-id="c2246-125">标头</span><span class="sxs-lookup"><span data-stu-id="c2246-125">Header</span></span>        | <span data-ttu-id="c2246-126">值</span><span class="sxs-lookup"><span data-stu-id="c2246-126">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="c2246-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2246-127">Authorization</span></span> | <span data-ttu-id="c2246-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c2246-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c2246-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2246-130">Request body</span></span>

<span data-ttu-id="c2246-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c2246-131">Do not supply a request body for this method.</span></span>

><span data-ttu-id="c2246-132">**注意：** 使用从列表已发布 [应用调用](./appcatalogs-list-teamsapps.md) 返回的 ID 引用要删除的应用。</span><span class="sxs-lookup"><span data-stu-id="c2246-132">**Note:** Use the ID returned from the [List published apps](./appcatalogs-list-teamsapps.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="c2246-133">请勿使用 zip 应用包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="c2246-133">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="c2246-134">响应</span><span class="sxs-lookup"><span data-stu-id="c2246-134">Response</span></span>

<span data-ttu-id="c2246-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c2246-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2246-137">示例</span><span class="sxs-lookup"><span data-stu-id="c2246-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2246-138">请求</span><span class="sxs-lookup"><span data-stu-id="c2246-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c2246-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="c2246-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="c2246-140">C#</span><span class="sxs-lookup"><span data-stu-id="c2246-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c2246-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2246-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c2246-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c2246-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c2246-143">Java</span><span class="sxs-lookup"><span data-stu-id="c2246-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="c2246-144">响应</span><span class="sxs-lookup"><span data-stu-id="c2246-144">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

