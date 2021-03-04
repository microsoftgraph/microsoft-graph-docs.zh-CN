---
title: privilegedApproval：myRequests
description: 获取请求者的审批请求。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 5c552e49826c28368657af6dd574811288986cb5
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442248"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="dcc04-103">privilegedApproval：myRequests</span><span class="sxs-lookup"><span data-stu-id="dcc04-103">privilegedApproval: myRequests</span></span>

<span data-ttu-id="dcc04-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dcc04-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dcc04-105">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="dcc04-105">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="dcc04-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="dcc04-106">Permissions</span></span>
<span data-ttu-id="dcc04-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dcc04-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="dcc04-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dcc04-109">Permission type</span></span>      | <span data-ttu-id="dcc04-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dcc04-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dcc04-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dcc04-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dcc04-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="dcc04-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dcc04-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dcc04-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dcc04-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcc04-114">Not supported.</span></span>    |
|<span data-ttu-id="dcc04-115">Application</span><span class="sxs-lookup"><span data-stu-id="dcc04-115">Application</span></span> | <span data-ttu-id="dcc04-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dcc04-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="dcc04-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dcc04-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="dcc04-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="dcc04-118">Request headers</span></span>
| <span data-ttu-id="dcc04-119">名称</span><span class="sxs-lookup"><span data-stu-id="dcc04-119">Name</span></span>       | <span data-ttu-id="dcc04-120">说明</span><span class="sxs-lookup"><span data-stu-id="dcc04-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="dcc04-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dcc04-121">Authorization</span></span>  | <span data-ttu-id="dcc04-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dcc04-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dcc04-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="dcc04-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="dcc04-125">响应</span><span class="sxs-lookup"><span data-stu-id="dcc04-125">Response</span></span>

<span data-ttu-id="dcc04-126">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和 [privilegedApproval](../resources/privilegedapproval.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dcc04-126">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="dcc04-127">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="dcc04-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="dcc04-128">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="dcc04-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="dcc04-129">示例</span><span class="sxs-lookup"><span data-stu-id="dcc04-129">Example</span></span>
<span data-ttu-id="dcc04-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="dcc04-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="dcc04-131">请求</span><span class="sxs-lookup"><span data-stu-id="dcc04-131">Request</span></span>
<span data-ttu-id="dcc04-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dcc04-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dcc04-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dcc04-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="c"></a>[<span data-ttu-id="dcc04-134">C#</span><span class="sxs-lookup"><span data-stu-id="dcc04-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dcc04-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dcc04-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dcc04-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dcc04-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dcc04-137">Java</span><span class="sxs-lookup"><span data-stu-id="dcc04-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedapproval-myrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="dcc04-138">响应</span><span class="sxs-lookup"><span data-stu-id="dcc04-138">Response</span></span>
<span data-ttu-id="dcc04-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dcc04-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "privilegedApproval: myRequests",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


