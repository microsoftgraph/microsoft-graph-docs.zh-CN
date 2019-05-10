---
title: 列出 memberOf
description: '返回用户是其直接成员的组和目录角色。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 89f6ee1ee2b9f28267b130f7038a6cdbae7846d2
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33601654"
---
# <a name="list-memberof"></a><span data-ttu-id="f10b3-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="f10b3-103">List memberOf</span></span>

<span data-ttu-id="f10b3-104">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="f10b3-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="f10b3-105">权限</span><span class="sxs-lookup"><span data-stu-id="f10b3-105">Permissions</span></span>
<span data-ttu-id="f10b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f10b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f10b3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="f10b3-108">Permission type</span></span>      | <span data-ttu-id="f10b3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f10b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f10b3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f10b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="f10b3-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f10b3-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f10b3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f10b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f10b3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="f10b3-113">Not supported.</span></span>    |
|<span data-ttu-id="f10b3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="f10b3-114">Application</span></span> | <span data-ttu-id="f10b3-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f10b3-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f10b3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f10b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/memberOf
or
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f10b3-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f10b3-117">Optional query parameters</span></span>
<span data-ttu-id="f10b3-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="f10b3-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span> <span data-ttu-id="f10b3-119">$filter 不受支持。</span><span class="sxs-lookup"><span data-stu-id="f10b3-119">$filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="f10b3-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f10b3-120">Request headers</span></span>
| <span data-ttu-id="f10b3-121">标头</span><span class="sxs-lookup"><span data-stu-id="f10b3-121">Header</span></span>       | <span data-ttu-id="f10b3-122">值</span><span class="sxs-lookup"><span data-stu-id="f10b3-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="f10b3-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f10b3-123">Authorization</span></span>  | <span data-ttu-id="f10b3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f10b3-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f10b3-126">接受</span><span class="sxs-lookup"><span data-stu-id="f10b3-126">Accept</span></span>  | <span data-ttu-id="f10b3-127">application/json</span><span class="sxs-lookup"><span data-stu-id="f10b3-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f10b3-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="f10b3-128">Request body</span></span>
<span data-ttu-id="f10b3-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f10b3-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f10b3-130">响应</span><span class="sxs-lookup"><span data-stu-id="f10b3-130">Response</span></span>

<span data-ttu-id="f10b3-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="f10b3-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="f10b3-132">示例</span><span class="sxs-lookup"><span data-stu-id="f10b3-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f10b3-133">请求</span><span class="sxs-lookup"><span data-stu-id="f10b3-133">Request</span></span>
<span data-ttu-id="f10b3-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f10b3-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="f10b3-135">响应</span><span class="sxs-lookup"><span data-stu-id="f10b3-135">Response</span></span>
<span data-ttu-id="f10b3-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f10b3-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="f10b3-139">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="f10b3-139">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="f10b3-140">C#</span><span class="sxs-lookup"><span data-stu-id="f10b3-140">c</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_memberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="f10b3-141">Javascript</span><span class="sxs-lookup"><span data-stu-id="f10b3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_memberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/user-list-memberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
