---
title: 'privilegedApproval: myRequests'
description: 获取请求者的审批请求。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 8c59bb1aabb6f356cc1dc468d705c968db360698
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35983389"
---
# <a name="privilegedapproval-myrequests"></a><span data-ttu-id="7557b-103">privilegedApproval: myRequests</span><span class="sxs-lookup"><span data-stu-id="7557b-103">privilegedApproval: myRequests</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7557b-104">获取请求者的审批请求。</span><span class="sxs-lookup"><span data-stu-id="7557b-104">Get the requestor's approval requests.</span></span>

## <a name="permissions"></a><span data-ttu-id="7557b-105">权限</span><span class="sxs-lookup"><span data-stu-id="7557b-105">Permissions</span></span>
<span data-ttu-id="7557b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7557b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="7557b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7557b-108">Permission type</span></span>      | <span data-ttu-id="7557b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7557b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7557b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7557b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7557b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7557b-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7557b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7557b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7557b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7557b-113">Not supported.</span></span>    |
|<span data-ttu-id="7557b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7557b-114">Application</span></span> | <span data-ttu-id="7557b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7557b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7557b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7557b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/myRequests

```
## <a name="request-headers"></a><span data-ttu-id="7557b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7557b-117">Request headers</span></span>
| <span data-ttu-id="7557b-118">名称</span><span class="sxs-lookup"><span data-stu-id="7557b-118">Name</span></span>       | <span data-ttu-id="7557b-119">说明</span><span class="sxs-lookup"><span data-stu-id="7557b-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7557b-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7557b-120">Authorization</span></span>  | <span data-ttu-id="7557b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7557b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7557b-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="7557b-123">Request body</span></span>

## <a name="response"></a><span data-ttu-id="7557b-124">响应</span><span class="sxs-lookup"><span data-stu-id="7557b-124">Response</span></span>

<span data-ttu-id="7557b-125">如果成功, 此方法在`200 OK`响应正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7557b-125">If successful, this method returns `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="7557b-126">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="7557b-126">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7557b-127">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="7557b-127">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="7557b-128">示例</span><span class="sxs-lookup"><span data-stu-id="7557b-128">Example</span></span>
<span data-ttu-id="7557b-129">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="7557b-129">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="7557b-130">请求</span><span class="sxs-lookup"><span data-stu-id="7557b-130">Request</span></span>
<span data-ttu-id="7557b-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7557b-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7557b-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7557b-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "privilegedapproval_myrequests"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval/myRequests
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7557b-133">C#</span><span class="sxs-lookup"><span data-stu-id="7557b-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/privilegedapproval-myrequests-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7557b-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="7557b-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/privilegedapproval-myrequests-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7557b-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="7557b-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/privilegedapproval-myrequests-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7557b-136">Java</span><span class="sxs-lookup"><span data-stu-id="7557b-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/privilegedapproval-myrequests-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="7557b-137">响应</span><span class="sxs-lookup"><span data-stu-id="7557b-137">Response</span></span>
<span data-ttu-id="7557b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7557b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
