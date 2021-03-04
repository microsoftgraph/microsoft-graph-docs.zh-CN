---
title: 获取 privilegedApproval
description: 检索 privilegedapproval 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 0408d01fa214ec37261814e58fb2f9312e4248b2
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442262"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="395ff-103">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="395ff-103">Get privilegedApproval</span></span>

<span data-ttu-id="395ff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="395ff-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="395ff-105">检索 privilegedapproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="395ff-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="395ff-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="395ff-106">Permissions</span></span>
<span data-ttu-id="395ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="395ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="395ff-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="395ff-109">Permission type</span></span>      | <span data-ttu-id="395ff-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="395ff-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="395ff-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="395ff-111">Delegated (work or school account)</span></span> | <span data-ttu-id="395ff-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="395ff-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="395ff-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="395ff-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="395ff-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="395ff-114">Not supported.</span></span>    |
|<span data-ttu-id="395ff-115">Application</span><span class="sxs-lookup"><span data-stu-id="395ff-115">Application</span></span> | <span data-ttu-id="395ff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="395ff-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="395ff-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="395ff-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="395ff-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="395ff-118">Optional query parameters</span></span>
<span data-ttu-id="395ff-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="395ff-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="395ff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="395ff-120">Request headers</span></span>
| <span data-ttu-id="395ff-121">名称</span><span class="sxs-lookup"><span data-stu-id="395ff-121">Name</span></span>      |<span data-ttu-id="395ff-122">说明</span><span class="sxs-lookup"><span data-stu-id="395ff-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="395ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="395ff-123">Authorization</span></span>  | <span data-ttu-id="395ff-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="395ff-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="395ff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="395ff-126">Request body</span></span>
<span data-ttu-id="395ff-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="395ff-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="395ff-128">响应</span><span class="sxs-lookup"><span data-stu-id="395ff-128">Response</span></span>

<span data-ttu-id="395ff-129">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [privilegedApproval](../resources/privilegedapproval.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="395ff-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="395ff-130">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="395ff-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="395ff-131">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="395ff-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="395ff-132">示例</span><span class="sxs-lookup"><span data-stu-id="395ff-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="395ff-133">请求</span><span class="sxs-lookup"><span data-stu-id="395ff-133">Request</span></span>
<span data-ttu-id="395ff-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="395ff-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="395ff-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="395ff-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="395ff-136">C#</span><span class="sxs-lookup"><span data-stu-id="395ff-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="395ff-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="395ff-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="395ff-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="395ff-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="395ff-139">Java</span><span class="sxs-lookup"><span data-stu-id="395ff-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="395ff-140">响应</span><span class="sxs-lookup"><span data-stu-id="395ff-140">Response</span></span>
<span data-ttu-id="395ff-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="395ff-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 193

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
