---
title: 列出 teamsApp
description: 列出在租户应用目录中发布的 Teams 应用。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 35a922e2ed7fd3ccd4c41d19173199d243bb3192
ms.sourcegitcommit: 75428fc7535662f34e965c6b69fef3a53fdaf1cb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/16/2020
ms.locfileid: "49690362"
---
# <a name="list-teamsapp"></a><span data-ttu-id="059ed-103">列出 teamsApp</span><span class="sxs-lookup"><span data-stu-id="059ed-103">List teamsApp</span></span>

<span data-ttu-id="059ed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="059ed-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="059ed-105">列出 [在](../resources/teamsapp.md) Microsoft Teams 应用目录中发布的应用。</span><span class="sxs-lookup"><span data-stu-id="059ed-105">List [apps](../resources/teamsapp.md) published in the Microsoft Teams app catalog.</span></span> <span data-ttu-id="059ed-106">这包括来自 Microsoft Teams 应用商店的应用，以及组织的应用程序目录中的应用 (租户应用程序) 。</span><span class="sxs-lookup"><span data-stu-id="059ed-106">This includes apps from the Microsoft Teams store, as well as apps from your organization's app catalog (the tenant app catalog).</span></span> <span data-ttu-id="059ed-107">若要仅从组织的应用程序目录中获取应用，请 `organization` 指定为请求中的 **distributionMethod。**</span><span class="sxs-lookup"><span data-stu-id="059ed-107">To get apps from your organization's app catalog only, specify `organization` as the **distributionMethod** in the request.</span></span>

## <a name="permissions"></a><span data-ttu-id="059ed-108">权限</span><span class="sxs-lookup"><span data-stu-id="059ed-108">Permissions</span></span>

<span data-ttu-id="059ed-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="059ed-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

> <span data-ttu-id="059ed-111">**注意：** 只有全局管理员可以调用此 API。</span><span class="sxs-lookup"><span data-stu-id="059ed-111">**Note:** Only global administrators can call this API.</span></span>

| <span data-ttu-id="059ed-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="059ed-112">Permission Type</span></span>                        | <span data-ttu-id="059ed-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="059ed-113">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:------------------------------------|
| <span data-ttu-id="059ed-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="059ed-114">Delegated (work or school account)</span></span>     | <span data-ttu-id="059ed-115">AppCatalog.Read.All、AppCatalog.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="059ed-115">AppCatalog.Read.All, AppCatalog.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |
| <span data-ttu-id="059ed-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="059ed-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="059ed-117">不支持</span><span class="sxs-lookup"><span data-stu-id="059ed-117">Not supported</span></span>                       |
| <span data-ttu-id="059ed-118">Application</span><span class="sxs-lookup"><span data-stu-id="059ed-118">Application</span></span>                            | <span data-ttu-id="059ed-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="059ed-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="059ed-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="059ed-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /appCatalogs/teamsApps
```

## <a name="optional-query-parameters"></a><span data-ttu-id="059ed-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="059ed-121">Optional query parameters</span></span>

<span data-ttu-id="059ed-122">此方法支持使用 `$filter`、`$select` 和`$expand` [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="059ed-122">This method supports the `$filter`, `$select`, and `$expand` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

<span data-ttu-id="059ed-123">`$expand=AppDefinitions`使用将返回有关应用状态详细信息。</span><span class="sxs-lookup"><span data-stu-id="059ed-123">Using `$expand=AppDefinitions` will return more information about the state of the app.</span></span> 

> <span data-ttu-id="059ed-124">**注意：** 可以筛选 [teamsApp](../resources/teamsapp.md) 对象的任何字段以缩短结果列表。</span><span class="sxs-lookup"><span data-stu-id="059ed-124">**Note:** You can filter on any of the fields of the [teamsApp](../resources/teamsapp.md) object to shorten the list of results.</span></span> <span data-ttu-id="059ed-125">可以使用下列任一筛选操作：等于、不等于和/或不。</span><span class="sxs-lookup"><span data-stu-id="059ed-125">You can use any of the following filter operations: Equal, not-equal, and, or, and not.</span></span>

## <a name="request-headers"></a><span data-ttu-id="059ed-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="059ed-126">Request headers</span></span>

| <span data-ttu-id="059ed-127">标头</span><span class="sxs-lookup"><span data-stu-id="059ed-127">Header</span></span>        | <span data-ttu-id="059ed-128">值</span><span class="sxs-lookup"><span data-stu-id="059ed-128">Value</span></span>                     |
|:--------------|:--------------------------|
| <span data-ttu-id="059ed-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="059ed-129">Authorization</span></span> | <span data-ttu-id="059ed-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="059ed-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="059ed-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="059ed-132">Request body</span></span>

<span data-ttu-id="059ed-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="059ed-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="059ed-134">响应</span><span class="sxs-lookup"><span data-stu-id="059ed-134">Response</span></span>

<span data-ttu-id="059ed-135">如果成功，此方法在响应 `200 OK` 正文中返回响应代码和 [teamsApp](../resources/teamsapp.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="059ed-135">If successful, this method returns a `200 OK` response code and a list of [teamsApp](../resources/teamsapp.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="059ed-136">示例</span><span class="sxs-lookup"><span data-stu-id="059ed-136">Examples</span></span>

### <a name="example-1-list-all-applications-specific-to-the-tenant"></a><span data-ttu-id="059ed-137">示例 1：列出特定于租户的所有应用程序</span><span class="sxs-lookup"><span data-stu-id="059ed-137">Example 1: List all applications specific to the tenant</span></span>

<span data-ttu-id="059ed-138">以下示例列出了特定于租户的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="059ed-138">The following example lists all applications that are specific to your tenant.</span></span>

#### <a name="request"></a><span data-ttu-id="059ed-139">请求</span><span class="sxs-lookup"><span data-stu-id="059ed-139">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="059ed-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="059ed-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapps_filter_distributionMethod"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=distributionMethod eq 'organization'
```
# <a name="c"></a>[<span data-ttu-id="059ed-141">C#</span><span class="sxs-lookup"><span data-stu-id="059ed-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapps-filter-distributionmethod-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="059ed-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="059ed-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapps-filter-distributionmethod-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="059ed-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="059ed-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapps-filter-distributionmethod-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="059ed-144">Java</span><span class="sxs-lookup"><span data-stu-id="059ed-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapps-filter-distributionmethod-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---




<!-- markdownlint-disable MD024 -->

#### <a name="response"></a><span data-ttu-id="059ed-145">响应</span><span class="sxs-lookup"><span data-stu-id="059ed-145">Response</span></span>

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

### <a name="example-2-list-applications-with-a-given-id"></a><span data-ttu-id="059ed-146">示例 2：列出具有给定 ID 的应用程序</span><span class="sxs-lookup"><span data-stu-id="059ed-146">Example 2: List applications with a given ID</span></span>

<span data-ttu-id="059ed-147">以下示例列出具有给定 ID 的应用程序。</span><span class="sxs-lookup"><span data-stu-id="059ed-147">The following example lists applications with a given ID.</span></span>

#### <a name="request"></a><span data-ttu-id="059ed-148">请求</span><span class="sxs-lookup"><span data-stu-id="059ed-148">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="059ed-149">HTTP</span><span class="sxs-lookup"><span data-stu-id="059ed-149">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_id"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=id%20eq%20'b1c5353a-7aca-41b3-830f-27d5218fe0e5'
```
# <a name="c"></a>[<span data-ttu-id="059ed-150">C#</span><span class="sxs-lookup"><span data-stu-id="059ed-150">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="059ed-151">JavaScript</span><span class="sxs-lookup"><span data-stu-id="059ed-151">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="059ed-152">Objective-C</span><span class="sxs-lookup"><span data-stu-id="059ed-152">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="059ed-153">Java</span><span class="sxs-lookup"><span data-stu-id="059ed-153">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="059ed-154">响应</span><span class="sxs-lookup"><span data-stu-id="059ed-154">Response</span></span>

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
### <a name="example-3-find-application-based-on-the-teams-app-manifest-id"></a><span data-ttu-id="059ed-155">示例 3：根据 Teams 应用清单 ID 查找应用程序。</span><span class="sxs-lookup"><span data-stu-id="059ed-155">Example 3: Find application based on the Teams app manifest ID.</span></span>

<span data-ttu-id="059ed-156">以下示例列出了与 Teams 应用清单中指定的"id"匹配的应用程序。</span><span class="sxs-lookup"><span data-stu-id="059ed-156">The following example lists applications that match the 'id' specified in the Teams app manifest.</span></span> <span data-ttu-id="059ed-157">在此示例中，Teams 应用的清单 ID 为“cf1ba4c7-f94e-4d80-ba90-5594b641a8ee”。</span><span class="sxs-lookup"><span data-stu-id="059ed-157">In the example, the manifest ID of the Teams app is 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'.</span></span>

#### <a name="request"></a><span data-ttu-id="059ed-158">请求</span><span class="sxs-lookup"><span data-stu-id="059ed-158">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="059ed-159">HTTP</span><span class="sxs-lookup"><span data-stu-id="059ed-159">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_teamsapp_filter_externalid"
}-->

```msgraph-interactive
GET  https://graph.microsoft.com/v1.0/appCatalogs/teamsApps?$filter=externalId eq 'cf1ba4c7-f94e-4d80-ba90-5594b641a8ee'
```
# <a name="c"></a>[<span data-ttu-id="059ed-160">C#</span><span class="sxs-lookup"><span data-stu-id="059ed-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-teamsapp-filter-externalid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="059ed-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="059ed-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-teamsapp-filter-externalid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="059ed-162">Objective-C</span><span class="sxs-lookup"><span data-stu-id="059ed-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-teamsapp-filter-externalid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="059ed-163">Java</span><span class="sxs-lookup"><span data-stu-id="059ed-163">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-teamsapp-filter-externalid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="059ed-164">响应</span><span class="sxs-lookup"><span data-stu-id="059ed-164">Response</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#appCatalogs/teamsApps",
    "value": [
        {
            "id": "22f73bbe-f67a-4dea-bd54-54cac718cb2b",
            "externalId": "cf1ba4c7-f94e-4d80-ba90-5594b641a8ee",
            "displayName": "YPA",
            "distributionMethod": "organization"
        }
    ]
}
```

## <a name="see-also"></a><span data-ttu-id="059ed-165">另请参阅</span><span class="sxs-lookup"><span data-stu-id="059ed-165">See also</span></span>

- [<span data-ttu-id="059ed-166">列出在团队中安装的应用</span><span class="sxs-lookup"><span data-stu-id="059ed-166">List apps installed in a team</span></span>](team-list-installedapps.md)
- [<span data-ttu-id="059ed-167">列出在用户的个人范围内安装的应用</span><span class="sxs-lookup"><span data-stu-id="059ed-167">List apps installed in the personal scope of a user</span></span>](userteamwork-list-installedapps.md)

