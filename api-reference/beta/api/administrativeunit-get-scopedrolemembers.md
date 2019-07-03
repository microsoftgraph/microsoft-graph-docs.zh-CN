---
title: 获取 scopedRoleMember
description: 检索特定的 scopedRoleMembership 资源。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 84eea8ba422be859b36da0e278320b594fdfea79
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35439929"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="d06c1-103">获取 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="d06c1-103">Get a scopedRoleMember</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d06c1-104">检索特定的[scopedRoleMembership](../resources/scopedrolemembership.md)资源。</span><span class="sxs-lookup"><span data-stu-id="d06c1-104">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="d06c1-105">权限</span><span class="sxs-lookup"><span data-stu-id="d06c1-105">Permissions</span></span>
<span data-ttu-id="d06c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d06c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d06c1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d06c1-108">Permission type</span></span>      | <span data-ttu-id="d06c1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d06c1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d06c1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d06c1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d06c1-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d06c1-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d06c1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d06c1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d06c1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d06c1-113">Not supported.</span></span>    |
|<span data-ttu-id="d06c1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d06c1-114">Application</span></span> | <span data-ttu-id="d06c1-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d06c1-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d06c1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d06c1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d06c1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d06c1-117">Optional query parameters</span></span>
<span data-ttu-id="d06c1-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d06c1-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d06c1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d06c1-119">Request headers</span></span>
| <span data-ttu-id="d06c1-120">名称</span><span class="sxs-lookup"><span data-stu-id="d06c1-120">Name</span></span>      |<span data-ttu-id="d06c1-121">说明</span><span class="sxs-lookup"><span data-stu-id="d06c1-121">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d06c1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d06c1-122">Authorization</span></span>  | <span data-ttu-id="d06c1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d06c1-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d06c1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d06c1-125">Request body</span></span>
<span data-ttu-id="d06c1-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d06c1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d06c1-127">响应</span><span class="sxs-lookup"><span data-stu-id="d06c1-127">Response</span></span>

<span data-ttu-id="d06c1-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和请求的[scopedRoleMembership](../resources/scopedrolemembership.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d06c1-128">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d06c1-129">示例</span><span class="sxs-lookup"><span data-stu-id="d06c1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d06c1-130">请求</span><span class="sxs-lookup"><span data-stu-id="d06c1-130">Request</span></span>
<span data-ttu-id="d06c1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d06c1-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d06c1-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d06c1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```http
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d06c1-133">C#</span><span class="sxs-lookup"><span data-stu-id="d06c1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d06c1-134">Javascript</span><span class="sxs-lookup"><span data-stu-id="d06c1-134">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d06c1-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="d06c1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d06c1-136">响应</span><span class="sxs-lookup"><span data-stu-id="d06c1-136">Response</span></span>
<span data-ttu-id="d06c1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d06c1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "id": "id-value",
  "roleId": "roleId-value",
  "administrativeUnitId": "administrativeUnitId-value",
  "roleMemberInfo": {
      "id": "id-value",
      "displayName": "displayName-value",
      "userPrincipalName": "userPrincipalName-value"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedRoleMembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
