---
title: 'servicePrincipal: List appRoleAssignments'
description: 检索 approleassignment 对象的列表。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: a722d2578885367e3a8708d38f4267e739d599ca
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35991385"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="7a641-103">servicePrincipal: List appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="7a641-103">servicePrincipal: List appRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7a641-104">检索 approleassignment 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7a641-104">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="7a641-105">权限</span><span class="sxs-lookup"><span data-stu-id="7a641-105">Permissions</span></span>
<span data-ttu-id="7a641-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7a641-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7a641-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7a641-108">Permission type</span></span>      | <span data-ttu-id="7a641-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7a641-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7a641-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7a641-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7a641-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7a641-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7a641-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7a641-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7a641-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7a641-113">Not supported.</span></span>    |
|<span data-ttu-id="7a641-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7a641-114">Application</span></span> | <span data-ttu-id="7a641-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7a641-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7a641-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7a641-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7a641-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7a641-117">Optional query parameters</span></span>
<span data-ttu-id="7a641-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7a641-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7a641-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="7a641-119">Request headers</span></span>
| <span data-ttu-id="7a641-120">名称</span><span class="sxs-lookup"><span data-stu-id="7a641-120">Name</span></span>       | <span data-ttu-id="7a641-121">类型</span><span class="sxs-lookup"><span data-stu-id="7a641-121">Type</span></span> | <span data-ttu-id="7a641-122">说明</span><span class="sxs-lookup"><span data-stu-id="7a641-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7a641-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7a641-123">Authorization</span></span>  | <span data-ttu-id="7a641-124">string</span><span class="sxs-lookup"><span data-stu-id="7a641-124">string</span></span>  | <span data-ttu-id="7a641-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7a641-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7a641-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7a641-127">Request body</span></span>
<span data-ttu-id="7a641-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7a641-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7a641-129">响应</span><span class="sxs-lookup"><span data-stu-id="7a641-129">Response</span></span>

<span data-ttu-id="7a641-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="7a641-130">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="7a641-131">示例</span><span class="sxs-lookup"><span data-stu-id="7a641-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7a641-132">请求</span><span class="sxs-lookup"><span data-stu-id="7a641-132">Request</span></span>
<span data-ttu-id="7a641-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7a641-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="7a641-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="7a641-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="7a641-135">C#</span><span class="sxs-lookup"><span data-stu-id="7a641-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignments-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="7a641-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="7a641-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignments-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="7a641-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="7a641-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignments-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="7a641-138">Java</span><span class="sxs-lookup"><span data-stu-id="7a641-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-approleassignments-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="7a641-139">响应</span><span class="sxs-lookup"><span data-stu-id="7a641-139">Response</span></span>
<span data-ttu-id="7a641-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7a641-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
