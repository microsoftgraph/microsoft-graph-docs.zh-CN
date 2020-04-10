---
title: 获取 privilegedApproval
description: 检索 privilegedapproval 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: shauliu
ms.openlocfilehash: dbf8611e94e07b4f0a5bea1024a59779f72c53dc
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43218813"
---
# <a name="get-privilegedapproval"></a><span data-ttu-id="0a4b7-103">获取 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="0a4b7-103">Get privilegedApproval</span></span>

<span data-ttu-id="0a4b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0a4b7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0a4b7-105">检索 privilegedapproval 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-105">Retrieve the properties and relationships of privilegedapproval object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0a4b7-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0a4b7-106">Permissions</span></span>
<span data-ttu-id="0a4b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="0a4b7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0a4b7-109">Permission type</span></span>      | <span data-ttu-id="0a4b7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0a4b7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0a4b7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0a4b7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0a4b7-112">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="0a4b7-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="0a4b7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0a4b7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0a4b7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-114">Not supported.</span></span>    |
|<span data-ttu-id="0a4b7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0a4b7-115">Application</span></span> | <span data-ttu-id="0a4b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="0a4b7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0a4b7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0a4b7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0a4b7-118">Optional query parameters</span></span>
<span data-ttu-id="0a4b7-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0a4b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0a4b7-120">Request headers</span></span>
| <span data-ttu-id="0a4b7-121">名称</span><span class="sxs-lookup"><span data-stu-id="0a4b7-121">Name</span></span>      |<span data-ttu-id="0a4b7-122">说明</span><span class="sxs-lookup"><span data-stu-id="0a4b7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0a4b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a4b7-123">Authorization</span></span>  | <span data-ttu-id="0a4b7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0a4b7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0a4b7-126">Request body</span></span>
<span data-ttu-id="0a4b7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a4b7-128">响应</span><span class="sxs-lookup"><span data-stu-id="0a4b7-128">Response</span></span>

<span data-ttu-id="0a4b7-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-129">If successful, this method returns a `200 OK` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="0a4b7-130">请注意，需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="0a4b7-131">否则，将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="0a4b7-132">示例</span><span class="sxs-lookup"><span data-stu-id="0a4b7-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0a4b7-133">请求</span><span class="sxs-lookup"><span data-stu-id="0a4b7-133">Request</span></span>
<span data-ttu-id="0a4b7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-134">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0a4b7-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="0a4b7-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/privilegedApproval/{id}
```
# <a name="c"></a>[<span data-ttu-id="0a4b7-136">C#</span><span class="sxs-lookup"><span data-stu-id="0a4b7-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0a4b7-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0a4b7-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0a4b7-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0a4b7-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0a4b7-139">响应</span><span class="sxs-lookup"><span data-stu-id="0a4b7-139">Response</span></span>
<span data-ttu-id="0a4b7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0a4b7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
