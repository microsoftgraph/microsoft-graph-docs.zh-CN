---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 8e099f6ba8bef07cba3406e2deb2cbb8961aa227
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260352"
---
# <a name="get-drive"></a><span data-ttu-id="3d362-102">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="3d362-102">Get Drive</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3d362-103">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="3d362-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="3d362-104">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="3d362-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="3d362-105">权限</span><span class="sxs-lookup"><span data-stu-id="3d362-105">Permissions</span></span>

<span data-ttu-id="3d362-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3d362-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3d362-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="3d362-108">Permission type</span></span>      | <span data-ttu-id="3d362-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3d362-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3d362-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3d362-110">Delegated (work or school account)</span></span> | <span data-ttu-id="3d362-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d362-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d362-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3d362-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3d362-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d362-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="3d362-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="3d362-114">Application</span></span> | <span data-ttu-id="3d362-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3d362-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="3d362-116">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="3d362-116">Get current user's OneDrive</span></span>

<span data-ttu-id="3d362-117">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="3d362-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="3d362-118">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="3d362-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3d362-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d362-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d362-120">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3d362-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d362-121">C#</span><span class="sxs-lookup"><span data-stu-id="3d362-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d362-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d362-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d362-123">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d362-123">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-default-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="3d362-124">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="3d362-124">Get a user's OneDrive</span></span>

<span data-ttu-id="3d362-125">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="3d362-125">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="3d362-126">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="3d362-126">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="3d362-127">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d362-127">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d362-128">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3d362-128">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d362-129">C#</span><span class="sxs-lookup"><span data-stu-id="3d362-129">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d362-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d362-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d362-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d362-131">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="3d362-132">路径参数</span><span class="sxs-lookup"><span data-stu-id="3d362-132">Path parameters</span></span>

| <span data-ttu-id="3d362-133">参数名称</span><span class="sxs-lookup"><span data-stu-id="3d362-133">Parameter name</span></span> | <span data-ttu-id="3d362-134">值</span><span class="sxs-lookup"><span data-stu-id="3d362-134">Value</span></span>  | <span data-ttu-id="3d362-135">说明</span><span class="sxs-lookup"><span data-stu-id="3d362-135">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3d362-136">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="3d362-136">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="3d362-137">string</span><span class="sxs-lookup"><span data-stu-id="3d362-137">string</span></span> | <span data-ttu-id="3d362-138">必需。</span><span class="sxs-lookup"><span data-stu-id="3d362-138">Required.</span></span> <span data-ttu-id="3d362-139">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="3d362-139">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="3d362-140">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="3d362-140">Get the document library associated with a group</span></span>

<span data-ttu-id="3d362-141">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="3d362-141">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="3d362-142">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d362-142">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d362-143">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3d362-143">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d362-144">C#</span><span class="sxs-lookup"><span data-stu-id="3d362-144">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d362-145">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d362-145">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d362-146">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d362-146">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="3d362-147">路径参数</span><span class="sxs-lookup"><span data-stu-id="3d362-147">Path parameters</span></span>

| <span data-ttu-id="3d362-148">参数名称</span><span class="sxs-lookup"><span data-stu-id="3d362-148">Parameter name</span></span> | <span data-ttu-id="3d362-149">值</span><span class="sxs-lookup"><span data-stu-id="3d362-149">Value</span></span>  | <span data-ttu-id="3d362-150">说明</span><span class="sxs-lookup"><span data-stu-id="3d362-150">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3d362-151">_groupId_</span><span class="sxs-lookup"><span data-stu-id="3d362-151">_groupId_</span></span>      | <span data-ttu-id="3d362-152">string</span><span class="sxs-lookup"><span data-stu-id="3d362-152">string</span></span> | <span data-ttu-id="3d362-153">必需。</span><span class="sxs-lookup"><span data-stu-id="3d362-153">Required.</span></span> <span data-ttu-id="3d362-154">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="3d362-154">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="3d362-155">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="3d362-155">Get the document library for a site</span></span>

<span data-ttu-id="3d362-156">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="3d362-156">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="3d362-157">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d362-157">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d362-158">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3d362-158">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d362-159">C#</span><span class="sxs-lookup"><span data-stu-id="3d362-159">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d362-160">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d362-160">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d362-161">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d362-161">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="3d362-162">路径参数</span><span class="sxs-lookup"><span data-stu-id="3d362-162">Path parameters</span></span>

| <span data-ttu-id="3d362-163">参数名称</span><span class="sxs-lookup"><span data-stu-id="3d362-163">Parameter name</span></span> | <span data-ttu-id="3d362-164">值</span><span class="sxs-lookup"><span data-stu-id="3d362-164">Value</span></span>  | <span data-ttu-id="3d362-165">说明</span><span class="sxs-lookup"><span data-stu-id="3d362-165">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3d362-166">_siteId_</span><span class="sxs-lookup"><span data-stu-id="3d362-166">_siteId_</span></span>       | <span data-ttu-id="3d362-167">string</span><span class="sxs-lookup"><span data-stu-id="3d362-167">string</span></span> | <span data-ttu-id="3d362-168">必需。</span><span class="sxs-lookup"><span data-stu-id="3d362-168">Required.</span></span> <span data-ttu-id="3d362-169">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="3d362-169">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="3d362-170">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="3d362-170">Get a drive by ID</span></span>

<span data-ttu-id="3d362-171">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="3d362-171">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="3d362-172">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3d362-172">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="3d362-173">路径参数</span><span class="sxs-lookup"><span data-stu-id="3d362-173">Path parameters</span></span>

| <span data-ttu-id="3d362-174">参数名称</span><span class="sxs-lookup"><span data-stu-id="3d362-174">Parameter name</span></span> | <span data-ttu-id="3d362-175">值</span><span class="sxs-lookup"><span data-stu-id="3d362-175">Value</span></span>  | <span data-ttu-id="3d362-176">说明</span><span class="sxs-lookup"><span data-stu-id="3d362-176">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="3d362-177">_driveId_</span><span class="sxs-lookup"><span data-stu-id="3d362-177">_driveId_</span></span>      | <span data-ttu-id="3d362-178">字符串</span><span class="sxs-lookup"><span data-stu-id="3d362-178">string</span></span> | <span data-ttu-id="3d362-p105">必需。 请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="3d362-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="3d362-181">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3d362-181">Optional query parameters</span></span>

<span data-ttu-id="3d362-182">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="3d362-182">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="3d362-183">响应</span><span class="sxs-lookup"><span data-stu-id="3d362-183">Response</span></span>

<span data-ttu-id="3d362-184">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="3d362-184">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="3d362-185">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="3d362-185">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="3d362-186">C#</span><span class="sxs-lookup"><span data-stu-id="3d362-186">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="3d362-187">Javascript</span><span class="sxs-lookup"><span data-stu-id="3d362-187">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="3d362-188">目标-C</span><span class="sxs-lookup"><span data-stu-id="3d362-188">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="3d362-189">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="3d362-189">Error response codes</span></span>

<span data-ttu-id="3d362-190">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="3d362-190">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
