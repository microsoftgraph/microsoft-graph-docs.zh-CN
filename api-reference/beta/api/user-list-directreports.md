---
title: 列出 directReports
description: 获取用户的直接下属。返回指定此用户作为经理的用户和联系人。
ms.openlocfilehash: 33903aa45fb5f7550feba72d0db48da389dd8c82
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044130"
---
# <a name="list-directreports"></a><span data-ttu-id="f5378-104">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="f5378-104">List directReports</span></span>

> <span data-ttu-id="f5378-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f5378-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f5378-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f5378-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f5378-p103">获取用户的直接下属。返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="f5378-p103">Get user's direct reports. Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="f5378-109">权限</span><span class="sxs-lookup"><span data-stu-id="f5378-109">Permissions</span></span>
<span data-ttu-id="f5378-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f5378-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f5378-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="f5378-112">Permission type</span></span>      | <span data-ttu-id="f5378-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f5378-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f5378-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f5378-114">Delegated (work or school account)</span></span> | <span data-ttu-id="f5378-115">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f5378-115">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f5378-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f5378-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f5378-117">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="f5378-117">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="f5378-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f5378-118">Application</span></span> | <span data-ttu-id="f5378-119">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f5378-119">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f5378-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f5378-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f5378-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f5378-121">Optional query parameters</span></span>
<span data-ttu-id="f5378-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f5378-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f5378-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="f5378-123">Request headers</span></span>
| <span data-ttu-id="f5378-124">标头</span><span class="sxs-lookup"><span data-stu-id="f5378-124">Header</span></span>       | <span data-ttu-id="f5378-125">值</span><span class="sxs-lookup"><span data-stu-id="f5378-125">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="f5378-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="f5378-126">Authorization</span></span>  | <span data-ttu-id="f5378-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f5378-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f5378-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f5378-129">Content-Type</span></span>   | <span data-ttu-id="f5378-130">application/json</span><span class="sxs-lookup"><span data-stu-id="f5378-130">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="f5378-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f5378-131">Request body</span></span>
<span data-ttu-id="f5378-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f5378-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f5378-133">响应</span><span class="sxs-lookup"><span data-stu-id="f5378-133">Response</span></span>

<span data-ttu-id="f5378-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f5378-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f5378-135">示例</span><span class="sxs-lookup"><span data-stu-id="f5378-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f5378-136">请求</span><span class="sxs-lookup"><span data-stu-id="f5378-136">Request</span></span>
<span data-ttu-id="f5378-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f5378-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="f5378-138">响应</span><span class="sxs-lookup"><span data-stu-id="f5378-138">Response</span></span>
<span data-ttu-id="f5378-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f5378-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->