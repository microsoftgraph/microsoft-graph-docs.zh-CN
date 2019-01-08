---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: 获取驱动器
ms.openlocfilehash: 903eb9d5886bf2ec3b7f8672438f01482e754f9b
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748589"
---
# <a name="get-drive"></a><span data-ttu-id="6d7a2-102">获取驱动器</span><span class="sxs-lookup"><span data-stu-id="6d7a2-102">Get Drive</span></span>

> <span data-ttu-id="6d7a2-103">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6d7a2-104">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6d7a2-105">检索 [Drive](../resources/drive.md) 资源的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-105">Retrieve the properties and relationships of a [Drive](../resources/drive.md) resource.</span></span>

<span data-ttu-id="6d7a2-106">驱动器是文件系统的顶级容器，例如 OneDrive 或 SharePoint 文档库。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-106">A Drive is the top-level container for a file system, such as OneDrive or SharePoint document libraries.</span></span>

## <a name="permissions"></a><span data-ttu-id="6d7a2-107">权限</span><span class="sxs-lookup"><span data-stu-id="6d7a2-107">Permissions</span></span>

<span data-ttu-id="6d7a2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d7a2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d7a2-110">Permission type</span></span>      | <span data-ttu-id="6d7a2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6d7a2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6d7a2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d7a2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="6d7a2-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d7a2-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d7a2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d7a2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6d7a2-115">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d7a2-115">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="6d7a2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d7a2-116">Application</span></span> | <span data-ttu-id="6d7a2-117">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6d7a2-117">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="get-current-users-onedrive"></a><span data-ttu-id="6d7a2-118">获取当前用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="6d7a2-118">Get current user's OneDrive</span></span>

<span data-ttu-id="6d7a2-119">可以通过 `me` 单一实例访问登录用户的驱动器（如果使用委派身份验证）。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-119">The signed in user's drive (when using delegated authentication) can be accessed from the `me` singleton.</span></span>

<span data-ttu-id="6d7a2-120">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-120">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="6d7a2-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d7a2-121">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-default", "scopes": "files.read" } -->

```http
GET /me/drive
```

## <a name="get-a-users-onedrive"></a><span data-ttu-id="6d7a2-122">获取用户的 OneDrive</span><span class="sxs-lookup"><span data-stu-id="6d7a2-122">Get a user's OneDrive</span></span>

<span data-ttu-id="6d7a2-123">若要访问用户的 OneDrive 或 OneDrive for Business，应用必须请求对 User 资源获取 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-123">To access a user's OneDrive or OneDrive for Business, your app must request the **drive** relationship on the User resource.</span></span>

<span data-ttu-id="6d7a2-124">如果未设置用户的 OneDrive，但用户有使用 OneDrive 的许可，那么在使用委派身份验证时，该请求将自动设置用户驱动器。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-124">If a user's OneDrive is not provisioned but the user has a license to use OneDrive, this request will automatically provision the user's drive, when using delegated authentication.</span></span>

### <a name="http-request"></a><span data-ttu-id="6d7a2-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d7a2-125">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-user", "scopes": "files.read.all" } -->

```http
GET /users/{idOrUserPrincipalName}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="6d7a2-126">路径参数</span><span class="sxs-lookup"><span data-stu-id="6d7a2-126">Path parameters</span></span>

| <span data-ttu-id="6d7a2-127">参数名称</span><span class="sxs-lookup"><span data-stu-id="6d7a2-127">Parameter name</span></span> | <span data-ttu-id="6d7a2-128">值</span><span class="sxs-lookup"><span data-stu-id="6d7a2-128">Value</span></span>  | <span data-ttu-id="6d7a2-129">说明</span><span class="sxs-lookup"><span data-stu-id="6d7a2-129">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6d7a2-130">_idOrUserPrincipalName_</span><span class="sxs-lookup"><span data-stu-id="6d7a2-130">_idOrUserPrincipalName_</span></span>     | <span data-ttu-id="6d7a2-131">string</span><span class="sxs-lookup"><span data-stu-id="6d7a2-131">string</span></span> | <span data-ttu-id="6d7a2-132">必需。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-132">Required.</span></span> <span data-ttu-id="6d7a2-133">拥有 OneDrive 的用户对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-133">The identifier for the user object who owns the OneDrive.</span></span> |

## <a name="get-the-document-library-associated-with-a-group"></a><span data-ttu-id="6d7a2-134">获取与组关联的文档库</span><span class="sxs-lookup"><span data-stu-id="6d7a2-134">Get the document library associated with a group</span></span>

<span data-ttu-id="6d7a2-135">若要访问组的默认文档库，你的应用程序应请求组中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-135">To access a Group's default document library, your app requests the **drive** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="6d7a2-136">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d7a2-136">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-group", "scopes": "group.read.all" } -->

```http
GET /groups/{groupId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="6d7a2-137">路径参数</span><span class="sxs-lookup"><span data-stu-id="6d7a2-137">Path parameters</span></span>

| <span data-ttu-id="6d7a2-138">参数名称</span><span class="sxs-lookup"><span data-stu-id="6d7a2-138">Parameter name</span></span> | <span data-ttu-id="6d7a2-139">值</span><span class="sxs-lookup"><span data-stu-id="6d7a2-139">Value</span></span>  | <span data-ttu-id="6d7a2-140">说明</span><span class="sxs-lookup"><span data-stu-id="6d7a2-140">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6d7a2-141">_groupId_</span><span class="sxs-lookup"><span data-stu-id="6d7a2-141">_groupId_</span></span>      | <span data-ttu-id="6d7a2-142">string</span><span class="sxs-lookup"><span data-stu-id="6d7a2-142">string</span></span> | <span data-ttu-id="6d7a2-143">必需。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-143">Required.</span></span> <span data-ttu-id="6d7a2-144">拥有文档库的组的标识符。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-144">The identifier for the group which owns the document library.</span></span> |

## <a name="get-the-document-library-for-a-site"></a><span data-ttu-id="6d7a2-145">获取某个站点的文档库</span><span class="sxs-lookup"><span data-stu-id="6d7a2-145">Get the document library for a site</span></span>

<span data-ttu-id="6d7a2-146">为了访问[站点的](../resources/site.md)默认文档库，你的应用程序应请求站点中的 **drive** 关系。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-146">To access a [Site's](../resources/site.md) default document library, your app requests the **drive** relationship on the Site.</span></span>

### <a name="http-request"></a><span data-ttu-id="6d7a2-147">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d7a2-147">HTTP request</span></span>

```http
GET /sites/{siteId}/drive
```

### <a name="path-parameters"></a><span data-ttu-id="6d7a2-148">路径参数</span><span class="sxs-lookup"><span data-stu-id="6d7a2-148">Path parameters</span></span>

| <span data-ttu-id="6d7a2-149">参数名称</span><span class="sxs-lookup"><span data-stu-id="6d7a2-149">Parameter name</span></span> | <span data-ttu-id="6d7a2-150">值</span><span class="sxs-lookup"><span data-stu-id="6d7a2-150">Value</span></span>  | <span data-ttu-id="6d7a2-151">说明</span><span class="sxs-lookup"><span data-stu-id="6d7a2-151">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6d7a2-152">_siteId_</span><span class="sxs-lookup"><span data-stu-id="6d7a2-152">_siteId_</span></span>       | <span data-ttu-id="6d7a2-153">string</span><span class="sxs-lookup"><span data-stu-id="6d7a2-153">string</span></span> | <span data-ttu-id="6d7a2-154">必需。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-154">Required.</span></span> <span data-ttu-id="6d7a2-155">包含文档库的站点的标识符。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-155">The identifier for the site that contains the document library.</span></span> |

## <a name="get-a-drive-by-id"></a><span data-ttu-id="6d7a2-156">根据 ID 获取驱动器</span><span class="sxs-lookup"><span data-stu-id="6d7a2-156">Get a drive by ID</span></span>

<span data-ttu-id="6d7a2-157">如果你有某个驱动器的唯一标识符，则可以直接从顶级驱动器集合来访问它。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-157">If you have the unique identifier for a drive, you can access it directly from the top-level drives collection.</span></span>

### <a name="http-request"></a><span data-ttu-id="6d7a2-158">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d7a2-158">HTTP request</span></span>

<!-- { "blockType": "request", "name": "get-drive-by-id", "scopes": "files.read" } -->

```http
GET /drives/{driveId}
```

### <a name="path-parameters"></a><span data-ttu-id="6d7a2-159">路径参数</span><span class="sxs-lookup"><span data-stu-id="6d7a2-159">Path parameters</span></span>

| <span data-ttu-id="6d7a2-160">参数名称</span><span class="sxs-lookup"><span data-stu-id="6d7a2-160">Parameter name</span></span> | <span data-ttu-id="6d7a2-161">值</span><span class="sxs-lookup"><span data-stu-id="6d7a2-161">Value</span></span>  | <span data-ttu-id="6d7a2-162">说明</span><span class="sxs-lookup"><span data-stu-id="6d7a2-162">Description</span></span>                                       |
|:---------------|:-------|:--------------------------------------------------|
| <span data-ttu-id="6d7a2-163">_driveId_</span><span class="sxs-lookup"><span data-stu-id="6d7a2-163">_driveId_</span></span>      | <span data-ttu-id="6d7a2-164">string</span><span class="sxs-lookup"><span data-stu-id="6d7a2-164">string</span></span> | <span data-ttu-id="6d7a2-165">必需。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-165">Required.</span></span> <span data-ttu-id="6d7a2-166">请求获取的驱动器的标识符。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-166">The identifier for the drive requested.</span></span> |

## <a name="optional-query-parameters"></a><span data-ttu-id="6d7a2-167">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6d7a2-167">Optional query parameters</span></span>

<span data-ttu-id="6d7a2-168">这些方法支持 [$select 查询参数][odata-query-parameters]塑造响应。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-168">These method support the [$select query parameter][odata-query-parameters] to shape the response.</span></span>

## <a name="response"></a><span data-ttu-id="6d7a2-169">响应</span><span class="sxs-lookup"><span data-stu-id="6d7a2-169">Response</span></span>

<span data-ttu-id="6d7a2-170">每个方法将在响应正文中返回匹配驱动器的 [Drive 资源][drive-resource]。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-170">Each of these methods returns a [Drive resource][drive-resource] for the matching drive in the response body.</span></span>

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

### <a name="error-response-codes"></a><span data-ttu-id="6d7a2-171">错误响应代码</span><span class="sxs-lookup"><span data-stu-id="6d7a2-171">Error response codes</span></span>

<span data-ttu-id="6d7a2-172">如果驱动器不存在且无法自动设置（当使用委派身份验证），将返回 `HTTP 404` 响应。</span><span class="sxs-lookup"><span data-stu-id="6d7a2-172">If the drive does not exist and cannot be provisioned automatically (when using delegated authentication) an `HTTP 404` response will be returned.</span></span>

[drive-resource]: ../resources/drive.md
[odata-query-parameters]: /graph/query-parameters

<!-- {
  "type": "#page.annotation",
  "description": "Get metadata for a OneDrive, OneDrive for Business, or Office 365 group drive",
  "keywords": "drive,onedrive,default drive,group drive",
  "section": "documentation",
  "tocPath": "Drives/Get drive"
} -->
