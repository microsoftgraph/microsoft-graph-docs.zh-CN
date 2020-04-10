---
title: 创建 appRoleAssignment
description: 使用此 API 创建新的 appRoleAssignment。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 71148acc2c62572a2f6c7e9f711e3660d5d523ad
ms.sourcegitcommit: bdef75943ade3f1080120f555b67d5ebb3245699
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/10/2020
ms.locfileid: "43219030"
---
# <a name="create-approleassignment"></a><span data-ttu-id="49cbc-103">创建 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="49cbc-103">Create appRoleAssignment</span></span>

<span data-ttu-id="49cbc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49cbc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49cbc-105">使用此 API 创建新的 appRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="49cbc-105">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="49cbc-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="49cbc-106">Permissions</span></span>
<span data-ttu-id="49cbc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="49cbc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49cbc-109">Permission type</span></span>      | <span data-ttu-id="49cbc-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49cbc-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="49cbc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49cbc-111">Delegated (work or school account)</span></span> | <span data-ttu-id="49cbc-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="49cbc-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="49cbc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49cbc-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49cbc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49cbc-114">Not supported.</span></span>    |
|<span data-ttu-id="49cbc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49cbc-115">Application</span></span> | <span data-ttu-id="49cbc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="49cbc-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="49cbc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49cbc-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="49cbc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="49cbc-118">Request headers</span></span>
| <span data-ttu-id="49cbc-119">名称</span><span class="sxs-lookup"><span data-stu-id="49cbc-119">Name</span></span>       | <span data-ttu-id="49cbc-120">类型</span><span class="sxs-lookup"><span data-stu-id="49cbc-120">Type</span></span> | <span data-ttu-id="49cbc-121">说明</span><span class="sxs-lookup"><span data-stu-id="49cbc-121">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="49cbc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="49cbc-122">Authorization</span></span>  | <span data-ttu-id="49cbc-123">string</span><span class="sxs-lookup"><span data-stu-id="49cbc-123">string</span></span>  | <span data-ttu-id="49cbc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="49cbc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="49cbc-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="49cbc-126">Request body</span></span>
<span data-ttu-id="49cbc-127">在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49cbc-127">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="49cbc-128">响应</span><span class="sxs-lookup"><span data-stu-id="49cbc-128">Response</span></span>

<span data-ttu-id="49cbc-129">如果成功，此方法在`201 Created`响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="49cbc-129">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="49cbc-130">示例</span><span class="sxs-lookup"><span data-stu-id="49cbc-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="49cbc-131">请求</span><span class="sxs-lookup"><span data-stu-id="49cbc-131">Request</span></span>
<span data-ttu-id="49cbc-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="49cbc-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="49cbc-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="49cbc-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
# <a name="c"></a>[<span data-ttu-id="49cbc-134">C#</span><span class="sxs-lookup"><span data-stu-id="49cbc-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-approleassignment-from-serviceprincipal-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="49cbc-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="49cbc-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-approleassignment-from-serviceprincipal-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="49cbc-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="49cbc-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-approleassignment-from-serviceprincipal-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="49cbc-137">在请求正文中，提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49cbc-137">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="49cbc-138">响应</span><span class="sxs-lookup"><span data-stu-id="49cbc-138">Response</span></span>
<span data-ttu-id="49cbc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="49cbc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
