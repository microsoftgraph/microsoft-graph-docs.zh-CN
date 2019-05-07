---
title: 'servicePrincipal: List appRoleAssignments'
description: 检索 approleassignment 对象的列表。
localization_priority: Normal
ms.openlocfilehash: cad5cd853f4fa0ef85447b69af0421b1db0c2dc2
ms.sourcegitcommit: 3e5f4f515f050e16680ec44f68af40583147af9e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2019
ms.locfileid: "33639157"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="c5dfa-103">servicePrincipal: List appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="c5dfa-103">servicePrincipal: List appRoleAssignments</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c5dfa-104">检索 approleassignment 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-104">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c5dfa-105">权限</span><span class="sxs-lookup"><span data-stu-id="c5dfa-105">Permissions</span></span>
<span data-ttu-id="c5dfa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c5dfa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c5dfa-108">Permission type</span></span>      | <span data-ttu-id="c5dfa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c5dfa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c5dfa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c5dfa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c5dfa-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c5dfa-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c5dfa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c5dfa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c5dfa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-113">Not supported.</span></span>    |
|<span data-ttu-id="c5dfa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c5dfa-114">Application</span></span> | <span data-ttu-id="c5dfa-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c5dfa-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c5dfa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c5dfa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c5dfa-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c5dfa-117">Optional query parameters</span></span>
<span data-ttu-id="c5dfa-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c5dfa-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c5dfa-119">Request headers</span></span>
| <span data-ttu-id="c5dfa-120">名称</span><span class="sxs-lookup"><span data-stu-id="c5dfa-120">Name</span></span>       | <span data-ttu-id="c5dfa-121">类型</span><span class="sxs-lookup"><span data-stu-id="c5dfa-121">Type</span></span> | <span data-ttu-id="c5dfa-122">说明</span><span class="sxs-lookup"><span data-stu-id="c5dfa-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c5dfa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c5dfa-123">Authorization</span></span>  | <span data-ttu-id="c5dfa-124">string</span><span class="sxs-lookup"><span data-stu-id="c5dfa-124">string</span></span>  | <span data-ttu-id="c5dfa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c5dfa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c5dfa-127">Request body</span></span>
<span data-ttu-id="c5dfa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c5dfa-129">响应</span><span class="sxs-lookup"><span data-stu-id="c5dfa-129">Response</span></span>

<span data-ttu-id="c5dfa-130">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-130">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c5dfa-131">示例</span><span class="sxs-lookup"><span data-stu-id="c5dfa-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c5dfa-132">请求</span><span class="sxs-lookup"><span data-stu-id="c5dfa-132">Request</span></span>
<span data-ttu-id="c5dfa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="c5dfa-134">响应</span><span class="sxs-lookup"><span data-stu-id="c5dfa-134">Response</span></span>
<span data-ttu-id="c5dfa-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c5dfa-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="c5dfa-138">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="c5dfa-138">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="c5dfa-139">语言</span><span class="sxs-lookup"><span data-stu-id="c5dfa-139">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_approleassignments-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c5dfa-140">Javascript</span><span class="sxs-lookup"><span data-stu-id="c5dfa-140">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_approleassignments-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

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
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/serviceprincipal-list-approleassignments.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
