---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Priority
ms.prod: sharepoint
description: 检索 Drive 资源的属性和关系。
doc_type: apiPageType
ms.openlocfilehash: 5af01a9eea8cb8c362ca99cb22db467ff54e8d62
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36726961"
---
# <a name="get-drive"></a><span data-ttu-id="dc15b-103">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="dc15b-103">Get Drive</span></span>

<span data-ttu-id="dc15b-104">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dc15b-104">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="dc15b-105">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="dc15b-105">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="dc15b-106">权限</span><span class="sxs-lookup"><span data-stu-id="dc15b-106">Permissions</span></span>

<span data-ttu-id="dc15b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dc15b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dc15b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dc15b-109">Permission type</span></span>      | <span data-ttu-id="dc15b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dc15b-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dc15b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dc15b-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dc15b-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc15b-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc15b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dc15b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dc15b-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc15b-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="dc15b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dc15b-115">Application</span></span> | <span data-ttu-id="dc15b-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc15b-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="dc15b-117">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="dc15b-117">Get current user's OneDrive</span></span>

<span data-ttu-id="dc15b-118">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="dc15b-118">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="dc15b-119">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="dc15b-119">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="dc15b-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc15b-120">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc15b-121">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc15b-121">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc15b-122">C#</span><span class="sxs-lookup"><span data-stu-id="dc15b-122">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc15b-123">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc15b-123">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc15b-124">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc15b-124">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc15b-125">Java</span><span class="sxs-lookup"><span data-stu-id="dc15b-125">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="dc15b-126">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="dc15b-126">Get a user's OneDrive</span></span>

<span data-ttu-id="dc15b-127">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="dc15b-127">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="dc15b-128">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="dc15b-128">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="dc15b-129">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc15b-129">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc15b-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc15b-130">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc15b-131">C#</span><span class="sxs-lookup"><span data-stu-id="dc15b-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc15b-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc15b-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc15b-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc15b-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc15b-134">Java</span><span class="sxs-lookup"><span data-stu-id="dc15b-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="dc15b-135">路径参数</span><span class="sxs-lookup"><span data-stu-id="dc15b-135">Path parameters</span></span>

| <span data-ttu-id="dc15b-136">参数名称</span><span class="sxs-lookup"><span data-stu-id="dc15b-136">Parameter name</span></span> | <span data-ttu-id="dc15b-137">值</span><span class="sxs-lookup"><span data-stu-id="dc15b-137">Value</span></span>  | <span data-ttu-id="dc15b-138">说明</span><span class="sxs-lookup"><span data-stu-id="dc15b-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="dc15b-139">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="dc15b-139">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="dc15b-140">string</span><span class="sxs-lookup"><span data-stu-id="dc15b-140">string</span></span> | <span data-ttu-id="dc15b-141">必需。</span><span class="sxs-lookup"><span data-stu-id="dc15b-141">Required.</span></span> <span data-ttu-id="dc15b-142">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15b-142">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="dc15b-143">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="dc15b-143">Get the document library associated with a group</span></span>

<span data-ttu-id="dc15b-144">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="dc15b-144">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="dc15b-145">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc15b-145">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc15b-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc15b-146">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc15b-147">C#</span><span class="sxs-lookup"><span data-stu-id="dc15b-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc15b-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc15b-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc15b-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc15b-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc15b-150">Java</span><span class="sxs-lookup"><span data-stu-id="dc15b-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="dc15b-151">路径参数</span><span class="sxs-lookup"><span data-stu-id="dc15b-151">Path parameters</span></span>

| <span data-ttu-id="dc15b-152">参数名称</span><span class="sxs-lookup"><span data-stu-id="dc15b-152">Parameter name</span></span> | <span data-ttu-id="dc15b-153">值</span><span class="sxs-lookup"><span data-stu-id="dc15b-153">Value</span></span>  | <span data-ttu-id="dc15b-154">说明</span><span class="sxs-lookup"><span data-stu-id="dc15b-154">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="dc15b-155">_groupId_</span><span class="sxs-lookup"><span data-stu-id="dc15b-155">_groupId_</span></span>      | <span data-ttu-id="dc15b-156">string</span><span class="sxs-lookup"><span data-stu-id="dc15b-156">string</span></span> | <span data-ttu-id="dc15b-157">必需。</span><span class="sxs-lookup"><span data-stu-id="dc15b-157">Required.</span></span> <span data-ttu-id="dc15b-158">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15b-158">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="dc15b-159">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="dc15b-159">Get the document library for a site</span></span>

<span data-ttu-id="dc15b-160">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="dc15b-160">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="dc15b-161">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc15b-161">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc15b-162">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc15b-162">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc15b-163">C#</span><span class="sxs-lookup"><span data-stu-id="dc15b-163">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc15b-164">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc15b-164">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc15b-165">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc15b-165">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc15b-166">Java</span><span class="sxs-lookup"><span data-stu-id="dc15b-166">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="dc15b-167">路径参数</span><span class="sxs-lookup"><span data-stu-id="dc15b-167">Path parameters</span></span>

| <span data-ttu-id="dc15b-168">参数名称</span><span class="sxs-lookup"><span data-stu-id="dc15b-168">Parameter name</span></span> | <span data-ttu-id="dc15b-169">值</span><span class="sxs-lookup"><span data-stu-id="dc15b-169">Value</span></span>  | <span data-ttu-id="dc15b-170">说明</span><span class="sxs-lookup"><span data-stu-id="dc15b-170">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="dc15b-171">_siteId_</span><span class="sxs-lookup"><span data-stu-id="dc15b-171">_siteId_</span></span>       | <span data-ttu-id="dc15b-172">string</span><span class="sxs-lookup"><span data-stu-id="dc15b-172">string</span></span> | <span data-ttu-id="dc15b-173">必需。</span><span class="sxs-lookup"><span data-stu-id="dc15b-173">Required.</span></span> <span data-ttu-id="dc15b-174">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15b-174">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="dc15b-175">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="dc15b-175">Get a drive by ID</span></span>

<span data-ttu-id="dc15b-176">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="dc15b-176">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="dc15b-177">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dc15b-177">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="dc15b-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="dc15b-178">--Http</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="dc15b-179">C#</span><span class="sxs-lookup"><span data-stu-id="dc15b-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="dc15b-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dc15b-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="dc15b-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dc15b-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="dc15b-182">Java</span><span class="sxs-lookup"><span data-stu-id="dc15b-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="dc15b-183">路径参数</span><span class="sxs-lookup"><span data-stu-id="dc15b-183">Path parameters</span></span>

| <span data-ttu-id="dc15b-184">参数名称</span><span class="sxs-lookup"><span data-stu-id="dc15b-184">Parameter name</span></span> | <span data-ttu-id="dc15b-185">值</span><span class="sxs-lookup"><span data-stu-id="dc15b-185">Value</span></span>  | <span data-ttu-id="dc15b-186">说明</span><span class="sxs-lookup"><span data-stu-id="dc15b-186">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="dc15b-187">_driveId_</span><span class="sxs-lookup"><span data-stu-id="dc15b-187">_driveId_</span></span>      | <span data-ttu-id="dc15b-188">字符串</span><span class="sxs-lookup"><span data-stu-id="dc15b-188">string</span></span> | <span data-ttu-id="dc15b-p105">必需。 请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="dc15b-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="dc15b-191">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dc15b-191">Optional query parameters</span></span>

<span data-ttu-id="dc15b-192">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="dc15b-192">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="dc15b-193">响应</span><span class="sxs-lookup"><span data-stu-id="dc15b-193">Response</span></span>

<span data-ttu-id="dc15b-194">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="dc15b-194">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="dc15b-195">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="dc15b-195">Error response codes</span></span>

<span data-ttu-id="dc15b-196">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="dc15b-196">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "suppressions": [
      "Warning: /api-reference/v1.0/api/drive-get.md:
        Unable to map some markdown elements into schema.
            Unmapped methods:
        get-drive-default, get-drive-by-user, get-drive-by-group, get-drive-by-id
            Unmapped tables:
        Permissions - AuthScopes, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters, Path parameters - PathParameters"
  ],
  "tocPath": "Drives/Get drive"
} -->
