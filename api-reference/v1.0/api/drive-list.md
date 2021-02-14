---
author: JeremyKelley
ms.date: 09/10/2017
title: 列出驱动器
localization_priority: Priority
ms.prod: sharepoint
description: 检索可用于目标用户、群组或站点的 Drive 资源列表。
doc_type: apiPageType
ms.openlocfilehash: 5e2dd0b204e769695d0f8b31da01cadb5948aa13
ms.sourcegitcommit: 5b0aab5422e0619ce8806664c479479d223129ec
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/14/2021
ms.locfileid: "50240519"
---
# <a name="list-available-drives"></a><span data-ttu-id="45179-103">列出可用的驱动器</span><span class="sxs-lookup"><span data-stu-id="45179-103">List available drives</span></span>

<span data-ttu-id="45179-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45179-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="45179-105">检索可用于目标用户、组或[站点](../resources/site.md)的 [Drive](../resources/drive.md) 资源列表。</span><span class="sxs-lookup"><span data-stu-id="45179-105">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="45179-106">权限</span><span class="sxs-lookup"><span data-stu-id="45179-106">Permissions</span></span>

<span data-ttu-id="45179-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45179-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45179-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45179-109">Permission type</span></span>      | <span data-ttu-id="45179-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45179-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45179-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45179-111">Delegated (work or school account)</span></span> | <span data-ttu-id="45179-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45179-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="45179-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45179-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45179-114">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45179-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="45179-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45179-115">Application</span></span> | <span data-ttu-id="45179-116">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45179-116">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="45179-117">列出组的驱动器</span><span class="sxs-lookup"><span data-stu-id="45179-117">List a group's drives</span></span>

<span data-ttu-id="45179-118">若要列出某个组的文档库，应用应请求组中的 **drives** 关系。</span><span class="sxs-lookup"><span data-stu-id="45179-118">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="45179-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45179-119">HTTP request</span></span>


# <a name="http"></a>[<span data-ttu-id="45179-120">HTTP</span><span class="sxs-lookup"><span data-stu-id="45179-120">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /groups/{groupId}/drives
```
# <a name="c"></a>[<span data-ttu-id="45179-121">C#</span><span class="sxs-lookup"><span data-stu-id="45179-121">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/group-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45179-122">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45179-122">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/group-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45179-123">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45179-123">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/group-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45179-124">Java</span><span class="sxs-lookup"><span data-stu-id="45179-124">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/group-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-sites-drives"></a><span data-ttu-id="45179-125">列出站点的驱动器</span><span class="sxs-lookup"><span data-stu-id="45179-125">List a site's drives</span></span>

<span data-ttu-id="45179-126">若要列出某个站点的文档库，应用应请求站点中的 **drives** 关系。</span><span class="sxs-lookup"><span data-stu-id="45179-126">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>


# <a name="http"></a>[<span data-ttu-id="45179-127">HTTP</span><span class="sxs-lookup"><span data-stu-id="45179-127">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all", "tags": "service.graph" } -->

```msgraph-interactive
GET /sites/{siteId}/drives
```
# <a name="c"></a>[<span data-ttu-id="45179-128">C#</span><span class="sxs-lookup"><span data-stu-id="45179-128">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/site-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45179-129">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45179-129">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/site-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45179-130">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45179-130">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/site-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45179-131">Java</span><span class="sxs-lookup"><span data-stu-id="45179-131">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/site-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-a-users-drives"></a><span data-ttu-id="45179-132">列出用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="45179-132">List a user's drives</span></span>


# <a name="http"></a>[<span data-ttu-id="45179-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45179-133">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /users/{userId}/drives
```
# <a name="c"></a>[<span data-ttu-id="45179-134">C#</span><span class="sxs-lookup"><span data-stu-id="45179-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/user-list-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45179-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45179-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/user-list-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45179-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45179-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/user-list-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45179-137">Java</span><span class="sxs-lookup"><span data-stu-id="45179-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/user-list-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="list-the-current-users-drives"></a><span data-ttu-id="45179-138">列出当前用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="45179-138">List the current user's drives</span></span>


# <a name="http"></a>[<span data-ttu-id="45179-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="45179-139">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read", "tags": "service.graph" } -->

```msgraph-interactive
GET /me/drives
```
# <a name="c"></a>[<span data-ttu-id="45179-140">C#</span><span class="sxs-lookup"><span data-stu-id="45179-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/enum-drives-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45179-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45179-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/enum-drives-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45179-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45179-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/enum-drives-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45179-143">Java</span><span class="sxs-lookup"><span data-stu-id="45179-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/enum-drives-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


## <a name="optional-query-parameters"></a><span data-ttu-id="45179-144">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="45179-144">Optional query parameters</span></span>

<span data-ttu-id="45179-145">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](/graph/query-parameters)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="45179-145">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](/graph/query-parameters) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="45179-146">响应</span><span class="sxs-lookup"><span data-stu-id="45179-146">Response</span></span>

<span data-ttu-id="45179-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Drive](../resources/drive.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="45179-147">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="45179-148">备注</span><span class="sxs-lookup"><span data-stu-id="45179-148">Remarks</span></span>

<span data-ttu-id="45179-149">大多数用户将只有一个 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="45179-149">Most users will only have a single Drive resource.</span></span>

<span data-ttu-id="45179-150">组和站点可使用多个 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="45179-150">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="45179-151">默认情况下将隐藏包含 [system][] Facet 的 Drive。</span><span class="sxs-lookup"><span data-stu-id="45179-151">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="45179-152">若要列出它们，请在 `$select` 语句中包含 `system`。</span><span class="sxs-lookup"><span data-stu-id="45179-152">To list them, include `system` in your `$select` statement.</span></span>

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

