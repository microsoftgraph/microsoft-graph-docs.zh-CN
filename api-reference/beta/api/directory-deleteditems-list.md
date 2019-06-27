---
title: 列出已删除的项目
description: 从已删除的项目中检索最近删除的项目列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 31a5336ec1a01b61b522e826daa28efcde9bf9c9
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260870"
---
# <a name="list-deleted-items"></a><span data-ttu-id="f6e64-103">列出已删除的项目</span><span class="sxs-lookup"><span data-stu-id="f6e64-103">List deleted items</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f6e64-104">从[已删除的项目](../resources/directory.md)中检索最近删除的项目列表。</span><span class="sxs-lookup"><span data-stu-id="f6e64-104">Retrieve a list of recently deleted items from [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="f6e64-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="f6e64-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="f6e64-106">权限</span><span class="sxs-lookup"><span data-stu-id="f6e64-106">Permissions</span></span>
<span data-ttu-id="f6e64-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f6e64-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="f6e64-109">对于用户: Directory.accessasuser.all、全部、全部读取、全部、全部、全部、全部、目录</span><span class="sxs-lookup"><span data-stu-id="f6e64-109">For users: User.Read.All, Directory.Read.All, User.ReadWrite.All, Directory.AccessAsUser.All</span></span>
* <span data-ttu-id="f6e64-110">对于 groups: Group. All、Directory.accessasuser.all、Group 写 All、all、all。 All</span><span class="sxs-lookup"><span data-stu-id="f6e64-110">For groups: Group.Read.All, Directory.Read.All, Group.ReadWrite.All, Directory.AccessAsUser.All</span></span>

## <a name="http-request"></a><span data-ttu-id="f6e64-111">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f6e64-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http 
GET /directory/deleteditems/microsoft.graph.group
GET /directory/deletedItems/microsoft.graph.user
```

<span data-ttu-id="f6e64-112">此 API 当前支持从已删除的项目中检索组 (microsoft.graph.group) 或用户 (microsoft.graph.user) 的对象类型。</span><span class="sxs-lookup"><span data-stu-id="f6e64-112">This API currently supports retrieving object types of groups (microsoft.graph.group) or users (microsoft.graph.user) from deleted items.</span></span> <span data-ttu-id="f6e64-113">类型指定为 URI 的必需部分。</span><span class="sxs-lookup"><span data-stu-id="f6e64-113">The type is specified as a required part of the URI.</span></span> <span data-ttu-id="f6e64-114">不支持在没有类型的情况下调用 GET /directory/deleteditems。</span><span class="sxs-lookup"><span data-stu-id="f6e64-114">Calling GET /directory/deleteditems without a type is not supported.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="f6e64-115">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f6e64-115">Optional query parameters</span></span>
<span data-ttu-id="f6e64-116">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f6e64-116">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f6e64-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="f6e64-117">Request headers</span></span>
| <span data-ttu-id="f6e64-118">名称</span><span class="sxs-lookup"><span data-stu-id="f6e64-118">Name</span></span>      |<span data-ttu-id="f6e64-119">说明</span><span class="sxs-lookup"><span data-stu-id="f6e64-119">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="f6e64-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="f6e64-120">Authorization</span></span>  | <span data-ttu-id="f6e64-121">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="f6e64-121">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="f6e64-122">接受</span><span class="sxs-lookup"><span data-stu-id="f6e64-122">Accept</span></span>  | <span data-ttu-id="f6e64-123">application/json</span><span class="sxs-lookup"><span data-stu-id="f6e64-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="f6e64-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f6e64-124">Request body</span></span>
<span data-ttu-id="f6e64-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f6e64-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f6e64-126">响应</span><span class="sxs-lookup"><span data-stu-id="f6e64-126">Response</span></span>

<span data-ttu-id="f6e64-127">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f6e64-127">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f6e64-128">示例</span><span class="sxs-lookup"><span data-stu-id="f6e64-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f6e64-129">请求</span><span class="sxs-lookup"><span data-stu-id="f6e64-129">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_deleteditems"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/microsoft.graph.group
```
##### <a name="response"></a><span data-ttu-id="f6e64-130">响应</span><span class="sxs-lookup"><span data-stu-id="f6e64-130">Response</span></span>
<span data-ttu-id="f6e64-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f6e64-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="f6e64-133">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f6e64-133">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f6e64-134">C#</span><span class="sxs-lookup"><span data-stu-id="f6e64-134">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_deleteditems-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f6e64-135">Javascript</span><span class="sxs-lookup"><span data-stu-id="f6e64-135">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_deleteditems-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="f6e64-136">目标-C</span><span class="sxs-lookup"><span data-stu-id="f6e64-136">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_deleteditems-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List deleteditems",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-list.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
