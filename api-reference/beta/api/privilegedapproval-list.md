---
title: 列出 privilegedApproval
description: 检索 privilegedapproval 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 54b2d6bb593e8d733a883b77a735a151d71dcd98
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35978812"
---
# <a name="list-privilegedapproval"></a><span data-ttu-id="b57ad-103">列出 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="b57ad-103">List privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b57ad-104">检索 privilegedapproval 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="b57ad-104">Retrieve a list of privilegedapproval objects.</span></span>

<span data-ttu-id="b57ad-105">若要筛选查询中的结果，请在 URL 中使用标准 OData ``$filter`` 表达式。</span><span class="sxs-lookup"><span data-stu-id="b57ad-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="b57ad-106">权限</span><span class="sxs-lookup"><span data-stu-id="b57ad-106">Permissions</span></span>
<span data-ttu-id="b57ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b57ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="b57ad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b57ad-109">Permission type</span></span>      | <span data-ttu-id="b57ad-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b57ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b57ad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b57ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b57ad-112">PrivilegedAccess 的 AzureAD、Directory.accessasuser.all</span><span class="sxs-lookup"><span data-stu-id="b57ad-112">PrivilegedAccess.ReadWrite.AzureAD, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b57ad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b57ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b57ad-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b57ad-114">Not supported.</span></span>    |
|<span data-ttu-id="b57ad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b57ad-115">Application</span></span> | <span data-ttu-id="b57ad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b57ad-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b57ad-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b57ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedApproval
```
## <a name="optional-query-parameters"></a><span data-ttu-id="b57ad-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b57ad-118">Optional query parameters</span></span>
<span data-ttu-id="b57ad-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b57ad-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b57ad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b57ad-120">Request headers</span></span>
| <span data-ttu-id="b57ad-121">名称</span><span class="sxs-lookup"><span data-stu-id="b57ad-121">Name</span></span>      |<span data-ttu-id="b57ad-122">说明</span><span class="sxs-lookup"><span data-stu-id="b57ad-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="b57ad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b57ad-123">Authorization</span></span>  | <span data-ttu-id="b57ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b57ad-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b57ad-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b57ad-126">Request body</span></span>
<span data-ttu-id="b57ad-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b57ad-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b57ad-128">响应</span><span class="sxs-lookup"><span data-stu-id="b57ad-128">Response</span></span>

<span data-ttu-id="b57ad-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b57ad-129">If successful, this method returns a `200 OK` response code and collection of [privilegedApproval](../resources/privilegedapproval.md) objects in the response body.</span></span>

<span data-ttu-id="b57ad-130">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="b57ad-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="b57ad-131">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="b57ad-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="b57ad-132">示例</span><span class="sxs-lookup"><span data-stu-id="b57ad-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b57ad-133">请求</span><span class="sxs-lookup"><span data-stu-id="b57ad-133">Request</span></span>
<span data-ttu-id="b57ad-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b57ad-134">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="b57ad-135">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="b57ad-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_privilegedapproval"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedApproval
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="b57ad-136">C#</span><span class="sxs-lookup"><span data-stu-id="b57ad-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="b57ad-137">Javascript</span><span class="sxs-lookup"><span data-stu-id="b57ad-137">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="b57ad-138">目标-C</span><span class="sxs-lookup"><span data-stu-id="b57ad-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="b57ad-139">Java</span><span class="sxs-lookup"><span data-stu-id="b57ad-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="b57ad-140">响应</span><span class="sxs-lookup"><span data-stu-id="b57ad-140">Response</span></span>
<span data-ttu-id="b57ad-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b57ad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 246

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "approvalType": "approvalType-value",
      "approvalState": "approvalState-value",
      "approvalDuration": "datetime-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
