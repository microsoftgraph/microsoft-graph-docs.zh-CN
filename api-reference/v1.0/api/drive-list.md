---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 列出驱动器
localization_priority: Priority
ms.prod: sharepoint
description: 检索可用于目标用户、群组或站点的 Drive 资源列表。
doc_type: apiPageType
ms.openlocfilehash: 33df5c00844a625976e07fca7bdcee57ad29aea7
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721185"
---
# <a name="list-available-drives"></a><span data-ttu-id="2c258-103">列出可用的驱动器</span><span class="sxs-lookup"><span data-stu-id="2c258-103">List available drives</span></span>

<span data-ttu-id="2c258-104">检索可用于目标用户、组或[站点](../resources/site.md)的 [Drive](../resources/drive.md) 资源列表。</span><span class="sxs-lookup"><span data-stu-id="2c258-104">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c258-105">权限</span><span class="sxs-lookup"><span data-stu-id="2c258-105">Permissions</span></span>

<span data-ttu-id="2c258-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c258-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2c258-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c258-108">Permission type</span></span>      | <span data-ttu-id="2c258-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c258-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2c258-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c258-110">Delegated (work or school account)</span></span> | <span data-ttu-id="2c258-111">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c258-111">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c258-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c258-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2c258-113">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c258-113">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="2c258-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c258-114">Application</span></span> | <span data-ttu-id="2c258-115">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c258-115">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="2c258-116">列出组的驱动器</span><span class="sxs-lookup"><span data-stu-id="2c258-116">List a group's drives</span></span>

<span data-ttu-id="2c258-117">若要列出某个组的文档库，应用应请求组中的 **drives** 关系。</span><span class="sxs-lookup"><span data-stu-id="2c258-117">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="2c258-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c258-118">HTTP request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2c258-119">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c258-119">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c258-120">C#</span><span class="sxs-lookup"><span data-stu-id="2c258-120">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c258-121">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c258-121">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c258-122">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c258-122">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2c258-123">Java</span><span class="sxs-lookup"><span data-stu-id="2c258-123">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="2c258-124">列出站点的驱动器</span><span class="sxs-lookup"><span data-stu-id="2c258-124">List a site's drives</span></span>

<span data-ttu-id="2c258-125">若要列出某个站点的文档库，应用应请求站点中的 **drives** 关系。</span><span class="sxs-lookup"><span data-stu-id="2c258-125">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2c258-126">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c258-126">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /sites/{siteId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c258-127">C#</span><span class="sxs-lookup"><span data-stu-id="2c258-127">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c258-128">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c258-128">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c258-129">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c258-129">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2c258-130">Java</span><span class="sxs-lookup"><span data-stu-id="2c258-130">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="2c258-131">列出用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="2c258-131">List a user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2c258-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c258-132">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{userId}/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c258-133">C#</span><span class="sxs-lookup"><span data-stu-id="2c258-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c258-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c258-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c258-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c258-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2c258-136">Java</span><span class="sxs-lookup"><span data-stu-id="2c258-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="2c258-137">列出当前用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="2c258-137">List the current user's drives</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="2c258-138">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c258-138">--Http</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drives
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="2c258-139">C#</span><span class="sxs-lookup"><span data-stu-id="2c258-139">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="2c258-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c258-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="2c258-141">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c258-141">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="2c258-142">Java</span><span class="sxs-lookup"><span data-stu-id="2c258-142">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="2c258-143">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2c258-143">Optional query parameters</span></span>

<span data-ttu-id="2c258-144">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2c258-144">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="2c258-145">响应</span><span class="sxs-lookup"><span data-stu-id="2c258-145">Response</span></span>

<span data-ttu-id="2c258-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Drive](../resources/drive.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c258-146">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

<!-- { "blockType": "response", 
       "@odata.type": "Collection(microsoft.graph.drive)",
       "name": ["group-list-drives", "site-list-drives", "user-list-drives", "enum-drives"],
       "truncated": true } -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "942CAEB0-13AE-491B-85E4-7557CDC0F25F",
      "driveType": "documentLibrary",
      "name": "Shared Documents",
      "owner": {
        "user": {
          "id": "AE2A1EE9-81A7-423C-ABE4-B945F47509BB",
          "displayName": "Ryan Gregg"
        }
      }
    },
    {
      "id": "C1CD3ED9-0E98-4B0B-82D3-C8FB784B9DCC",
      "driveType": "documentLibrary",
      "name": "Contoso Project Files",
      "owner": {
        "user": {
          "id": "406B2281-18E8-4416-9857-38C531B904F1",
          "displayName": "Daron Spektor"
        }
      }
    }
  ]
}
```

## <a name="remarks"></a><span data-ttu-id="2c258-147">备注</span><span class="sxs-lookup"><span data-stu-id="2c258-147">Remarks</span></span>

<span data-ttu-id="2c258-148">大多数用户将只有一个 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="2c258-148">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="2c258-149">组和站点可使用多个 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="2c258-149">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="2c258-150">默认情况下将隐藏包含 [system][] Facet 的 Drive。</span><span class="sxs-lookup"><span data-stu-id="2c258-150">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="2c258-151">若要列出它们，请在 `$select` 语句中包含 `system`。</span><span class="sxs-lookup"><span data-stu-id="2c258-151">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemfacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives",
  "suppressions": [
  ]
} -->
