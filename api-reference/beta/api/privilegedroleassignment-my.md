---
title: privilegedRoleAssignment： my
description: 获取请求者的特权角色分配。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: fdcde1ab1b3bd5f901c2d4e05cc23ce7f6ef9023
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035034"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="524fb-103">privilegedRoleAssignment： my</span><span class="sxs-lookup"><span data-stu-id="524fb-103">privilegedRoleAssignment: my</span></span>

<span data-ttu-id="524fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="524fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="524fb-105">获取请求者的特权角色分配。</span><span class="sxs-lookup"><span data-stu-id="524fb-105">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="524fb-106">权限</span><span class="sxs-lookup"><span data-stu-id="524fb-106">Permissions</span></span>
<span data-ttu-id="524fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="524fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="524fb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="524fb-109">Permission type</span></span>      | <span data-ttu-id="524fb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="524fb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="524fb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="524fb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="524fb-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="524fb-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="524fb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="524fb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="524fb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="524fb-114">Not supported.</span></span>    |
|<span data-ttu-id="524fb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="524fb-115">Application</span></span> | <span data-ttu-id="524fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="524fb-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="524fb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="524fb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="524fb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="524fb-118">Request headers</span></span>
| <span data-ttu-id="524fb-119">名称</span><span class="sxs-lookup"><span data-stu-id="524fb-119">Name</span></span>       | <span data-ttu-id="524fb-120">说明</span><span class="sxs-lookup"><span data-stu-id="524fb-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="524fb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="524fb-121">Authorization</span></span>  | <span data-ttu-id="524fb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="524fb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="524fb-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="524fb-124">Request body</span></span>
<span data-ttu-id="524fb-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="524fb-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="524fb-126">响应</span><span class="sxs-lookup"><span data-stu-id="524fb-126">Response</span></span>

<span data-ttu-id="524fb-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [privilegedRoleAssignment](../resources/privilegedroleassignment.md) 集合对象。</span><span class="sxs-lookup"><span data-stu-id="524fb-127">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="524fb-128">示例</span><span class="sxs-lookup"><span data-stu-id="524fb-128">Example</span></span>
<span data-ttu-id="524fb-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="524fb-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="524fb-130">请求</span><span class="sxs-lookup"><span data-stu-id="524fb-130">Request</span></span>
<span data-ttu-id="524fb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="524fb-131">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="524fb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="524fb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```
# <a name="c"></a>[<span data-ttu-id="524fb-133">C#</span><span class="sxs-lookup"><span data-stu-id="524fb-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedroleassignment-my-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="524fb-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="524fb-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedroleassignment-my-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="524fb-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="524fb-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedroleassignment-my-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="524fb-136">响应</span><span class="sxs-lookup"><span data-stu-id="524fb-136">Response</span></span>
<span data-ttu-id="524fb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="524fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


