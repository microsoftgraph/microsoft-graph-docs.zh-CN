---
title: 获取已删除的项目
description: 检索已删除的项目中最近删除项目的属性。
ms.openlocfilehash: f1db1de878625ffb48357ca6ec58fddea181ef48
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041653"
---
# <a name="get-deleted-item"></a><span data-ttu-id="e8aeb-103">获取已删除的项目</span><span class="sxs-lookup"><span data-stu-id="e8aeb-103">Get deleted item</span></span>

> <span data-ttu-id="e8aeb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8aeb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8aeb-106">检索[已删除的项目](../resources/directory.md)中最近删除项目的属性。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-106">Retrieve the properties of a recently deleted item in [deleted items](../resources/directory.md).</span></span>

<span data-ttu-id="e8aeb-107">目前，已删除的项目功能仅支持用于 [group](../resources/group.md) 和 [user](../resources/user.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-107">Currently, deleted items functionality is only supported for the [group](../resources/group.md) and [user](../resources/user.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8aeb-108">权限</span><span class="sxs-lookup"><span data-stu-id="e8aeb-108">Permissions</span></span>
<span data-ttu-id="e8aeb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

* <span data-ttu-id="e8aeb-111">用户： User.Read.All，User.ReadWrite.All，Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8aeb-111">For users: User.Read.All, User.ReadWrite.All, Directory.Read.All</span></span>
* <span data-ttu-id="e8aeb-112">组： Group.Read.All，Group.ReadWrite.All，Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="e8aeb-112">For groups: Group.Read.All, Group.ReadWrite.All, Directory.Read.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e8aeb-113">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8aeb-113">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directory/deleteditems/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e8aeb-114">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e8aeb-114">Optional query parameters</span></span>
<span data-ttu-id="e8aeb-115">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-115">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="e8aeb-116">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8aeb-116">Request headers</span></span>
| <span data-ttu-id="e8aeb-117">名称</span><span class="sxs-lookup"><span data-stu-id="e8aeb-117">Name</span></span>      |<span data-ttu-id="e8aeb-118">说明</span><span class="sxs-lookup"><span data-stu-id="e8aeb-118">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="e8aeb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8aeb-119">Authorization</span></span>  | <span data-ttu-id="e8aeb-120">Bearer &lt;code&gt;。*必需*</span><span class="sxs-lookup"><span data-stu-id="e8aeb-120">Bearer &lt;code&gt; *Required*</span></span>|
| <span data-ttu-id="e8aeb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e8aeb-121">Accept</span></span>  | <span data-ttu-id="e8aeb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e8aeb-122">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="e8aeb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8aeb-123">Request body</span></span>
<span data-ttu-id="e8aeb-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8aeb-125">响应</span><span class="sxs-lookup"><span data-stu-id="e8aeb-125">Response</span></span>

<span data-ttu-id="e8aeb-126">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-126">If successful, this method returns a `200 OK` response code and [directoryObject](../resources/directoryobject.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e8aeb-127">示例</span><span class="sxs-lookup"><span data-stu-id="e8aeb-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8aeb-128">请求</span><span class="sxs-lookup"><span data-stu-id="e8aeb-128">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_directory"
}-->
```http
GET https://graph.microsoft.com/beta/directory/deleteditems/46cc6179-19d0-473e-97ad-6ff84347bbbb
```
##### <a name="response"></a><span data-ttu-id="e8aeb-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8aeb-129">Response</span></span>
<span data-ttu-id="e8aeb-p103">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8aeb-p103">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get directory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->