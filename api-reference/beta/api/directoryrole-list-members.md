---
title: 列出成员
description: 检索分配给目录角色的用户列表。只能将用户分配给目录角色。
author: lleonard-msft
ms.openlocfilehash: 8bd0f67d6ca565dac6dfae501f5bc5c829f4db3b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27359099"
---
# <a name="list-members"></a><span data-ttu-id="53099-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="53099-104">List members</span></span>

> <span data-ttu-id="53099-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="53099-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="53099-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53099-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="53099-p103">检索分配给目录角色的用户列表。只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="53099-p103">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="53099-109">权限</span><span class="sxs-lookup"><span data-stu-id="53099-109">Permissions</span></span>
<span data-ttu-id="53099-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53099-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="53099-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="53099-112">Permission type</span></span>      | <span data-ttu-id="53099-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="53099-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="53099-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53099-114">Delegated (work or school account)</span></span> | <span data-ttu-id="53099-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="53099-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="53099-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53099-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="53099-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="53099-117">Not supported.</span></span>    |
|<span data-ttu-id="53099-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="53099-118">Application</span></span> | <span data-ttu-id="53099-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53099-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="53099-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53099-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="53099-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="53099-121">Optional query parameters</span></span>
<span data-ttu-id="53099-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="53099-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="53099-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="53099-123">Request headers</span></span>
| <span data-ttu-id="53099-124">Name</span><span class="sxs-lookup"><span data-stu-id="53099-124">Name</span></span>       | <span data-ttu-id="53099-125">类型</span><span class="sxs-lookup"><span data-stu-id="53099-125">Type</span></span> | <span data-ttu-id="53099-126">说明</span><span class="sxs-lookup"><span data-stu-id="53099-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="53099-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="53099-127">Authorization</span></span>  | <span data-ttu-id="53099-128">string</span><span class="sxs-lookup"><span data-stu-id="53099-128">string</span></span>  | <span data-ttu-id="53099-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="53099-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="53099-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="53099-131">Request body</span></span>
<span data-ttu-id="53099-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="53099-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="53099-133">响应</span><span class="sxs-lookup"><span data-stu-id="53099-133">Response</span></span>

<span data-ttu-id="53099-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="53099-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="53099-135">示例</span><span class="sxs-lookup"><span data-stu-id="53099-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="53099-136">请求</span><span class="sxs-lookup"><span data-stu-id="53099-136">Request</span></span>
<span data-ttu-id="53099-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53099-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="53099-138">响应</span><span class="sxs-lookup"><span data-stu-id="53099-138">Response</span></span>
<span data-ttu-id="53099-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53099-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->