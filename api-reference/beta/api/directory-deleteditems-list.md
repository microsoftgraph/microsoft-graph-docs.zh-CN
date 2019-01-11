---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: lleonard-msft
localization_priority: Normal
ms.openlocfilehash: ef23704c01a7d1b6cd3a85ffcab1dc34ded0936d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879434"
---
# <a name="list-deleted-items"></a><span data-ttu-id="5328c-103">列出已删除的项目</span><span class="sxs-lookup"><span data-stu-id="5328c-103">List deleted items</span></span>

> <span data-ttu-id="5328c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5328c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5328c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5328c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="5328c-106">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="5328c-106">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="5328c-107">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="5328c-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="5328c-108">权限</span><span class="sxs-lookup"><span data-stu-id="5328c-108">Permissions</span></span>
<span data-ttu-id="5328c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5328c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="5328c-111">用户： User.Read.All Directory.Read.All、 User.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5328c-111">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="5328c-112">组： Group.Read.All Directory.Read.All、 Group.ReadWrite.All、 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="5328c-112">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="5328c-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5328c-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="5328c-114">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="5328c-114">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="5328c-115">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="5328c-115">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="5328c-116">不支持在没有类型的情况下调用 GET /directory/deleteditems。</span><span class="sxs-lookup"><span data-stu-id="5328c-116">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="5328c-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5328c-117">Optional query parameters</span></span>
<span data-ttu-id="5328c-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5328c-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5328c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5328c-119">Request headers</span></span>
| <span data-ttu-id="5328c-120">名称</span><span class="sxs-lookup"><span data-stu-id="5328c-120">Name</span></span>      |<span data-ttu-id="5328c-121">说明</span><span class="sxs-lookup"><span data-stu-id="5328c-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="5328c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5328c-122">Authorization</span></span>  | <span data-ttu-id="5328c-123">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="5328c-123">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="5328c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="5328c-124">Accept</span></span>  | <span data-ttu-id="5328c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5328c-125">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="5328c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5328c-126">Request body</span></span>
<span data-ttu-id="5328c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5328c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5328c-128">响应</span><span class="sxs-lookup"><span data-stu-id="5328c-128">Response</span></span>

<span data-ttu-id="5328c-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5328c-129">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="5328c-130">示例</span><span class="sxs-lookup"><span data-stu-id="5328c-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="5328c-131">请求</span><span class="sxs-lookup"><span data-stu-id="5328c-131">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="5328c-132">响应</span><span class="sxs-lookup"><span data-stu-id="5328c-132">Response</span></span>
<span data-ttu-id="5328c-p104">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5328c-p104">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#groups",
  "value": [
    {
      "id":"46cc6179-19d0-473e-97ad-6ff84347bbbb",
      "displayName":"SampleGroup",
      "groupTypes":["Unified"],
      "mail":"example@contoso.com",
      "mailEnabled":true,
      "mailNickname":"Example",
      "securityEnabled":false,
      "visibility":"Public"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
