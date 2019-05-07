---
title: List registeredDevices
description: 获取用户的注册设备列表。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 5ee2fa5f1e33fabae9b22391f6b962a133a5a47b
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33637183"
---
# <a name="list-registereddevices"></a><span data-ttu-id="e557e-103">List registeredDevices</span><span class="sxs-lookup"><span data-stu-id="e557e-103">List registeredDevices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e557e-104">获取用户的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="e557e-104">Get the list of user's registered devices.</span></span>
## <a name="permissions"></a><span data-ttu-id="e557e-105">权限</span><span class="sxs-lookup"><span data-stu-id="e557e-105">Permissions</span></span>
<span data-ttu-id="e557e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e557e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e557e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e557e-108">Permission type</span></span>      | <span data-ttu-id="e557e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e557e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e557e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e557e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e557e-111">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e557e-111">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e557e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e557e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e557e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e557e-113">Not supported.</span></span>    |
|<span data-ttu-id="e557e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e557e-114">Application</span></span> | <span data-ttu-id="e557e-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e557e-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e557e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e557e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/registeredDevices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e557e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e557e-117">Optional query parameters</span></span>
<span data-ttu-id="e557e-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e557e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e557e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e557e-119">Request headers</span></span>
| <span data-ttu-id="e557e-120">标头</span><span class="sxs-lookup"><span data-stu-id="e557e-120">Header</span></span>       | <span data-ttu-id="e557e-121">值</span><span class="sxs-lookup"><span data-stu-id="e557e-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e557e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e557e-122">Authorization</span></span>  | <span data-ttu-id="e557e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e557e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e557e-125">接受</span><span class="sxs-lookup"><span data-stu-id="e557e-125">Accept</span></span>  | <span data-ttu-id="e557e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e557e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e557e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e557e-127">Request body</span></span>
<span data-ttu-id="e557e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e557e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e557e-129">响应</span><span class="sxs-lookup"><span data-stu-id="e557e-129">Response</span></span>

<span data-ttu-id="e557e-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e557e-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e557e-131">示例</span><span class="sxs-lookup"><span data-stu-id="e557e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e557e-132">请求</span><span class="sxs-lookup"><span data-stu-id="e557e-132">Request</span></span>
<span data-ttu-id="e557e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e557e-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registereddevices"
}-->
```http
GET https://graph.microsoft.com/beta/me/registeredDevices
```
##### <a name="response"></a><span data-ttu-id="e557e-134">响应</span><span class="sxs-lookup"><span data-stu-id="e557e-134">Response</span></span>
<span data-ttu-id="e557e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e557e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="e557e-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="e557e-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="e557e-139">语言</span><span class="sxs-lookup"><span data-stu-id="e557e-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_registereddevices-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="e557e-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="e557e-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_registereddevices-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List registeredDevices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-registereddevices.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/user-list-registereddevices.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
