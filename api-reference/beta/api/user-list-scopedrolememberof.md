---
title: 列出 scopedAdministratorOf
description: 检索用户的 scopedRoleMembership 列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 929048213fac24186c0fd4594bf16fa21d02b04d
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721885"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="ebfec-103">列出 scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="ebfec-103">List scopedAdministratorOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ebfec-104">检索用户的[scopedRoleMembership](../resources/scopedrolemembership.md)列表。</span><span class="sxs-lookup"><span data-stu-id="ebfec-104">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="ebfec-105">权限</span><span class="sxs-lookup"><span data-stu-id="ebfec-105">Permissions</span></span>
<span data-ttu-id="ebfec-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ebfec-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ebfec-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ebfec-108">Permission type</span></span>      | <span data-ttu-id="ebfec-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ebfec-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ebfec-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ebfec-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ebfec-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ebfec-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ebfec-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ebfec-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ebfec-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ebfec-113">Not supported.</span></span>    |
|<span data-ttu-id="ebfec-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ebfec-114">Application</span></span> | <span data-ttu-id="ebfec-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebfec-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ebfec-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ebfec-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedAdministratorOf
GET /users/{id}/scopedAdministratorOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="ebfec-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ebfec-117">Optional query parameters</span></span>
<span data-ttu-id="ebfec-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ebfec-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ebfec-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ebfec-119">Request headers</span></span>
| <span data-ttu-id="ebfec-120">标头</span><span class="sxs-lookup"><span data-stu-id="ebfec-120">Header</span></span>       | <span data-ttu-id="ebfec-121">值</span><span class="sxs-lookup"><span data-stu-id="ebfec-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="ebfec-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ebfec-122">Authorization</span></span>  | <span data-ttu-id="ebfec-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ebfec-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ebfec-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ebfec-125">Request body</span></span>
<span data-ttu-id="ebfec-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ebfec-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ebfec-127">响应</span><span class="sxs-lookup"><span data-stu-id="ebfec-127">Response</span></span>

<span data-ttu-id="ebfec-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ebfec-128">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ebfec-129">示例</span><span class="sxs-lookup"><span data-stu-id="ebfec-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ebfec-130">请求</span><span class="sxs-lookup"><span data-stu-id="ebfec-130">Request</span></span>
<span data-ttu-id="ebfec-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ebfec-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ebfec-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ebfec-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedAdministratorOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ebfec-133">C#</span><span class="sxs-lookup"><span data-stu-id="ebfec-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ebfec-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ebfec-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ebfec-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="ebfec-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="ebfec-136">响应</span><span class="sxs-lookup"><span data-stu-id="ebfec-136">Response</span></span>
<span data-ttu-id="ebfec-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ebfec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 307

{
  "value": [
    {
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      },
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedAdministratorOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
