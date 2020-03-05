---
title: 'privilegedApproval: myRequests'
description: 获取请求者的审批请求。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28d203daac2ad4027aed05add21c331dfa9d8d13
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42455415"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="f2e75-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="f2e75-103">privilegedApproval: myRequests</span></span>

<span data-ttu-id="f2e75-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f2e75-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2e75-105">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="f2e75-105">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="f2e75-106">权限</span><span class="sxs-lookup"><span data-stu-id="f2e75-106">Permissions</span></span>
<span data-ttu-id="f2e75-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2e75-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f2e75-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2e75-109">Permission type</span></span>      | <span data-ttu-id="f2e75-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2e75-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2e75-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2e75-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f2e75-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2e75-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2e75-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2e75-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2e75-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2e75-114">Not supported.</span></span>    |
|<span data-ttu-id="f2e75-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2e75-115">Application</span></span> | <span data-ttu-id="f2e75-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2e75-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2e75-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2e75-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="f2e75-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2e75-118">Request headers</span></span>
| <span data-ttu-id="f2e75-119">名称</span><span class="sxs-lookup"><span data-stu-id="f2e75-119">Name</span></span>       | <span data-ttu-id="f2e75-120">说明</span><span class="sxs-lookup"><span data-stu-id="f2e75-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="f2e75-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2e75-121">Authorization</span></span>  | <span data-ttu-id="f2e75-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2e75-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2e75-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2e75-124">Request body</span></span>

## <a name="response"></a><span data-ttu-id="f2e75-125">响应</span><span class="sxs-lookup"><span data-stu-id="f2e75-125">Response</span></span>

<span data-ttu-id="f2e75-126">如果成功，此方法在`200 OK`响应正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f2e75-126">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="f2e75-127">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="f2e75-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="f2e75-128">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="f2e75-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="f2e75-129">示例</span><span class="sxs-lookup"><span data-stu-id="f2e75-129">Example</span></span>
<span data-ttu-id="f2e75-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="f2e75-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="f2e75-131">请求</span><span class="sxs-lookup"><span data-stu-id="f2e75-131">Request</span></span>
<span data-ttu-id="f2e75-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2e75-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f2e75-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2e75-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="c"></a>[<span data-ttu-id="f2e75-134">C#</span><span class="sxs-lookup"><span data-stu-id="f2e75-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2e75-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2e75-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2e75-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2e75-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="f2e75-137">响应</span><span class="sxs-lookup"><span data-stu-id="f2e75-137">Response</span></span>
<span data-ttu-id="f2e75-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2e75-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
