---
author: JeremyKelley
description: 检索 Drive 资源的属性和关系。
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: de46637d41f6e3db9a8f5d546fdecf9db33103b2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42433305"
---
# <a name="get-drive"></a><span data-ttu-id="debf9-103">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="debf9-103">Get Drive</span></span>

<span data-ttu-id="debf9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="debf9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="debf9-105">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="debf9-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="debf9-106">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="debf9-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="debf9-107">权限</span><span class="sxs-lookup"><span data-stu-id="debf9-107">Permissions</span></span>

<span data-ttu-id="debf9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="debf9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="debf9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="debf9-110">Permission type</span></span>      | <span data-ttu-id="debf9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="debf9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="debf9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="debf9-112">Delegated (work or school account)</span></span> | <span data-ttu-id="debf9-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debf9-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="debf9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="debf9-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="debf9-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debf9-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="debf9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="debf9-116">Application</span></span> | <span data-ttu-id="debf9-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="debf9-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="debf9-118">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="debf9-118">Get current user's OneDrive</span></span>

<span data-ttu-id="debf9-119">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="debf9-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="debf9-120">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="debf9-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="debf9-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debf9-121">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="debf9-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="debf9-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[<span data-ttu-id="debf9-123">C#</span><span class="sxs-lookup"><span data-stu-id="debf9-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="debf9-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debf9-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="debf9-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="debf9-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="debf9-126">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="debf9-126">Get a user's OneDrive</span></span>

<span data-ttu-id="debf9-127">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="debf9-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="debf9-128">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="debf9-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="debf9-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debf9-129">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="debf9-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="debf9-130">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[<span data-ttu-id="debf9-131">C#</span><span class="sxs-lookup"><span data-stu-id="debf9-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="debf9-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debf9-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="debf9-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="debf9-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="debf9-134">路径参数</span><span class="sxs-lookup"><span data-stu-id="debf9-134">Path parameters</span></span>

| <span data-ttu-id="debf9-135">参数名称</span><span class="sxs-lookup"><span data-stu-id="debf9-135">Parameter name</span></span> | <span data-ttu-id="debf9-136">值</span><span class="sxs-lookup"><span data-stu-id="debf9-136">Value</span></span>  | <span data-ttu-id="debf9-137">说明</span><span class="sxs-lookup"><span data-stu-id="debf9-137">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="debf9-138">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="debf9-138">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="debf9-139">string</span><span class="sxs-lookup"><span data-stu-id="debf9-139">string</span></span> | <span data-ttu-id="debf9-140">必需。</span><span class="sxs-lookup"><span data-stu-id="debf9-140">Required.</span></span> <span data-ttu-id="debf9-141">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="debf9-141">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="debf9-142">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="debf9-142">Get the document library associated with a group</span></span>

<span data-ttu-id="debf9-143">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="debf9-143">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="debf9-144">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debf9-144">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="debf9-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="debf9-145">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[<span data-ttu-id="debf9-146">C#</span><span class="sxs-lookup"><span data-stu-id="debf9-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="debf9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debf9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="debf9-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="debf9-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="debf9-149">路径参数</span><span class="sxs-lookup"><span data-stu-id="debf9-149">Path parameters</span></span>

| <span data-ttu-id="debf9-150">参数名称</span><span class="sxs-lookup"><span data-stu-id="debf9-150">Parameter name</span></span> | <span data-ttu-id="debf9-151">值</span><span class="sxs-lookup"><span data-stu-id="debf9-151">Value</span></span>  | <span data-ttu-id="debf9-152">说明</span><span class="sxs-lookup"><span data-stu-id="debf9-152">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="debf9-153">_groupId_</span><span class="sxs-lookup"><span data-stu-id="debf9-153">_groupId_</span></span>      | <span data-ttu-id="debf9-154">string</span><span class="sxs-lookup"><span data-stu-id="debf9-154">string</span></span> | <span data-ttu-id="debf9-155">必需。</span><span class="sxs-lookup"><span data-stu-id="debf9-155">Required.</span></span> <span data-ttu-id="debf9-156">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="debf9-156">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="debf9-157">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="debf9-157">Get the document library for a site</span></span>

<span data-ttu-id="debf9-158">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="debf9-158">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="debf9-159">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debf9-159">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="debf9-160">HTTP</span><span class="sxs-lookup"><span data-stu-id="debf9-160">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[<span data-ttu-id="debf9-161">C#</span><span class="sxs-lookup"><span data-stu-id="debf9-161">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="debf9-162">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debf9-162">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="debf9-163">Objective-C</span><span class="sxs-lookup"><span data-stu-id="debf9-163">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="debf9-164">路径参数</span><span class="sxs-lookup"><span data-stu-id="debf9-164">Path parameters</span></span>

| <span data-ttu-id="debf9-165">参数名称</span><span class="sxs-lookup"><span data-stu-id="debf9-165">Parameter name</span></span> | <span data-ttu-id="debf9-166">值</span><span class="sxs-lookup"><span data-stu-id="debf9-166">Value</span></span>  | <span data-ttu-id="debf9-167">说明</span><span class="sxs-lookup"><span data-stu-id="debf9-167">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="debf9-168">_siteId_</span><span class="sxs-lookup"><span data-stu-id="debf9-168">_siteId_</span></span>       | <span data-ttu-id="debf9-169">string</span><span class="sxs-lookup"><span data-stu-id="debf9-169">string</span></span> | <span data-ttu-id="debf9-170">必需。</span><span class="sxs-lookup"><span data-stu-id="debf9-170">Required.</span></span> <span data-ttu-id="debf9-171">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="debf9-171">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="debf9-172">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="debf9-172">Get a drive by ID</span></span>

<span data-ttu-id="debf9-173">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="debf9-173">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="debf9-174">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="debf9-174">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="debf9-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="debf9-175">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{driveId}
```
# <a name="c"></a>[<span data-ttu-id="debf9-176">C#</span><span class="sxs-lookup"><span data-stu-id="debf9-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="debf9-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="debf9-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="debf9-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="debf9-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="debf9-179">路径参数</span><span class="sxs-lookup"><span data-stu-id="debf9-179">Path parameters</span></span>

| <span data-ttu-id="debf9-180">参数名称</span><span class="sxs-lookup"><span data-stu-id="debf9-180">Parameter name</span></span> | <span data-ttu-id="debf9-181">值</span><span class="sxs-lookup"><span data-stu-id="debf9-181">Value</span></span>  | <span data-ttu-id="debf9-182">说明</span><span class="sxs-lookup"><span data-stu-id="debf9-182">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="debf9-183">_driveId_</span><span class="sxs-lookup"><span data-stu-id="debf9-183">_driveId_</span></span>      | <span data-ttu-id="debf9-184">字符串</span><span class="sxs-lookup"><span data-stu-id="debf9-184">string</span></span> | <span data-ttu-id="debf9-p105">必需。 请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="debf9-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="debf9-187">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="debf9-187">Optional query parameters</span></span>

<span data-ttu-id="debf9-188">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="debf9-188">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="debf9-189">响应</span><span class="sxs-lookup"><span data-stu-id="debf9-189">Response</span></span>

<span data-ttu-id="debf9-190">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="debf9-190">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id",] } -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "b!t18F8ybsHUq1z3LTz8xvZqP8zaSWjkFNhsME-Fepo75dTf9vQKfeRblBZjoSQrd7",
    "driveType": "business",
    "owner": {
        "user": {
            "id": "efee1b77-fb3b-4f65-99d6-274c11914d12",
            "displayName": "Ryan Gregg"
        }
    },
    "quota": {
        "deleted": 256938,
        "remaining": 1099447353539,
        "state": "normal",
        "total": 1099511627776
    }
}
```

### <a name="error-response-codes"></a><span data-ttu-id="debf9-191">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="debf9-191">Error response codes</span></span>

<span data-ttu-id="debf9-192">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="debf9-192">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!--
{
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive",
  "suppressions": [
  ]
}
-->
