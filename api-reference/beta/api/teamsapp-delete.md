---
title: 删除 teamsApp
description: " (租户应用程序目录) 中删除组织的应用程序目录中的团队应用程序。 "
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: f346115feaabf7a732cf849d50aac4375c7ba9ca
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968076"
---
# <a name="delete-teamsapp"></a><span data-ttu-id="6849b-103">删除 teamsApp</span><span class="sxs-lookup"><span data-stu-id="6849b-103">Delete teamsApp</span></span>

<span data-ttu-id="6849b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6849b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<!-- markdownlint-disable MD001 -->

<span data-ttu-id="6849b-105"> (租户应用程序目录) 中删除组织的应用程序目录中的 [应用](../resources/teamsapp.md) 程序。</span><span class="sxs-lookup"><span data-stu-id="6849b-105">Delete an [app](../resources/teamsapp.md) from an organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="6849b-106">若要删除应用程序，必须将应用程序的 **distributionMethod** 属性设置为 `organization` 。</span><span class="sxs-lookup"><span data-stu-id="6849b-106">To delete an app, the **distributionMethod** property for the app must be set to `organization`.</span></span>

<span data-ttu-id="6849b-107">您还可以使用此 API 从审阅过程中删除已提交的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6849b-107">You can also use this API to remove a submitted app from the review process.</span></span>

## <a name="permissions"></a><span data-ttu-id="6849b-108">权限</span><span class="sxs-lookup"><span data-stu-id="6849b-108">Permissions</span></span>

<span data-ttu-id="6849b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6849b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

><span data-ttu-id="6849b-111">**注意：** 只有全局管理员才能调用此 API。</span><span class="sxs-lookup"><span data-stu-id="6849b-111">**Note:** Only global administrators can call this API.</span></span> 

| <span data-ttu-id="6849b-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="6849b-112">Permission Type</span></span>                        | <span data-ttu-id="6849b-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6849b-113">Permissions (from least to most privileged)</span></span>|
|:----------------------------------     |:-------------|
| <span data-ttu-id="6849b-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6849b-114">Delegated (work or school account)</span></span> | <span data-ttu-id="6849b-115">AppCatalog、AppCatalog、all 和所有目录。</span><span class="sxs-lookup"><span data-stu-id="6849b-115">AppCatalog.Submit, AppCatalog.ReadWrite.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="6849b-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6849b-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6849b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="6849b-117">Not supported.</span></span>|
| <span data-ttu-id="6849b-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="6849b-118">Application</span></span>                            | <span data-ttu-id="6849b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6849b-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6849b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6849b-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

<span data-ttu-id="6849b-121">从应用程序目录中删除应用程序：</span><span class="sxs-lookup"><span data-stu-id="6849b-121">To delete an app from the app catalog:</span></span>

```http
DELETE /appCatalogs/teamsApps/{id}
```

<span data-ttu-id="6849b-122">若要删除已提交但尚未批准的应用程序，请执行以下操作：</span><span class="sxs-lookup"><span data-stu-id="6849b-122">To delete an app that has been submitted but has not been approved:</span></span>

```http
DELETE appCatalogs/teamsApps/{appId}/appDefinitions/{appDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="6849b-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="6849b-123">Request headers</span></span>

| <span data-ttu-id="6849b-124">标头</span><span class="sxs-lookup"><span data-stu-id="6849b-124">Header</span></span>        | <span data-ttu-id="6849b-125">值</span><span class="sxs-lookup"><span data-stu-id="6849b-125">Value</span></span>           |
|:--------------|:--------------  |
| <span data-ttu-id="6849b-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="6849b-126">Authorization</span></span> | <span data-ttu-id="6849b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6849b-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6849b-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="6849b-129">Request body</span></span>

<span data-ttu-id="6849b-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6849b-130">Do not supply a request body for this method.</span></span>

><span data-ttu-id="6849b-131">**注意：** 使用从 [列表已发布的应用程序](./teamsapp-list.md) 调用返回的 ID 引用要删除的应用程序。</span><span class="sxs-lookup"><span data-stu-id="6849b-131">**Note:** Use the ID returned from the [List published apps](./teamsapp-list.md) call to reference the app you'd like to delete.</span></span> <span data-ttu-id="6849b-132">请勿使用 zip 应用程序包清单中的 ID。</span><span class="sxs-lookup"><span data-stu-id="6849b-132">Do not use the ID from the manifest of the zip app package.</span></span>

## <a name="response"></a><span data-ttu-id="6849b-133">响应</span><span class="sxs-lookup"><span data-stu-id="6849b-133">Response</span></span>

<span data-ttu-id="6849b-p105">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="6849b-p105">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6849b-136">示例</span><span class="sxs-lookup"><span data-stu-id="6849b-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="6849b-137">请求</span><span class="sxs-lookup"><span data-stu-id="6849b-137">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="6849b-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="6849b-138">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_teamsapp"
}-->

```http
DELETE https://graph.microsoft.com/beta/appCatalogs/teamsApps/06805b9e-77e3-4b93-ac81-525eb87513b8
```
# <a name="c"></a>[<span data-ttu-id="6849b-139">C#</span><span class="sxs-lookup"><span data-stu-id="6849b-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6849b-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6849b-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6849b-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6849b-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6849b-142">Java</span><span class="sxs-lookup"><span data-stu-id="6849b-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-teamsapp-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

### <a name="response"></a><span data-ttu-id="6849b-143">响应</span><span class="sxs-lookup"><span data-stu-id="6849b-143">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
