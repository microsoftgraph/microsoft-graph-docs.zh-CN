---
title: 获取 appRoleAssignment
description: 检索 approleassignment 对象的属性和关系。
localization_priority: Priority
ms.openlocfilehash: b14a200ee2eadb3c2f68449f33ad137ff02ed474
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439481"
---
# <a name="get-approleassignment"></a><span data-ttu-id="0af3e-103">获取 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="0af3e-103">Get appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0af3e-104">检索 approleassignment 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0af3e-104">Retrieve the properties and relationships of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="0af3e-105">权限</span><span class="sxs-lookup"><span data-stu-id="0af3e-105">Permissions</span></span>
<span data-ttu-id="0af3e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0af3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af3e-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0af3e-108">Permission type</span></span>      | <span data-ttu-id="0af3e-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0af3e-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0af3e-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0af3e-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0af3e-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0af3e-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0af3e-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0af3e-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af3e-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af3e-113">Not supported.</span></span>    |
|<span data-ttu-id="0af3e-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0af3e-114">Application</span></span> | <span data-ttu-id="0af3e-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0af3e-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0af3e-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0af3e-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/appRoleAssignments/{id}
GET /servicePrincipals/{id}/appRoleAssignedTo
GET /groups/{id}/appRoleAssignments/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0af3e-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0af3e-117">Optional query parameters</span></span>
<span data-ttu-id="0af3e-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0af3e-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0af3e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0af3e-119">Request headers</span></span>
| <span data-ttu-id="0af3e-120">名称</span><span class="sxs-lookup"><span data-stu-id="0af3e-120">Name</span></span>       | <span data-ttu-id="0af3e-121">类型</span><span class="sxs-lookup"><span data-stu-id="0af3e-121">Type</span></span> | <span data-ttu-id="0af3e-122">说明</span><span class="sxs-lookup"><span data-stu-id="0af3e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0af3e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af3e-123">Authorization</span></span>  | <span data-ttu-id="0af3e-124">string</span><span class="sxs-lookup"><span data-stu-id="0af3e-124">string</span></span>  | <span data-ttu-id="0af3e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0af3e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0af3e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0af3e-127">Request body</span></span>
<span data-ttu-id="0af3e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0af3e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0af3e-129">响应</span><span class="sxs-lookup"><span data-stu-id="0af3e-129">Response</span></span>

<span data-ttu-id="0af3e-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [appRoleAssignment](../resources/approleassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0af3e-130">If successful, this method returns a `200 OK` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0af3e-131">示例</span><span class="sxs-lookup"><span data-stu-id="0af3e-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0af3e-132">请求</span><span class="sxs-lookup"><span data-stu-id="0af3e-132">Request</span></span>
<span data-ttu-id="0af3e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0af3e-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0af3e-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af3e-134">--Http</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_approleassignment"
}-->
```http
GET https://graph.microsoft.com/beta/appRoleAssignments/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="0af3e-135">C#</span><span class="sxs-lookup"><span data-stu-id="0af3e-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0af3e-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="0af3e-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0af3e-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0af3e-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0af3e-138">响应</span><span class="sxs-lookup"><span data-stu-id="0af3e-138">Response</span></span>
<span data-ttu-id="0af3e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0af3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
