---
title: 列出 teamsApp
description: '列出 Microsoft 团队应用程序目录中的应用程序。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 3fa9e49c35101cd151b18c4af9066d371b729bfc
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46806281"
---
# <a name="list-teamsapp"></a><span data-ttu-id="81ef1-103">列出 teamsApp</span><span class="sxs-lookup"><span data-stu-id="81ef1-103">List teamsApp</span></span>

<span data-ttu-id="81ef1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81ef1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81ef1-105">列出 Microsoft 团队应用程序目录中的 [应用程序](../resources/teamsapp.md) 。</span><span class="sxs-lookup"><span data-stu-id="81ef1-105">List [apps](../resources/teamsapp.md) from the Microsoft Teams app catalog.</span></span>
<span data-ttu-id="81ef1-106">这包括 Microsoft 团队存储中的应用程序，以及组织的应用程序目录 (租户应用程序目录) 中的应用程序。</span><span class="sxs-lookup"><span data-stu-id="81ef1-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="81ef1-107">若要仅从组织的应用程序目录中获取应用程序，请 `organization` 在请求中将 **distributionMethod** 指定为 ""。</span><span class="sxs-lookup"><span data-stu-id="81ef1-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="81ef1-108">权限</span><span class="sxs-lookup"><span data-stu-id="81ef1-108">Permissions</span></span>

<span data-ttu-id="81ef1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81ef1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="81ef1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="81ef1-111">Permission Type</span></span>                        | <span data-ttu-id="81ef1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81ef1-112">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="81ef1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81ef1-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="81ef1-114">AppCatalog、AppCatalog、所有的、所有读写的。 all</span><span class="sxs-lookup"><span data-stu-id="81ef1-114">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="81ef1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81ef1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81ef1-116">不支持</span><span class="sxs-lookup"><span data-stu-id="81ef1-116">Not supported</span></span>                       |
| <span data-ttu-id="81ef1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="81ef1-117">Application</span></span>                            | <span data-ttu-id="81ef1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="81ef1-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="81ef1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81ef1-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="81ef1-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="81ef1-120">Optional query parameters</span></span>

<span data-ttu-id="81ef1-121">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="81ef1-121">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="81ef1-122">使用 `$expand=AppDefinitions` 将返回有关应用的状态的详细信息（如 **publishingState**），它反映应用程序提交的审阅状态，并返回应用程序是否已被批准、被拒绝或仍处于审阅状态。</span><span class="sxs-lookup"><span data-stu-id="81ef1-122">Using `$expand=AppDefinitions` will return more information about the state of the app, such as the **publishingState**, which reflects the app submission review status and returns whether an app has been approved, rejected, or remains under review.</span></span> 

> <span data-ttu-id="81ef1-123">**注意：** 您可以对 [teamsApp](../resources/teamsapp.md) 对象的任何字段进行筛选，以缩短结果列表。</span><span class="sxs-lookup"><span data-stu-id="81ef1-123">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="81ef1-124">您可以使用以下任何筛选器操作：等于、不等于、和、或，而不是。</span><span class="sxs-lookup"><span data-stu-id="81ef1-124">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="81ef1-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="81ef1-125">Request headers</span></span>

| <span data-ttu-id="81ef1-126">标头</span><span class="sxs-lookup"><span data-stu-id="81ef1-126">Header</span></span>        | <span data-ttu-id="81ef1-127">值</span><span class="sxs-lookup"><span data-stu-id="81ef1-127">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="81ef1-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="81ef1-128">Authorization</span></span> | <span data-ttu-id="81ef1-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81ef1-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="81ef1-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="81ef1-131">Request body</span></span>

<span data-ttu-id="81ef1-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81ef1-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81ef1-133">响应</span><span class="sxs-lookup"><span data-stu-id="81ef1-133">Response</span></span>

<span data-ttu-id="81ef1-134">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [teamsApp](../resources/teamsapp.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="81ef1-134">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="81ef1-135">示例</span><span class="sxs-lookup"><span data-stu-id="81ef1-135">Examples</span></span>

### <a name="example-1-list-all-applications-in-a-tenant"></a><span data-ttu-id="81ef1-136">示例1：列出租户中的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="81ef1-136">Example 1: List all applications in a tenant</span></span>

<span data-ttu-id="81ef1-137">下面的示例列出了特定于您的租户的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="81ef1-137">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="81ef1-138">请求</span><span class="sxs-lookup"><span data-stu-id="81ef1-138">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="81ef1-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="81ef1-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="81ef1-140">C#</span><span class="sxs-lookup"><span data-stu-id="81ef1-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81ef1-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81ef1-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81ef1-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81ef1-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="81ef1-143">响应</span><span class="sxs-lookup"><span data-stu-id="81ef1-143">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="81ef1-144">示例2：列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="81ef1-144">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="81ef1-145">下面的示例列出了具有给定 ID 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="81ef1-145">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="81ef1-146">请求</span><span class="sxs-lookup"><span data-stu-id="81ef1-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="81ef1-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="81ef1-147">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="81ef1-148">C#</span><span class="sxs-lookup"><span data-stu-id="81ef1-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="81ef1-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="81ef1-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="81ef1-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="81ef1-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="81ef1-151">响应</span><span class="sxs-lookup"><span data-stu-id="81ef1-151">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "b1c5353a-7aca-41b3-830f-27d5218fe0e5",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization"
    }
  ]
}
```

### <a name="example-3-list-applications-with-a-given-id-and-return-the-submission-review-state"></a><span data-ttu-id="81ef1-152">示例3：列出具有给定 ID 的应用程序，并返回提交检查状态</span><span class="sxs-lookup"><span data-stu-id="81ef1-152">Example 3: List applications with a given ID, and return the submission review state</span></span>

<span data-ttu-id="81ef1-153">下面的示例列出了具有给定 ID 的应用程序，并展开 **appDefinitions** 以返回 **publishingState**，这将反映应用程序的提交审阅状态。</span><span class="sxs-lookup"><span data-stu-id="81ef1-153">The following example lists applications with a given ID, and expands **appDefinitions** to return the **publishingState**, which reflects the app's submission review state.</span></span> <span data-ttu-id="81ef1-154">`Submitted` 表示正在等待审阅， `published` 表示该应用程序已由管理员批准，并且该 `rejected` 应用程序被管理员拒绝。</span><span class="sxs-lookup"><span data-stu-id="81ef1-154">`Submitted` means the review is pending, `published` means the app was approved by the admin, and `rejected` means the app was rejected by the admin.</span></span>

#### <a name="request"></a><span data-ttu-id="81ef1-155">请求</span><span class="sxs-lookup"><span data-stu-id="81ef1-155">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list_teamsapp"
}-->

```http
GET  https://graph.microsoft.com/beta/appCatalogs/teamsApps?$filter=id eq '876df28f-2e78-423b-94a5-44181bd0e225'&$expand=appDefinitions
```

#### <a name="response"></a><span data-ttu-id="81ef1-156">响应</span><span class="sxs-lookup"><span data-stu-id="81ef1-156">Response</span></span>

<!-- {
  "blockType": "response",
  "@odata.type": "microsoft.graph.teamsApp",
  "truncated": true,
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "876df28f-2e78-423b-94a5-44181bd0e225",
      "externalId": "f31b1263-ba99-435a-a679-911d24850d7c",
      "name": "Test App",
      "version": "1.0.1",
      "distributionMethod": "Organization",
      "appDefinitions": [
                {

                    "id": "NGQyMGNiNDUtZWViYS00ZTEyLWE3YzktMGQ0NDgzYjYxNzU2IyMxLjAuMA==",

                    "teamsAppId": "876df28f-2e78-423b-94a5-44181bd0e225",

                    "azureADAppId": null,

                    "displayName": "Test App",

                    "version": "1.0.1",

                    "requiredResourceSpecificApplicationPermissions": [],

                    "publishingState": "published"

                  }
            ]
      }
    ]
  }
```
