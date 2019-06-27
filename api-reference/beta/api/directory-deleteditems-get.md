---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6f916a213c697698b76dcb8031409614eb63c16e
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35260884"
---
# <a name="get-deleted-item"></a><span data-ttu-id="d0447-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="d0447-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0447-104">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="d0447-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="d0447-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="d0447-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="d0447-106">权限</span><span class="sxs-lookup"><span data-stu-id="d0447-106">Permissions</span></span>
<span data-ttu-id="d0447-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0447-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="d0447-109">对于用户: 用户: Read. All, Read. All</span><span class="sxs-lookup"><span data-stu-id="d0447-109">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="d0447-110">对于组: Group. All、Group. all、Read. All</span><span class="sxs-lookup"><span data-stu-id="d0447-110">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d0447-111">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0447-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d0447-112">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d0447-112">Optional query parameters</span></span>
<span data-ttu-id="d0447-113">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d0447-113">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d0447-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0447-114">Request headers</span></span>
| <span data-ttu-id="d0447-115">名称</span><span class="sxs-lookup"><span data-stu-id="d0447-115">Name</span></span>      |<span data-ttu-id="d0447-116">说明</span><span class="sxs-lookup"><span data-stu-id="d0447-116">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d0447-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0447-117">Authorization</span></span>  | <span data-ttu-id="d0447-118">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="d0447-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="d0447-119">接受</span><span class="sxs-lookup"><span data-stu-id="d0447-119">Accept</span></span>  | <span data-ttu-id="d0447-120">application/json</span><span class="sxs-lookup"><span data-stu-id="d0447-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="d0447-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0447-121">Request body</span></span>
<span data-ttu-id="d0447-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0447-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0447-123">响应</span><span class="sxs-lookup"><span data-stu-id="d0447-123">Response</span></span>

<span data-ttu-id="d0447-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0447-124">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d0447-125">示例</span><span class="sxs-lookup"><span data-stu-id="d0447-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0447-126">请求</span><span class="sxs-lookup"><span data-stu-id="d0447-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="d0447-127">响应</span><span class="sxs-lookup"><span data-stu-id="d0447-127">Response</span></span>
<span data-ttu-id="d0447-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0447-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects/$entity",
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0447-130">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d0447-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0447-131">C#</span><span class="sxs-lookup"><span data-stu-id="d0447-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0447-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0447-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directory-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d0447-133">目标-C</span><span class="sxs-lookup"><span data-stu-id="d0447-133">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_directory-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/beta/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
