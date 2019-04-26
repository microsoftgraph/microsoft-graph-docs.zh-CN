---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: d1d1ed77f2cebb7165ca0357cf5df3b20d0598b2
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326004"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="ffe72-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="ffe72-103">Restore deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ffe72-104">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="ffe72-104">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="ffe72-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="ffe72-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="ffe72-106">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="ffe72-106">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="ffe72-107">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="ffe72-107">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="ffe72-108">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="ffe72-108">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="ffe72-109">权限</span><span class="sxs-lookup"><span data-stu-id="ffe72-109">Permissions</span></span>
<span data-ttu-id="ffe72-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ffe72-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="ffe72-112">对于用户: directory.accessasuser.all 的所有用户。</span><span class="sxs-lookup"><span data-stu-id="ffe72-112">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="ffe72-113">对于组: directory.accessasuser.all 和 all 的组</span><span class="sxs-lookup"><span data-stu-id="ffe72-113">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ffe72-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ffe72-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="ffe72-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="ffe72-115">Request headers</span></span>
| <span data-ttu-id="ffe72-116">名称</span><span class="sxs-lookup"><span data-stu-id="ffe72-116">Name</span></span>       | <span data-ttu-id="ffe72-117">说明</span><span class="sxs-lookup"><span data-stu-id="ffe72-117">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ffe72-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="ffe72-118">Authorization</span></span>  | <span data-ttu-id="ffe72-119">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="ffe72-119">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="ffe72-120">接受</span><span class="sxs-lookup"><span data-stu-id="ffe72-120">Accept</span></span> | <span data-ttu-id="ffe72-121">application/json</span><span class="sxs-lookup"><span data-stu-id="ffe72-121">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="ffe72-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="ffe72-122">Request body</span></span>
<span data-ttu-id="ffe72-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ffe72-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ffe72-124">响应</span><span class="sxs-lookup"><span data-stu-id="ffe72-124">Response</span></span>

<span data-ttu-id="ffe72-125">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ffe72-125">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffe72-126">示例</span><span class="sxs-lookup"><span data-stu-id="ffe72-126">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ffe72-127">请求</span><span class="sxs-lookup"><span data-stu-id="ffe72-127">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="ffe72-128">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ffe72-128">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ffe72-129">响应</span><span class="sxs-lookup"><span data-stu-id="ffe72-129">Response</span></span>
<span data-ttu-id="ffe72-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ffe72-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "suppressions": []
}
-->
