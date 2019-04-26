---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 17bcf6c1d40afe1d1983141120ba8134a75e5c8a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33326024"
---
# <a name="list-deleted-items"></a><span data-ttu-id="76eed-103">列出已删除的项目</span><span class="sxs-lookup"><span data-stu-id="76eed-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76eed-104">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="76eed-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="76eed-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="76eed-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="76eed-106">权限</span><span class="sxs-lookup"><span data-stu-id="76eed-106">Permissions</span></span>
<span data-ttu-id="76eed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="76eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="76eed-109">对于用户: directory.accessasuser.all、全部、全部读取、全部、全部、全部、全部、目录</span><span class="sxs-lookup"><span data-stu-id="76eed-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="76eed-110">对于 groups: group. all、directory.accessasuser.all、Group 写 all、all、all。 all</span><span class="sxs-lookup"><span data-stu-id="76eed-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="76eed-111">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="76eed-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="76eed-112">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="76eed-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="76eed-113">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="76eed-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="76eed-114">不支持在没有类型的情况下调用 GET /directory/deleteditems。</span><span class="sxs-lookup"><span data-stu-id="76eed-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="76eed-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="76eed-115">Optional query parameters</span></span>
<span data-ttu-id="76eed-116">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="76eed-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="76eed-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="76eed-117">Request headers</span></span>
| <span data-ttu-id="76eed-118">名称</span><span class="sxs-lookup"><span data-stu-id="76eed-118">Name</span></span>      |<span data-ttu-id="76eed-119">说明</span><span class="sxs-lookup"><span data-stu-id="76eed-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="76eed-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="76eed-120">Authorization</span></span>  | <span data-ttu-id="76eed-121">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="76eed-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="76eed-122">接受</span><span class="sxs-lookup"><span data-stu-id="76eed-122">Accept</span></span>  | <span data-ttu-id="76eed-123">application/json</span><span class="sxs-lookup"><span data-stu-id="76eed-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="76eed-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="76eed-124">Request body</span></span>
<span data-ttu-id="76eed-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="76eed-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="76eed-126">响应</span><span class="sxs-lookup"><span data-stu-id="76eed-126">Response</span></span>

<span data-ttu-id="76eed-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="76eed-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="76eed-128">示例</span><span class="sxs-lookup"><span data-stu-id="76eed-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="76eed-129">请求</span><span class="sxs-lookup"><span data-stu-id="76eed-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="76eed-130">响应</span><span class="sxs-lookup"><span data-stu-id="76eed-130">Response</span></span>
<span data-ttu-id="76eed-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="76eed-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
