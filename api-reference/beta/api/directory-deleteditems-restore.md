---
title: 恢复已删除的项目
description: '从已删除的项目中还原最近删除的项目。 '
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 8c9a6e84a723fc0087f3155e4b2e973e72276233
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935967"
---
# <a name="restore-deleted-item"></a><span data-ttu-id="8899e-103">恢复已删除的项目</span><span class="sxs-lookup"><span data-stu-id="8899e-103">Restore deleted item</span></span>

> <span data-ttu-id="8899e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8899e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8899e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8899e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8899e-106">从[已删除的项目](../resources/directory.md)中还原最近删除的项目。</span><span class="sxs-lookup"><span data-stu-id="8899e-106">Restores a recently deleted item from [deleted items](../resources/directory.md).</span></span> 

<span data-ttu-id="8899e-107">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="8899e-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span> <span data-ttu-id="8899e-108">如果意外删除项目，可完全还原该项目。</span><span class="sxs-lookup"><span data-stu-id="8899e-108">If an item was accidentally deleted, you can fully restore the item.</span></span>

<span data-ttu-id="8899e-109">最近删除的项目将保留最多 30 天的可用时间。</span><span class="sxs-lookup"><span data-stu-id="8899e-109">A recently deleted item will remain available for up to 30 days.</span></span> <span data-ttu-id="8899e-110">30 天后，该项目将永久删除。</span><span class="sxs-lookup"><span data-stu-id="8899e-110">After 30 days, the item is permanently deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="8899e-111">权限</span><span class="sxs-lookup"><span data-stu-id="8899e-111">Permissions</span></span>
<span data-ttu-id="8899e-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8899e-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="8899e-114">用户： User.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8899e-114">For users: User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="8899e-115">组： Group.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8899e-115">For groups: Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="8899e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8899e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directory/deleteditems/{id}/restore
```

## <a name="request-headers"></a><span data-ttu-id="8899e-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="8899e-117">Request headers</span></span>
| <span data-ttu-id="8899e-118">名称</span><span class="sxs-lookup"><span data-stu-id="8899e-118">Name</span></span>       | <span data-ttu-id="8899e-119">说明</span><span class="sxs-lookup"><span data-stu-id="8899e-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="8899e-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="8899e-120">Authorization</span></span>  | <span data-ttu-id="8899e-121">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="8899e-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="8899e-122">Accept</span><span class="sxs-lookup"><span data-stu-id="8899e-122">Accept</span></span> | <span data-ttu-id="8899e-123">application/json</span><span class="sxs-lookup"><span data-stu-id="8899e-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8899e-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8899e-124">Request body</span></span>
<span data-ttu-id="8899e-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8899e-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8899e-126">响应</span><span class="sxs-lookup"><span data-stu-id="8899e-126">Response</span></span>

<span data-ttu-id="8899e-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8899e-127">If successful, this method returns `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8899e-128">示例</span><span class="sxs-lookup"><span data-stu-id="8899e-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="8899e-129">请求</span><span class="sxs-lookup"><span data-stu-id="8899e-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_directory"
}-->
```http
POST https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb/restore
```
<span data-ttu-id="8899e-130">在请求正文中，提供 [directoryObject](../resources/directoryobject.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8899e-130">In the request body, supply a JSON representation of [directoryObject](../resources/directoryobject.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="8899e-131">响应</span><span class="sxs-lookup"><span data-stu-id="8899e-131">Response</span></span>
<span data-ttu-id="8899e-p105">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8899e-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Create deletedItem",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
