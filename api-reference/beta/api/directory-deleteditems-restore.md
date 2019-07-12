---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ce665b06da098661de1ba27a9ea1648470e15ae0
ms.sourcegitcommit: 6720736406f21e40914b27ba28387adedf97fa56
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/12/2019
ms.locfileid: "35638970"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="255c6-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="255c6-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="255c6-104">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="255c6-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="255c6-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="255c6-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="255c6-106">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="255c6-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="255c6-107">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="255c6-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="255c6-108">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="255c6-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="255c6-109">权限</span><span class="sxs-lookup"><span data-stu-id="255c6-109">Permissions</span></span>
<span data-ttu-id="255c6-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="255c6-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="255c6-112">对于用户: Directory.accessasuser.all 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="255c6-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="255c6-113">对于组: Directory.accessasuser.all 和 all 的组</span><span class="sxs-lookup"><span data-stu-id="255c6-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="255c6-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="255c6-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="255c6-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="255c6-115">Request headers</span></span>
| <span data-ttu-id="255c6-116">名称</span><span class="sxs-lookup"><span data-stu-id="255c6-116">Name</span></span>       | <span data-ttu-id="255c6-117">说明</span><span class="sxs-lookup"><span data-stu-id="255c6-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="255c6-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="255c6-118">Authorization</span></span>  | <span data-ttu-id="255c6-119">必需&lt;的&gt; \*\* 持有者令牌</span><span class="sxs-lookup"><span data-stu-id="255c6-119">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="255c6-120">Content-type</span><span class="sxs-lookup"><span data-stu-id="255c6-120">Content-type</span></span> | <span data-ttu-id="255c6-121">application/json</span><span class="sxs-lookup"><span data-stu-id="255c6-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="255c6-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="255c6-122">Request body</span></span>
<span data-ttu-id="255c6-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="255c6-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="255c6-124">响应</span><span class="sxs-lookup"><span data-stu-id="255c6-124">Response</span></span>

<span data-ttu-id="255c6-125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="255c6-125">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="255c6-126">示例</span><span class="sxs-lookup"><span data-stu-id="255c6-126">Example</span></span>
### <a name="request"></a><span data-ttu-id="255c6-127">请求</span><span class="sxs-lookup"><span data-stu-id="255c6-127">Request</span></span>


# <a name="httptabhttp"></a>[<span data-ttu-id="255c6-128">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="255c6-128">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="255c6-129">C#</span><span class="sxs-lookup"><span data-stu-id="255c6-129">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="255c6-130">Javascript</span><span class="sxs-lookup"><span data-stu-id="255c6-130">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="255c6-131">目标-C</span><span class="sxs-lookup"><span data-stu-id="255c6-131">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="255c6-132">响应</span><span class="sxs-lookup"><span data-stu-id="255c6-132">Response</span></span>
<span data-ttu-id="255c6-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="255c6-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
  "@odata.type":"#microsoft.graph.group",
  "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
  "displayName":"SampleGroup",
  "groupTypes":["Unified"],
  "mail":"example@contoso.com",
  "mailEnabled":true,
  "mailNickname":"Example",
  "securityEnabled":false,
  "visibility":"Public"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
