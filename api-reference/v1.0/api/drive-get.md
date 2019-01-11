---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取驱动器
localization_priority: Priority
ms.openlocfilehash: ffa7162b700fc4f3e9a13b98ca3cef501d870291
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27846310"
---
# <a name="get-drive"></a><span data-ttu-id="8225a-102">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="8225a-102">Get Drive</span></span>

<span data-ttu-id="8225a-103">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8225a-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="8225a-104">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="8225a-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="8225a-105">权限</span><span class="sxs-lookup"><span data-stu-id="8225a-105">Permissions</span></span>

<span data-ttu-id="8225a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8225a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8225a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="8225a-108">Permission type</span></span>      | <span data-ttu-id="8225a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8225a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8225a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8225a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="8225a-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225a-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="8225a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8225a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8225a-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225a-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="8225a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="8225a-114">Application</span></span> | <span data-ttu-id="8225a-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8225a-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="8225a-116">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="8225a-116">Get current user's OneDrive</span></span>

<span data-ttu-id="8225a-117">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="8225a-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="8225a-118">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="8225a-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="8225a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8225a-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read", "tags": "service.graph" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="8225a-120">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="8225a-120">Get a user's OneDrive</span></span>

<span data-ttu-id="8225a-121">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="8225a-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="8225a-122">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="8225a-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="8225a-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8225a-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all", "tags": "service.graph" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8225a-124">路径参数</span><span class="sxs-lookup"><span data-stu-id="8225a-124">Path parameters</span></span>

| <span data-ttu-id="8225a-125">参数名称</span><span class="sxs-lookup"><span data-stu-id="8225a-125">Parameter name</span></span> | <span data-ttu-id="8225a-126">值</span><span class="sxs-lookup"><span data-stu-id="8225a-126">Value</span></span>  | <span data-ttu-id="8225a-127">说明</span><span class="sxs-lookup"><span data-stu-id="8225a-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8225a-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="8225a-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="8225a-129">string</span><span class="sxs-lookup"><span data-stu-id="8225a-129">string</span></span> | <span data-ttu-id="8225a-130">必需。</span><span class="sxs-lookup"><span data-stu-id="8225a-130">Required.</span></span> <span data-ttu-id="8225a-131">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="8225a-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="8225a-132">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="8225a-132">Get the document library associated with a group</span></span>

<span data-ttu-id="8225a-133">若要访问组的默认文档库，你的应用程序应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="8225a-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="8225a-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8225a-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all", "tags": "service.graph" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8225a-135">路径参数</span><span class="sxs-lookup"><span data-stu-id="8225a-135">Path parameters</span></span>

| <span data-ttu-id="8225a-136">参数名称</span><span class="sxs-lookup"><span data-stu-id="8225a-136">Parameter name</span></span> | <span data-ttu-id="8225a-137">值</span><span class="sxs-lookup"><span data-stu-id="8225a-137">Value</span></span>  | <span data-ttu-id="8225a-138">说明</span><span class="sxs-lookup"><span data-stu-id="8225a-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8225a-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="8225a-139">_groupId_</span></span>      | <span data-ttu-id="8225a-140">string</span><span class="sxs-lookup"><span data-stu-id="8225a-140">string</span></span> | <span data-ttu-id="8225a-141">必需。</span><span class="sxs-lookup"><span data-stu-id="8225a-141">Required.</span></span> <span data-ttu-id="8225a-142">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="8225a-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="8225a-143">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="8225a-143">Get the document library for a site</span></span>

<span data-ttu-id="8225a-144">为了访问[站点的](../resources/site.md)默认文档库，你的应用程序应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="8225a-144">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="8225a-145">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8225a-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="8225a-146">路径参数</span><span class="sxs-lookup"><span data-stu-id="8225a-146">Path parameters</span></span>

| <span data-ttu-id="8225a-147">参数名称</span><span class="sxs-lookup"><span data-stu-id="8225a-147">Parameter name</span></span> | <span data-ttu-id="8225a-148">值</span><span class="sxs-lookup"><span data-stu-id="8225a-148">Value</span></span>  | <span data-ttu-id="8225a-149">说明</span><span class="sxs-lookup"><span data-stu-id="8225a-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8225a-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="8225a-150">_siteId_</span></span>       | <span data-ttu-id="8225a-151">string</span><span class="sxs-lookup"><span data-stu-id="8225a-151">string</span></span> | <span data-ttu-id="8225a-152">必需。</span><span class="sxs-lookup"><span data-stu-id="8225a-152">Required.</span></span> <span data-ttu-id="8225a-153">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="8225a-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="8225a-154">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="8225a-154">Get a drive by ID</span></span>

<span data-ttu-id="8225a-155">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="8225a-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="8225a-156">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8225a-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{drive-id}
```

### <a name="path-parameters"></a><span data-ttu-id="8225a-157">路径参数</span><span class="sxs-lookup"><span data-stu-id="8225a-157">Path parameters</span></span>

| <span data-ttu-id="8225a-158">参数名称</span><span class="sxs-lookup"><span data-stu-id="8225a-158">Parameter name</span></span> | <span data-ttu-id="8225a-159">值</span><span class="sxs-lookup"><span data-stu-id="8225a-159">Value</span></span>  | <span data-ttu-id="8225a-160">说明</span><span class="sxs-lookup"><span data-stu-id="8225a-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="8225a-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="8225a-161">_driveId_</span></span>      | <span data-ttu-id="8225a-162">string</span><span class="sxs-lookup"><span data-stu-id="8225a-162">string</span></span> | <span data-ttu-id="8225a-163">必需。</span><span class="sxs-lookup"><span data-stu-id="8225a-163">Required.</span></span> <span data-ttu-id="8225a-164">请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="8225a-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="8225a-165">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8225a-165">Optional query parameters</span></span>

<span data-ttu-id="8225a-166">这些方法支持 [$select 查询参数][odata-query-parameters]塑造响应。</span><span class="sxs-lookup"><span data-stu-id="8225a-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="8225a-167">响应</span><span class="sxs-lookup"><span data-stu-id="8225a-167">Response</span></span>

<span data-ttu-id="8225a-168">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="8225a-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

<!-- { "blockType": "response", "@odata.type": "microsoft.graph.drive", "truncated": true, "name": ["get-drive-by-id", "get-drive-by-group", "get-drive-by-user", "get-drive-default"] } -->

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

### <a name="error-response-codes"></a><span data-ttu-id="8225a-169">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="8225a-169">Error response codes</span></span>

<span data-ttu-id="8225a-170">如果驱动器不存在且无法自动设置（当使用委派身份验证），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="8225a-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

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
