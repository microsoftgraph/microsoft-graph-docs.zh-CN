---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "获取驱动器"
ms.openlocfilehash: 91a140dbcb1550bc850656452a6fa24a84dd5500
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="get-drive"></a><span data-ttu-id="4c35e-102">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="4c35e-102">Get Drive</span></span>

<span data-ttu-id="4c35e-103">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4c35e-103">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="4c35e-104">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="4c35e-104">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="4c35e-105">权限</span><span class="sxs-lookup"><span data-stu-id="4c35e-105">Permissions</span></span>

<span data-ttu-id="4c35e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="4c35e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c35e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c35e-108">Permission type</span></span>      | <span data-ttu-id="4c35e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c35e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c35e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c35e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="4c35e-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c35e-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c35e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c35e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4c35e-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c35e-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="4c35e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c35e-114">Application</span></span> | <span data-ttu-id="4c35e-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c35e-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="4c35e-116">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="4c35e-116">Get a user's OneDrive</span></span>

<span data-ttu-id="4c35e-117">可以通过 `me` 单一实例访问登录用户驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="4c35e-117">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="4c35e-118">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="4c35e-118">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="4c35e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c35e-119">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="4c35e-120">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="4c35e-120">Get a user's OneDrive</span></span>

<span data-ttu-id="4c35e-121">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="4c35e-121">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="4c35e-122">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="4c35e-122">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="4c35e-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c35e-123">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="4c35e-124">路径参数</span><span class="sxs-lookup"><span data-stu-id="4c35e-124">Path parameters</span></span>

| <span data-ttu-id="4c35e-125">参数名称</span><span class="sxs-lookup"><span data-stu-id="4c35e-125">Parameter name</span></span> | <span data-ttu-id="4c35e-126">值</span><span class="sxs-lookup"><span data-stu-id="4c35e-126">Value</span></span>  | <span data-ttu-id="4c35e-127">说明</span><span class="sxs-lookup"><span data-stu-id="4c35e-127">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="4c35e-128">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="4c35e-128">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="4c35e-129">string</span><span class="sxs-lookup"><span data-stu-id="4c35e-129">string</span></span> | <span data-ttu-id="4c35e-130">必需。</span><span class="sxs-lookup"><span data-stu-id="4c35e-130">Required.</span></span> <span data-ttu-id="4c35e-131">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="4c35e-131">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="4c35e-132">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="4c35e-132">Get the document library associated with a group</span></span>

<span data-ttu-id="4c35e-133">若要访问组的默认文档库，应用应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="4c35e-133">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="4c35e-134">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c35e-134">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="4c35e-135">路径参数</span><span class="sxs-lookup"><span data-stu-id="4c35e-135">Path parameters</span></span>

| <span data-ttu-id="4c35e-136">参数名称</span><span class="sxs-lookup"><span data-stu-id="4c35e-136">Parameter name</span></span> | <span data-ttu-id="4c35e-137">值</span><span class="sxs-lookup"><span data-stu-id="4c35e-137">Value</span></span>  | <span data-ttu-id="4c35e-138">说明</span><span class="sxs-lookup"><span data-stu-id="4c35e-138">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="4c35e-139">_groupId_</span><span class="sxs-lookup"><span data-stu-id="4c35e-139">_groupId_</span></span>      | <span data-ttu-id="4c35e-140">string</span><span class="sxs-lookup"><span data-stu-id="4c35e-140">string</span></span> | <span data-ttu-id="4c35e-141">必需。</span><span class="sxs-lookup"><span data-stu-id="4c35e-141">Required.</span></span> <span data-ttu-id="4c35e-142">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="4c35e-142">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="4c35e-143">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="4c35e-143">Get the document library for a site</span></span>

<span data-ttu-id="4c35e-144">若要访问[站点](../resources/site.md)的默认文档库，应用应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="4c35e-144">To access a [Group's](../resources/site.md) default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="4c35e-145">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c35e-145">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="4c35e-146">路径参数</span><span class="sxs-lookup"><span data-stu-id="4c35e-146">Path parameters</span></span>

| <span data-ttu-id="4c35e-147">参数名称</span><span class="sxs-lookup"><span data-stu-id="4c35e-147">Parameter name</span></span> | <span data-ttu-id="4c35e-148">值</span><span class="sxs-lookup"><span data-stu-id="4c35e-148">Value</span></span>  | <span data-ttu-id="4c35e-149">说明</span><span class="sxs-lookup"><span data-stu-id="4c35e-149">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="4c35e-150">_siteId_</span><span class="sxs-lookup"><span data-stu-id="4c35e-150">_siteId_</span></span>       | <span data-ttu-id="4c35e-151">string</span><span class="sxs-lookup"><span data-stu-id="4c35e-151">string</span></span> | <span data-ttu-id="4c35e-152">必需。</span><span class="sxs-lookup"><span data-stu-id="4c35e-152">Required.</span></span> <span data-ttu-id="4c35e-153">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="4c35e-153">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="4c35e-154">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="4c35e-154">Get a drive by ID</span></span>

<span data-ttu-id="4c35e-155">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="4c35e-155">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="4c35e-156">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c35e-156">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="4c35e-157">路径参数</span><span class="sxs-lookup"><span data-stu-id="4c35e-157">Path parameters</span></span>

| <span data-ttu-id="4c35e-158">参数名称</span><span class="sxs-lookup"><span data-stu-id="4c35e-158">Parameter name</span></span> | <span data-ttu-id="4c35e-159">值</span><span class="sxs-lookup"><span data-stu-id="4c35e-159">Value</span></span>  | <span data-ttu-id="4c35e-160">说明</span><span class="sxs-lookup"><span data-stu-id="4c35e-160">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="4c35e-161">_driveId_</span><span class="sxs-lookup"><span data-stu-id="4c35e-161">_drive-id_</span></span>      | <span data-ttu-id="4c35e-162">string</span><span class="sxs-lookup"><span data-stu-id="4c35e-162">string</span></span> | <span data-ttu-id="4c35e-163">必需。</span><span class="sxs-lookup"><span data-stu-id="4c35e-163">Required.</span></span> <span data-ttu-id="4c35e-164">请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="4c35e-164">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="4c35e-165">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="4c35e-165">Optional query parameters</span></span>

<span data-ttu-id="4c35e-166">这些方法支持使用 [$select 查询参数][odata-query-parameters]形成响应。</span><span class="sxs-lookup"><span data-stu-id="4c35e-166">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="http-response"></a><span data-ttu-id="4c35e-167">HTTP 响应</span><span class="sxs-lookup"><span data-stu-id="4c35e-167">HTTP response</span></span>

<span data-ttu-id="4c35e-168">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="4c35e-168">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="4c35e-169">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="4c35e-169">Error response codes</span></span>

<span data-ttu-id="4c35e-170">如果驱动器不存在且无法自动设置（使用委派身份验证时），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="4c35e-170">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: ../../../concepts/query_parameters.md

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
