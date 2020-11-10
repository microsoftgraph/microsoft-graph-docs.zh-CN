---
title: 'privilegedApproval: myRequests'
description: 获取请求者的审批请求。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: 595528ef40da9193fadeb53d742bd6ab6aa6008b
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48970485"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="9ac2f-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="9ac2f-103">privilegedApproval: myRequests</span></span>

<span data-ttu-id="9ac2f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ac2f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9ac2f-105">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-105">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="9ac2f-106">权限</span><span class="sxs-lookup"><span data-stu-id="9ac2f-106">Permissions</span></span>
<span data-ttu-id="9ac2f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="9ac2f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ac2f-109">Permission type</span></span>      | <span data-ttu-id="9ac2f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9ac2f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9ac2f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ac2f-111">Delegated (work or school account)</span></span> | <span data-ttu-id="9ac2f-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9ac2f-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="9ac2f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ac2f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9ac2f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-114">Not supported.</span></span>    |
|<span data-ttu-id="9ac2f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ac2f-115">Application</span></span> | <span data-ttu-id="9ac2f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9ac2f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ac2f-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="9ac2f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ac2f-118">Request headers</span></span>
| <span data-ttu-id="9ac2f-119">名称</span><span class="sxs-lookup"><span data-stu-id="9ac2f-119">Name</span></span>       | <span data-ttu-id="9ac2f-120">说明</span><span class="sxs-lookup"><span data-stu-id="9ac2f-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="9ac2f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ac2f-121">Authorization</span></span>  | <span data-ttu-id="9ac2f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9ac2f-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ac2f-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="9ac2f-125">响应</span><span class="sxs-lookup"><span data-stu-id="9ac2f-125">Response</span></span>

<span data-ttu-id="9ac2f-126">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [privilegedApproval](../resources/privilegedapproval.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-126">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="9ac2f-127">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="9ac2f-128">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="9ac2f-129">示例</span><span class="sxs-lookup"><span data-stu-id="9ac2f-129">Example</span></span>
<span data-ttu-id="9ac2f-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="9ac2f-131">请求</span><span class="sxs-lookup"><span data-stu-id="9ac2f-131">Request</span></span>
<span data-ttu-id="9ac2f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="9ac2f-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac2f-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="c"></a>[<span data-ttu-id="9ac2f-134">C#</span><span class="sxs-lookup"><span data-stu-id="9ac2f-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9ac2f-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9ac2f-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9ac2f-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9ac2f-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9ac2f-137">Java</span><span class="sxs-lookup"><span data-stu-id="9ac2f-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedapproval-myrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="9ac2f-138">响应</span><span class="sxs-lookup"><span data-stu-id="9ac2f-138">Response</span></span>
<span data-ttu-id="9ac2f-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ac2f-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


