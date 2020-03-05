---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0c0a7a4e1e3087cf05eef023620eb273a62b9556
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42435316"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="bb8a0-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="bb8a0-103">Restore deleted item</span></span>

<span data-ttu-id="bb8a0-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="bb8a0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bb8a0-105">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-105">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="bb8a0-106">目前，仅支持[应用程序](../resources/application.md)、[组](../resources/group.md)和[用户](../resources/user.md)资源的 "已删除邮件" 功能。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-106">Currently, deleted items functionality is only supported for the [application](../resources/application.md), [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="bb8a0-107">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-107">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="bb8a0-108">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-108">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="bb8a0-109">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-109">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="bb8a0-110">权限</span><span class="sxs-lookup"><span data-stu-id="bb8a0-110">Permissions</span></span>
<span data-ttu-id="bb8a0-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="bb8a0-113">对于应用程序： Application.readwrite.ownedby、Directory.accessasuser.all、all、、all、。 All</span><span class="sxs-lookup"><span data-stu-id="bb8a0-113">For applications: Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="bb8a0-114">对于用户： Directory.accessasuser.all 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="bb8a0-115">对于组： Directory.accessasuser.all 和 all 的组</span><span class="sxs-lookup"><span data-stu-id="bb8a0-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="bb8a0-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bb8a0-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="bb8a0-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bb8a0-117">Request headers</span></span>
| <span data-ttu-id="bb8a0-118">名称</span><span class="sxs-lookup"><span data-stu-id="bb8a0-118">Name</span></span>       | <span data-ttu-id="bb8a0-119">说明</span><span class="sxs-lookup"><span data-stu-id="bb8a0-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="bb8a0-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bb8a0-120">Authorization</span></span>  | <span data-ttu-id="bb8a0-121">必需&lt;的&gt; \*\* 持有者令牌</span><span class="sxs-lookup"><span data-stu-id="bb8a0-121">Bearer &lt;token&gt; *Required*</span></span>|
| <span data-ttu-id="bb8a0-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="bb8a0-122">Content-type</span></span> | <span data-ttu-id="bb8a0-123">application/json</span><span class="sxs-lookup"><span data-stu-id="bb8a0-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="bb8a0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="bb8a0-124">Request body</span></span>
<span data-ttu-id="bb8a0-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bb8a0-126">响应</span><span class="sxs-lookup"><span data-stu-id="bb8a0-126">Response</span></span>

<span data-ttu-id="bb8a0-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-127">If successful, this method returns a `200 OK` response code and a [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bb8a0-128">示例</span><span class="sxs-lookup"><span data-stu-id="bb8a0-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="bb8a0-129">请求</span><span class="sxs-lookup"><span data-stu-id="bb8a0-129">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="bb8a0-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="bb8a0-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
# <a name="c"></a>[<span data-ttu-id="bb8a0-131">C#</span><span class="sxs-lookup"><span data-stu-id="bb8a0-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-directory-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="bb8a0-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bb8a0-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-directory-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="bb8a0-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bb8a0-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-directory-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="bb8a0-134">响应</span><span class="sxs-lookup"><span data-stu-id="bb8a0-134">Response</span></span>
<span data-ttu-id="bb8a0-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bb8a0-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
