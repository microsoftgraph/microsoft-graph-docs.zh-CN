---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Priority
ms.prod: sharepoint
ms.openlocfilehash: 47d068dd00223513ad0f49a784916e8a8185ea91
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466484"
---
# <a name="get-drive"></a><span data-ttu-id="0d794-102">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="0d794-102">Get Drive</span></span>

<span data-ttu-id="0d794-103">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0d794-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="0d794-104">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="0d794-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d794-105">权限</span><span class="sxs-lookup"><span data-stu-id="0d794-105">Permissions</span></span>

<span data-ttu-id="0d794-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d794-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d794-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d794-108">Permission type</span></span>      | <span data-ttu-id="0d794-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d794-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d794-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d794-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0d794-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d794-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d794-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d794-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d794-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d794-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="0d794-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d794-114">Application</span></span> | <span data-ttu-id="0d794-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d794-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="0d794-116">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="0d794-116">Get current user's OneDrive</span></span>

<span data-ttu-id="0d794-117">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="0d794-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="0d794-118">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="0d794-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="0d794-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d794-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d794-120">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0d794-120">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d794-121">C#</span><span class="sxs-lookup"><span data-stu-id="0d794-121">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-default-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d794-122">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d794-122">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-default-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

## <a name="get-a-users-onedrive"></a><span data-ttu-id="0d794-123">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="0d794-123">Get a user's OneDrive</span></span>

<span data-ttu-id="0d794-124">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="0d794-124">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="0d794-125">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="0d794-125">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="0d794-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d794-126">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d794-127">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0d794-127">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d794-128">C#</span><span class="sxs-lookup"><span data-stu-id="0d794-128">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d794-129">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d794-129">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-user-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="0d794-130">路径参数</span><span class="sxs-lookup"><span data-stu-id="0d794-130">Path parameters</span></span>

| <span data-ttu-id="0d794-131">参数名称</span><span class="sxs-lookup"><span data-stu-id="0d794-131">Parameter name</span></span> | <span data-ttu-id="0d794-132">值</span><span class="sxs-lookup"><span data-stu-id="0d794-132">Value</span></span>  | <span data-ttu-id="0d794-133">说明</span><span class="sxs-lookup"><span data-stu-id="0d794-133">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0d794-134">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="0d794-134">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="0d794-135">string</span><span class="sxs-lookup"><span data-stu-id="0d794-135">string</span></span> | <span data-ttu-id="0d794-136">必需。</span><span class="sxs-lookup"><span data-stu-id="0d794-136">Required.</span></span> <span data-ttu-id="0d794-137">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d794-137">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="0d794-138">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="0d794-138">Get the document library associated with a group</span></span>

<span data-ttu-id="0d794-139">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="0d794-139">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="0d794-140">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d794-140">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d794-141">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0d794-141">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d794-142">C#</span><span class="sxs-lookup"><span data-stu-id="0d794-142">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d794-143">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d794-143">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-group-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="0d794-144">路径参数</span><span class="sxs-lookup"><span data-stu-id="0d794-144">Path parameters</span></span>

| <span data-ttu-id="0d794-145">参数名称</span><span class="sxs-lookup"><span data-stu-id="0d794-145">Parameter name</span></span> | <span data-ttu-id="0d794-146">值</span><span class="sxs-lookup"><span data-stu-id="0d794-146">Value</span></span>  | <span data-ttu-id="0d794-147">说明</span><span class="sxs-lookup"><span data-stu-id="0d794-147">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0d794-148">_groupId_</span><span class="sxs-lookup"><span data-stu-id="0d794-148">_groupId_</span></span>      | <span data-ttu-id="0d794-149">string</span><span class="sxs-lookup"><span data-stu-id="0d794-149">string</span></span> | <span data-ttu-id="0d794-150">必需。</span><span class="sxs-lookup"><span data-stu-id="0d794-150">Required.</span></span> <span data-ttu-id="0d794-151">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d794-151">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="0d794-152">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="0d794-152">Get the document library for a site</span></span>

<span data-ttu-id="0d794-153">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="0d794-153">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="0d794-154">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d794-154">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```http
GET /sites/{siteId}/drive
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d794-155">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0d794-155">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d794-156">C#</span><span class="sxs-lookup"><span data-stu-id="0d794-156">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d794-157">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d794-157">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-site-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="path-parameters"></a><span data-ttu-id="0d794-158">路径参数</span><span class="sxs-lookup"><span data-stu-id="0d794-158">Path parameters</span></span>

| <span data-ttu-id="0d794-159">参数名称</span><span class="sxs-lookup"><span data-stu-id="0d794-159">Parameter name</span></span> | <span data-ttu-id="0d794-160">值</span><span class="sxs-lookup"><span data-stu-id="0d794-160">Value</span></span>  | <span data-ttu-id="0d794-161">说明</span><span class="sxs-lookup"><span data-stu-id="0d794-161">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0d794-162">_siteId_</span><span class="sxs-lookup"><span data-stu-id="0d794-162">_siteId_</span></span>       | <span data-ttu-id="0d794-163">string</span><span class="sxs-lookup"><span data-stu-id="0d794-163">string</span></span> | <span data-ttu-id="0d794-164">必需。</span><span class="sxs-lookup"><span data-stu-id="0d794-164">Required.</span></span> <span data-ttu-id="0d794-165">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d794-165">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="0d794-166">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="0d794-166">Get a drive by ID</span></span>

<span data-ttu-id="0d794-167">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="0d794-167">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="0d794-168">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d794-168">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="0d794-169">路径参数</span><span class="sxs-lookup"><span data-stu-id="0d794-169">Path parameters</span></span>

| <span data-ttu-id="0d794-170">参数名称</span><span class="sxs-lookup"><span data-stu-id="0d794-170">Parameter name</span></span> | <span data-ttu-id="0d794-171">值</span><span class="sxs-lookup"><span data-stu-id="0d794-171">Value</span></span>  | <span data-ttu-id="0d794-172">说明</span><span class="sxs-lookup"><span data-stu-id="0d794-172">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="0d794-173">_driveId_</span><span class="sxs-lookup"><span data-stu-id="0d794-173">_driveId_</span></span>      | <span data-ttu-id="0d794-174">字符串</span><span class="sxs-lookup"><span data-stu-id="0d794-174">string</span></span> | <span data-ttu-id="0d794-p105">必需。 请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="0d794-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="0d794-177">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0d794-177">Optional query parameters</span></span>

<span data-ttu-id="0d794-178">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="0d794-178">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="0d794-179">响应</span><span class="sxs-lookup"><span data-stu-id="0d794-179">Response</span></span>

<span data-ttu-id="0d794-180">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="0d794-180">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default" , "get-drive-by-site-id"] } -->

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0d794-181">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0d794-181">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0d794-182">C#</span><span class="sxs-lookup"><span data-stu-id="0d794-182">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0d794-183">Javascript</span><span class="sxs-lookup"><span data-stu-id="0d794-183">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get-drive-by-id-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

### <a name="error-response-codes"></a><span data-ttu-id="0d794-184">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="0d794-184">Error response codes</span></span>

<span data-ttu-id="0d794-185">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="0d794-185">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/drive-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)",
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
