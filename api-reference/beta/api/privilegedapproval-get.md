---
title: 获取 privilegedApproval
description: 检索 privilegedapproval 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: dc57db4d119438f9830325b657b5eae99c930040
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957245"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="59dfc-103">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="59dfc-103">Get privilegedApproval</span></span>

<span data-ttu-id="59dfc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="59dfc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59dfc-105">检索 privilegedapproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="59dfc-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="59dfc-106">权限</span><span class="sxs-lookup"><span data-stu-id="59dfc-106">Permissions</span></span>
<span data-ttu-id="59dfc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59dfc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="59dfc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="59dfc-109">Permission type</span></span>      | <span data-ttu-id="59dfc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59dfc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59dfc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59dfc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="59dfc-112">PrivilegedAccess.ReadWrite.AzureAD、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59dfc-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="59dfc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59dfc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59dfc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="59dfc-114">Not supported.</span></span>    |
|<span data-ttu-id="59dfc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="59dfc-115">Application</span></span> | <span data-ttu-id="59dfc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="59dfc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59dfc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59dfc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="59dfc-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59dfc-118">Optional query parameters</span></span>
<span data-ttu-id="59dfc-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59dfc-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59dfc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="59dfc-120">Request headers</span></span>
| <span data-ttu-id="59dfc-121">名称</span><span class="sxs-lookup"><span data-stu-id="59dfc-121">Name</span></span>      |<span data-ttu-id="59dfc-122">说明</span><span class="sxs-lookup"><span data-stu-id="59dfc-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="59dfc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="59dfc-123">Authorization</span></span>  | <span data-ttu-id="59dfc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59dfc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59dfc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="59dfc-126">Request body</span></span>
<span data-ttu-id="59dfc-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59dfc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59dfc-128">响应</span><span class="sxs-lookup"><span data-stu-id="59dfc-128">Response</span></span>

<span data-ttu-id="59dfc-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [privilegedApproval](../resources/privilegedapproval.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="59dfc-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="59dfc-130">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="59dfc-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="59dfc-131">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="59dfc-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="59dfc-132">示例</span><span class="sxs-lookup"><span data-stu-id="59dfc-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="59dfc-133">请求</span><span class="sxs-lookup"><span data-stu-id="59dfc-133">Request</span></span>
<span data-ttu-id="59dfc-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59dfc-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="59dfc-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="59dfc-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval_1"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="59dfc-136">C#</span><span class="sxs-lookup"><span data-stu-id="59dfc-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="59dfc-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="59dfc-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="59dfc-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="59dfc-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="59dfc-139">Java</span><span class="sxs-lookup"><span data-stu-id="59dfc-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="59dfc-140">响应</span><span class="sxs-lookup"><span data-stu-id="59dfc-140">Response</span></span>
<span data-ttu-id="59dfc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59dfc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
