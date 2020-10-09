---
title: 列出 scopedAdministratorOf
description: 检索用户的 scopedRoleMembership 列表。
author: krbain
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: cc5d67bb83102588ec1508912b36456c9f4da1c9
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48405132"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="6dbb0-103">列出 scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="6dbb0-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="6dbb0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6dbb0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6dbb0-105">检索用户的 [scopedRoleMembership](../resources/scopedrolemembership.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="6dbb0-106">权限</span><span class="sxs-lookup"><span data-stu-id="6dbb0-106">Permissions</span></span>
<span data-ttu-id="6dbb0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6dbb0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6dbb0-109">Permission type</span></span>      | <span data-ttu-id="6dbb0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6dbb0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6dbb0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6dbb0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6dbb0-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6dbb0-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6dbb0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6dbb0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6dbb0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-114">Not supported.</span></span>    |
|<span data-ttu-id="6dbb0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6dbb0-115">Application</span></span> | <span data-ttu-id="6dbb0-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6dbb0-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6dbb0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6dbb0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedRoleMemberOf 
GET /users/{id}/scopedRoleMemberOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="6dbb0-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6dbb0-118">Optional query parameters</span></span>
<span data-ttu-id="6dbb0-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6dbb0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6dbb0-120">Request headers</span></span>
| <span data-ttu-id="6dbb0-121">标头</span><span class="sxs-lookup"><span data-stu-id="6dbb0-121">Header</span></span>       | <span data-ttu-id="6dbb0-122">值</span><span class="sxs-lookup"><span data-stu-id="6dbb0-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6dbb0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6dbb0-123">Authorization</span></span>  | <span data-ttu-id="6dbb0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6dbb0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6dbb0-126">Request body</span></span>
<span data-ttu-id="6dbb0-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6dbb0-128">响应</span><span class="sxs-lookup"><span data-stu-id="6dbb0-128">Response</span></span>

<span data-ttu-id="6dbb0-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6dbb0-130">示例</span><span class="sxs-lookup"><span data-stu-id="6dbb0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6dbb0-131">请求</span><span class="sxs-lookup"><span data-stu-id="6dbb0-131">Request</span></span>
<span data-ttu-id="6dbb0-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6dbb0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6dbb0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedRoleMemberOf
```
# <a name="c"></a>[<span data-ttu-id="6dbb0-134">C#</span><span class="sxs-lookup"><span data-stu-id="6dbb0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6dbb0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6dbb0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6dbb0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6dbb0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6dbb0-137">响应</span><span class="sxs-lookup"><span data-stu-id="6dbb0-137">Response</span></span>
<span data-ttu-id="6dbb0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6dbb0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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