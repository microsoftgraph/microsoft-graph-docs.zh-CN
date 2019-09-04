---
title: 'privilegedRoleAssignment: my'
description: 获取请求者的特权角色分配。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 948d0919e296824c32919bed50407579f2978bed
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36725582"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="a7f0d-103">privilegedRoleAssignment: my</span><span class="sxs-lookup"><span data-stu-id="a7f0d-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7f0d-104">获取请求者的特权角色分配。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7f0d-105">权限</span><span class="sxs-lookup"><span data-stu-id="a7f0d-105">Permissions</span></span>
<span data-ttu-id="a7f0d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7f0d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7f0d-108">Permission type</span></span>      | <span data-ttu-id="a7f0d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7f0d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7f0d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7f0d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="a7f0d-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a7f0d-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a7f0d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7f0d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a7f0d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-113">Not supported.</span></span>    |
|<span data-ttu-id="a7f0d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7f0d-114">Application</span></span> | <span data-ttu-id="a7f0d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="a7f0d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7f0d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="a7f0d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7f0d-117">Request headers</span></span>
| <span data-ttu-id="a7f0d-118">名称</span><span class="sxs-lookup"><span data-stu-id="a7f0d-118">Name</span></span>       | <span data-ttu-id="a7f0d-119">说明</span><span class="sxs-lookup"><span data-stu-id="a7f0d-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a7f0d-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7f0d-120">Authorization</span></span>  | <span data-ttu-id="a7f0d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a7f0d-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7f0d-123">Request body</span></span>
<span data-ttu-id="a7f0d-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7f0d-125">响应</span><span class="sxs-lookup"><span data-stu-id="a7f0d-125">Response</span></span>

<span data-ttu-id="a7f0d-126">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)集合对象。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7f0d-127">示例</span><span class="sxs-lookup"><span data-stu-id="a7f0d-127">Example</span></span>
<span data-ttu-id="a7f0d-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="a7f0d-129">请求</span><span class="sxs-lookup"><span data-stu-id="a7f0d-129">Request</span></span>
<span data-ttu-id="a7f0d-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-130">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a7f0d-131">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a7f0d-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="a7f0d-132">C#</span><span class="sxs-lookup"><span data-stu-id="a7f0d-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a7f0d-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7f0d-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a7f0d-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="a7f0d-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a7f0d-135">响应</span><span class="sxs-lookup"><span data-stu-id="a7f0d-135">Response</span></span>
<span data-ttu-id="a7f0d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a7f0d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
