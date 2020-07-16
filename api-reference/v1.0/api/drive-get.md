---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Priority
ms.prod: sharepoint
description: 检索 Drive 资源的属性和关系。
doc_type: apiPageType
ms.openlocfilehash: 8538f44a368147ed8c8438ea61c95c94f037923f
ms.sourcegitcommit: 7153a13f4e95c7d9fed3f2c10a3d075ff87b368d
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/26/2020
ms.locfileid: "44897069"
---
# <a name="get-drive"></a><span data-ttu-id="fe39a-103">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="fe39a-103">Get Drive</span></span>

<span data-ttu-id="fe39a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe39a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe39a-105">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe39a-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="fe39a-106">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="fe39a-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe39a-107">权限</span><span class="sxs-lookup"><span data-stu-id="fe39a-107">Permissions</span></span>

<span data-ttu-id="fe39a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe39a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe39a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe39a-110">Permission type</span></span>      | <span data-ttu-id="fe39a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe39a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe39a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe39a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe39a-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe39a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe39a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe39a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe39a-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe39a-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="fe39a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe39a-116">Application</span></span> | <span data-ttu-id="fe39a-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fe39a-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="fe39a-118">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe39a-118">Get current user's OneDrive</span></span>

<span data-ttu-id="fe39a-119">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="fe39a-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="fe39a-120">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="fe39a-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="fe39a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe39a-121">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe39a-122">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe39a-122">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drive
```
# <a name="c"></a>[<span data-ttu-id="fe39a-123">C#</span><span class="sxs-lookup"><span data-stu-id="fe39a-123">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-default-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe39a-124">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe39a-124">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-default-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe39a-125">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe39a-125">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-default-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe39a-126">Java</span><span class="sxs-lookup"><span data-stu-id="fe39a-126">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-default-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="get-a-users-onedrive"></a><span data-ttu-id="fe39a-127">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="fe39a-127">Get a user's OneDrive</span></span>

<span data-ttu-id="fe39a-128">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="fe39a-128">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="fe39a-129">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="fe39a-129">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="fe39a-130">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe39a-130">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe39a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe39a-131">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{idOrUserPrincipalName}/drive
```
# <a name="c"></a>[<span data-ttu-id="fe39a-132">C#</span><span class="sxs-lookup"><span data-stu-id="fe39a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-user-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe39a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe39a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-user-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe39a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe39a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-user-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe39a-135">Java</span><span class="sxs-lookup"><span data-stu-id="fe39a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-user-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="fe39a-136">路径参数</span><span class="sxs-lookup"><span data-stu-id="fe39a-136">Path parameters</span></span>

| <span data-ttu-id="fe39a-137">参数名称</span><span class="sxs-lookup"><span data-stu-id="fe39a-137">Parameter name</span></span> | <span data-ttu-id="fe39a-138">值</span><span class="sxs-lookup"><span data-stu-id="fe39a-138">Value</span></span>  | <span data-ttu-id="fe39a-139">说明</span><span class="sxs-lookup"><span data-stu-id="fe39a-139">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="fe39a-140">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="fe39a-140">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="fe39a-141">string</span><span class="sxs-lookup"><span data-stu-id="fe39a-141">string</span></span> | <span data-ttu-id="fe39a-142">必需。</span><span class="sxs-lookup"><span data-stu-id="fe39a-142">Required.</span></span> <span data-ttu-id="fe39a-143">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="fe39a-143">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="fe39a-144">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="fe39a-144">Get the document library associated with a group</span></span>

<span data-ttu-id="fe39a-145">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="fe39a-145">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="fe39a-146">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe39a-146">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe39a-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe39a-147">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drive
```
# <a name="c"></a>[<span data-ttu-id="fe39a-148">C#</span><span class="sxs-lookup"><span data-stu-id="fe39a-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe39a-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe39a-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe39a-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe39a-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe39a-151">Java</span><span class="sxs-lookup"><span data-stu-id="fe39a-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="fe39a-152">路径参数</span><span class="sxs-lookup"><span data-stu-id="fe39a-152">Path parameters</span></span>

| <span data-ttu-id="fe39a-153">参数名称</span><span class="sxs-lookup"><span data-stu-id="fe39a-153">Parameter name</span></span> | <span data-ttu-id="fe39a-154">值</span><span class="sxs-lookup"><span data-stu-id="fe39a-154">Value</span></span>  | <span data-ttu-id="fe39a-155">说明</span><span class="sxs-lookup"><span data-stu-id="fe39a-155">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="fe39a-156">_groupId_</span><span class="sxs-lookup"><span data-stu-id="fe39a-156">_groupId_</span></span>      | <span data-ttu-id="fe39a-157">string</span><span class="sxs-lookup"><span data-stu-id="fe39a-157">string</span></span> | <span data-ttu-id="fe39a-158">必需。</span><span class="sxs-lookup"><span data-stu-id="fe39a-158">Required.</span></span> <span data-ttu-id="fe39a-159">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="fe39a-159">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="fe39a-160">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="fe39a-160">Get the document library for a site</span></span>

<span data-ttu-id="fe39a-161">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="fe39a-161">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="fe39a-162">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe39a-162">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe39a-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe39a-163">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-site-id", "scopes": "group.read.all" } -->

```msgraph-interactive
GET /sites/{siteId}/drive
```
# <a name="c"></a>[<span data-ttu-id="fe39a-164">C#</span><span class="sxs-lookup"><span data-stu-id="fe39a-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-site-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe39a-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe39a-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-site-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe39a-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe39a-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-site-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe39a-167">Java</span><span class="sxs-lookup"><span data-stu-id="fe39a-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-site-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="fe39a-168">路径参数</span><span class="sxs-lookup"><span data-stu-id="fe39a-168">Path parameters</span></span>

| <span data-ttu-id="fe39a-169">参数名称</span><span class="sxs-lookup"><span data-stu-id="fe39a-169">Parameter name</span></span> | <span data-ttu-id="fe39a-170">值</span><span class="sxs-lookup"><span data-stu-id="fe39a-170">Value</span></span>  | <span data-ttu-id="fe39a-171">说明</span><span class="sxs-lookup"><span data-stu-id="fe39a-171">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="fe39a-172">_siteId_</span><span class="sxs-lookup"><span data-stu-id="fe39a-172">_siteId_</span></span>       | <span data-ttu-id="fe39a-173">string</span><span class="sxs-lookup"><span data-stu-id="fe39a-173">string</span></span> | <span data-ttu-id="fe39a-174">必需。</span><span class="sxs-lookup"><span data-stu-id="fe39a-174">Required.</span></span> <span data-ttu-id="fe39a-175">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="fe39a-175">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="fe39a-176">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="fe39a-176">Get a drive by ID</span></span>

<span data-ttu-id="fe39a-177">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="fe39a-177">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="fe39a-178">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe39a-178">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="fe39a-179">HTTP</span><span class="sxs-lookup"><span data-stu-id="fe39a-179">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```msgraph-interactive
GET /drives/{drive-id}
```
# <a name="c"></a>[<span data-ttu-id="fe39a-180">C#</span><span class="sxs-lookup"><span data-stu-id="fe39a-180">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-drive-by-id-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fe39a-181">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fe39a-181">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-drive-by-id-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fe39a-182">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fe39a-182">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-drive-by-id-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fe39a-183">Java</span><span class="sxs-lookup"><span data-stu-id="fe39a-183">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-drive-by-id-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="path-parameters"></a><span data-ttu-id="fe39a-184">路径参数</span><span class="sxs-lookup"><span data-stu-id="fe39a-184">Path parameters</span></span>

| <span data-ttu-id="fe39a-185">参数名称</span><span class="sxs-lookup"><span data-stu-id="fe39a-185">Parameter name</span></span> | <span data-ttu-id="fe39a-186">值</span><span class="sxs-lookup"><span data-stu-id="fe39a-186">Value</span></span>  | <span data-ttu-id="fe39a-187">说明</span><span class="sxs-lookup"><span data-stu-id="fe39a-187">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="fe39a-188">_driveId_</span><span class="sxs-lookup"><span data-stu-id="fe39a-188">_driveId_</span></span>      | <span data-ttu-id="fe39a-189">字符串</span><span class="sxs-lookup"><span data-stu-id="fe39a-189">string</span></span> | <span data-ttu-id="fe39a-p105">必需。 请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="fe39a-p105">Required. The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="fe39a-192">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fe39a-192">Optional query parameters</span></span>

<span data-ttu-id="fe39a-193">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="fe39a-193">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="fe39a-194">响应</span><span class="sxs-lookup"><span data-stu-id="fe39a-194">Response</span></span>

<span data-ttu-id="fe39a-195">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="fe39a-195">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="fe39a-196">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="fe39a-196">Error response codes</span></span>

<span data-ttu-id="fe39a-197">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="fe39a-197">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Microsoft 365 group drive",
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
