---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: e8dd278352ca74ea1adc16b3f7f081c70ea8387a
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33590609"
---
# <a name="get-deleted-item"></a><span data-ttu-id="119be-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="119be-103">Get deleted item</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="119be-104">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="119be-104">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="119be-105">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="119be-105">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="119be-106">权限</span><span class="sxs-lookup"><span data-stu-id="119be-106">Permissions</span></span>
<span data-ttu-id="119be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="119be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="119be-109">对于用户: 用户: Read。 All, Read。 All</span><span class="sxs-lookup"><span data-stu-id="119be-109">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="119be-110">对于组: Group。 All、Group。 all、Read。 All</span><span class="sxs-lookup"><span data-stu-id="119be-110">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="119be-111">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="119be-111">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="119be-112">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="119be-112">Optional query parameters</span></span>
<span data-ttu-id="119be-113">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="119be-113">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="119be-114">请求标头</span><span class="sxs-lookup"><span data-stu-id="119be-114">Request headers</span></span>
| <span data-ttu-id="119be-115">名称</span><span class="sxs-lookup"><span data-stu-id="119be-115">Name</span></span>      |<span data-ttu-id="119be-116">说明</span><span class="sxs-lookup"><span data-stu-id="119be-116">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="119be-117">Authorization</span><span class="sxs-lookup"><span data-stu-id="119be-117">Authorization</span></span>  | <span data-ttu-id="119be-118">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="119be-118">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="119be-119">接受</span><span class="sxs-lookup"><span data-stu-id="119be-119">Accept</span></span>  | <span data-ttu-id="119be-120">application/json</span><span class="sxs-lookup"><span data-stu-id="119be-120">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="119be-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="119be-121">Request body</span></span>
<span data-ttu-id="119be-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="119be-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="119be-123">响应</span><span class="sxs-lookup"><span data-stu-id="119be-123">Response</span></span>

<span data-ttu-id="119be-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="119be-124">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="119be-125">示例</span><span class="sxs-lookup"><span data-stu-id="119be-125">Example</span></span>
##### <a name="request"></a><span data-ttu-id="119be-126">请求</span><span class="sxs-lookup"><span data-stu-id="119be-126">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="119be-127">响应</span><span class="sxs-lookup"><span data-stu-id="119be-127">Response</span></span>
<span data-ttu-id="119be-p102">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="119be-p102">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="119be-130">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="119be-130">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="119be-131">语言</span><span class="sxs-lookup"><span data-stu-id="119be-131">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_directory-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="119be-132">Javascript</span><span class="sxs-lookup"><span data-stu-id="119be-132">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_directory-Javascript-snippets.md)]

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
    "Error: /api-reference/beta/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directory-deleteditems-get.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
