---
author: JeremyKelley
description: 检索 Drive 资源的属性和关系。
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 4593959b5940df46d5a81dad95710aa6650511e4
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36718175"
---
# <a name="get-drive"></a><span data-ttu-id="c2235-103">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="c2235-103">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c2235-104">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c2235-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="c2235-105">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="c2235-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="c2235-106">权限</span><span class="sxs-lookup"><span data-stu-id="c2235-106">Permissions</span></span>

<span data-ttu-id="c2235-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2235-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2235-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2235-109">Permission type</span></span>      | <span data-ttu-id="c2235-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c2235-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c2235-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2235-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c2235-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2235-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2235-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2235-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c2235-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2235-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="c2235-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2235-115">Application</span></span> | <span data-ttu-id="c2235-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2235-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="c2235-117">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="c2235-117">Get current user's OneDrive</span></span>

<span data-ttu-id="c2235-118">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="c2235-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="c2235-119">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="c2235-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2235-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2235-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2235-121">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2235-121">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2235-122">C#</span><span class="sxs-lookup"><span data-stu-id="c2235-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2235-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2235-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2235-124">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2235-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="c2235-125">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="c2235-125">Get a user's OneDrive</span></span>

<span data-ttu-id="c2235-126">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="c2235-126">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="c2235-127">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="c2235-127">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2235-128">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2235-128">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2235-129">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2235-129">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2235-130">C#</span><span class="sxs-lookup"><span data-stu-id="c2235-130">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2235-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2235-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2235-132">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2235-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c2235-133">路径参数</span><span class="sxs-lookup"><span data-stu-id="c2235-133">Path parameters</span></span>

| <span data-ttu-id="c2235-134">参数名称</span><span class="sxs-lookup"><span data-stu-id="c2235-134">Parameter name</span></span> | <span data-ttu-id="c2235-135">值</span><span class="sxs-lookup"><span data-stu-id="c2235-135">Value</span></span>  | <span data-ttu-id="c2235-136">说明</span><span class="sxs-lookup"><span data-stu-id="c2235-136">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2235-137">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="c2235-137">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="c2235-138">string</span><span class="sxs-lookup"><span data-stu-id="c2235-138">string</span></span> | <span data-ttu-id="c2235-139">必需。</span><span class="sxs-lookup"><span data-stu-id="c2235-139">Required.</span></span> <span data-ttu-id="c2235-140">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="c2235-140">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="c2235-141">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="c2235-141">Get the document library associated with a group</span></span>

<span data-ttu-id="c2235-142">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="c2235-142">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2235-143">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2235-143">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2235-144">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2235-144">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2235-145">C#</span><span class="sxs-lookup"><span data-stu-id="c2235-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2235-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2235-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2235-147">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2235-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c2235-148">路径参数</span><span class="sxs-lookup"><span data-stu-id="c2235-148">Path parameters</span></span>

| <span data-ttu-id="c2235-149">参数名称</span><span class="sxs-lookup"><span data-stu-id="c2235-149">Parameter name</span></span> | <span data-ttu-id="c2235-150">值</span><span class="sxs-lookup"><span data-stu-id="c2235-150">Value</span></span>  | <span data-ttu-id="c2235-151">说明</span><span class="sxs-lookup"><span data-stu-id="c2235-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2235-152">_groupId_</span><span class="sxs-lookup"><span data-stu-id="c2235-152">_groupId_</span></span>      | <span data-ttu-id="c2235-153">string</span><span class="sxs-lookup"><span data-stu-id="c2235-153">string</span></span> | <span data-ttu-id="c2235-154">必需。</span><span class="sxs-lookup"><span data-stu-id="c2235-154">Required.</span></span> <span data-ttu-id="c2235-155">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="c2235-155">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="c2235-156">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="c2235-156">Get the document library for a site</span></span>

<span data-ttu-id="c2235-157">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="c2235-157">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2235-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2235-158">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2235-159">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2235-159">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2235-160">C#</span><span class="sxs-lookup"><span data-stu-id="c2235-160">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2235-161">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2235-161">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2235-162">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2235-162">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c2235-163">路径参数</span><span class="sxs-lookup"><span data-stu-id="c2235-163">Path parameters</span></span>

| <span data-ttu-id="c2235-164">参数名称</span><span class="sxs-lookup"><span data-stu-id="c2235-164">Parameter name</span></span> | <span data-ttu-id="c2235-165">值</span><span class="sxs-lookup"><span data-stu-id="c2235-165">Value</span></span>  | <span data-ttu-id="c2235-166">说明</span><span class="sxs-lookup"><span data-stu-id="c2235-166">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2235-167">_siteId_</span><span class="sxs-lookup"><span data-stu-id="c2235-167">_siteId_</span></span>       | <span data-ttu-id="c2235-168">string</span><span class="sxs-lookup"><span data-stu-id="c2235-168">string</span></span> | <span data-ttu-id="c2235-169">必需。</span><span class="sxs-lookup"><span data-stu-id="c2235-169">Required.</span></span> <span data-ttu-id="c2235-170">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="c2235-170">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="c2235-171">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="c2235-171">Get a drive by ID</span></span>

<span data-ttu-id="c2235-172">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="c2235-172">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="c2235-173">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2235-173">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="c2235-174">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c2235-174">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{driveId}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="c2235-175">C#</span><span class="sxs-lookup"><span data-stu-id="c2235-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c2235-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c2235-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="c2235-177">目标-C</span><span class="sxs-lookup"><span data-stu-id="c2235-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="c2235-178">路径参数</span><span class="sxs-lookup"><span data-stu-id="c2235-178">Path parameters</span></span>

| <span data-ttu-id="c2235-179">参数名称</span><span class="sxs-lookup"><span data-stu-id="c2235-179">Parameter name</span></span> | <span data-ttu-id="c2235-180">值</span><span class="sxs-lookup"><span data-stu-id="c2235-180">Value</span></span>  | <span data-ttu-id="c2235-181">说明</span><span class="sxs-lookup"><span data-stu-id="c2235-181">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="c2235-182">_driveId_</span><span class="sxs-lookup"><span data-stu-id="c2235-182">_driveId_</span></span>      | <span data-ttu-id="c2235-183">字符串</span><span class="sxs-lookup"><span data-stu-id="c2235-183">string</span></span> | <span data-ttu-id="c2235-p105">必需。 请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="c2235-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="c2235-186">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c2235-186">Optional query parameters</span></span>

<span data-ttu-id="c2235-187">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="c2235-187">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="c2235-188">响应</span><span class="sxs-lookup"><span data-stu-id="c2235-188">Response</span></span>

<span data-ttu-id="c2235-189">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="c2235-189">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="c2235-190">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="c2235-190">Error response codes</span></span>

<span data-ttu-id="c2235-191">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="c2235-191">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
