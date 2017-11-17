---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: "列出驱动器"
ms.openlocfilehash: 84771e589a65d11fc06707eb01b6211cf90a8581
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="list-available-drives"></a><span data-ttu-id="a5d41-102">列出可用的驱动器</span><span class="sxs-lookup"><span data-stu-id="a5d41-102">List available drives</span></span>

<span data-ttu-id="a5d41-103">检索可用于目标用户、组或[站点](../resources/site.md)的 [Drive](../resources/drive.md) 资源列表。</span><span class="sxs-lookup"><span data-stu-id="a5d41-103">Retrieve the list of [Drive](../resources/drive.md) resources available for a target User, Group, or [Site](../resources/site.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a5d41-104">权限</span><span class="sxs-lookup"><span data-stu-id="a5d41-104">Permissions</span></span>

<span data-ttu-id="a5d41-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a5d41-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a5d41-107">权限类型</span><span class="sxs-lookup"><span data-stu-id="a5d41-107">Permission type</span></span>      | <span data-ttu-id="a5d41-108">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a5d41-108">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a5d41-109">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a5d41-109">Delegated (work or school account)</span></span> | <span data-ttu-id="a5d41-110">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d41-110">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5d41-111">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a5d41-111">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a5d41-112">Files.Read、Files.ReadWrite、Files.Read.All、Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d41-112">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="a5d41-113">应用程序</span><span class="sxs-lookup"><span data-stu-id="a5d41-113">Application</span></span> | <span data-ttu-id="a5d41-114">Files.Read.All、Files.ReadWrite.All、Sites.Read.All、Sites.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5d41-114">Files.Read.All, Files.ReadWrite.All, Sites.Read.All, Sites.ReadWrite.All</span></span> |

## <a name="list-a-groups-drives"></a><span data-ttu-id="a5d41-115">列出组的驱动器</span><span class="sxs-lookup"><span data-stu-id="a5d41-115">List a group's drives</span></span>

<span data-ttu-id="a5d41-116">若要列出某个组的文档库，应用应请求组中的 **drives** 关系。</span><span class="sxs-lookup"><span data-stu-id="a5d41-116">To list the document libraries for a group, your app requests the **drives** relationship on the Group.</span></span>

### <a name="http-request"></a><span data-ttu-id="a5d41-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a5d41-117">HTTP request</span></span>

<!-- {"blockType": "request", "name": "group-list-drives", "scopes": "groups.read.all" } -->

```http
GET /groups/{groupId}/drives
```

## <a name="list-a-sites-drives"></a><span data-ttu-id="a5d41-118">列出站点的驱动器</span><span class="sxs-lookup"><span data-stu-id="a5d41-118">List a site's drives</span></span>

<span data-ttu-id="a5d41-119">若要列出某个站点的文档库，应用应请求站点中的 **drives** 关系。</span><span class="sxs-lookup"><span data-stu-id="a5d41-119">To list the document libraries for a site, your app requests the **drives** relationship on the Site.</span></span>

<!-- {"blockType": "request", "name": "site-list-drives", "scopes": "sites.read.all" } -->

```http
GET /sites/{siteId}/drives
```

## <a name="list-a-users-drives"></a><span data-ttu-id="a5d41-120">列出用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="a5d41-120">List a user's drives</span></span>

<!-- {"blockType": "request", "name": "user-list-drives", "scopes": "files.read.all" } -->

```http
GET /users/{userId}/drives
```

## <a name="list-the-current-users-drives"></a><span data-ttu-id="a5d41-121">列出当前用户的驱动器</span><span class="sxs-lookup"><span data-stu-id="a5d41-121">List the current user's drives</span></span>

<!-- {"blockType": "request", "name": "enum-drives", "scopes": "files.read" } -->

```http
GET /me/drives
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a5d41-122">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a5d41-122">Optional query parameters</span></span>

<span data-ttu-id="a5d41-123">此方法支持使用 `$expand`、`$select`、`$skipToken`、`$top` 和 `$orderby` [OData 查询参数](../../../concepts/query_parameters.md)自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a5d41-123">This method supports the `$expand`, `$select`, `$skipToken`, `$top`, and `$orderby` [OData query parameters](../../../concepts/query_parameters.md) to customize the response.</span></span>


## <a name="response"></a><span data-ttu-id="a5d41-124">响应</span><span class="sxs-lookup"><span data-stu-id="a5d41-124">Response</span></span>

<span data-ttu-id="a5d41-125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [Drive](../resources/drive.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a5d41-125">If successful, this method returns a `200 OK` response code and collection of [Drive](../resources/drive.md) objects in the response body.</span></span>

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

## <a name="remarks"></a><span data-ttu-id="a5d41-126">备注</span><span class="sxs-lookup"><span data-stu-id="a5d41-126">Remarks</span></span>

<span data-ttu-id="a5d41-127">大多数用户将只有一个 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="a5d41-127">Most users will only have a single Drive resource. Groups and some users may have multiple drive available.</span></span>

<span data-ttu-id="a5d41-128">组和站点可使用多个 Drive 资源。</span><span class="sxs-lookup"><span data-stu-id="a5d41-128">Groups and Sites may have multiple Drive resources available.</span></span>

<span data-ttu-id="a5d41-129">默认情况下将隐藏包含 [system][] Facet 的 Drive。</span><span class="sxs-lookup"><span data-stu-id="a5d41-129">Drives with the [system][] facet are hidden by default.</span></span>
<span data-ttu-id="a5d41-130">若要列出它们，请在 `$select` 语句中包含 `system`。</span><span class="sxs-lookup"><span data-stu-id="a5d41-130">To list them, include `system` in your `$select` statement.</span></span>

[system]: ../resources/systemFacet.md

<!-- {
  "type": "#page.annotation",
  "description": "List the available drives for a user, group, or site.",
  "keywords": "drive,onedrive.drive,list drives",
  "section": "documentation",
  "tocPath": "Drives/List drives"
} -->
