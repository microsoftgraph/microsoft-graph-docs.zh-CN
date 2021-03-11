---
title: 列出 scopedAdministratorOf
description: 检索用户的 scopedRoleMembership 列表。
author: jpettere
localization_priority: Normal
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 1de486edef0764b528491ed63bd5fd01d2e94895
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721493"
---
# <a name="list-scopedadministratorof"></a><span data-ttu-id="a079e-103">列出 scopedAdministratorOf</span><span class="sxs-lookup"><span data-stu-id="a079e-103">List scopedAdministratorOf</span></span>

<span data-ttu-id="a079e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a079e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a079e-105">检索用户的 [scopedRoleMembership](../resources/scopedrolemembership.md) 列表。</span><span class="sxs-lookup"><span data-stu-id="a079e-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) for the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="a079e-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="a079e-106">Permissions</span></span>
<span data-ttu-id="a079e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a079e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="a079e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a079e-109">Permission type</span></span>      | <span data-ttu-id="a079e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a079e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a079e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a079e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a079e-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a079e-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a079e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a079e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a079e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a079e-114">Not supported.</span></span>    |
|<span data-ttu-id="a079e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a079e-115">Application</span></span> | <span data-ttu-id="a079e-116">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a079e-116">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a079e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a079e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /me/scopedRoleMemberOf 
GET /users/{id}/scopedRoleMemberOf

```
## <a name="optional-query-parameters"></a><span data-ttu-id="a079e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a079e-118">Optional query parameters</span></span>
<span data-ttu-id="a079e-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a079e-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a079e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a079e-120">Request headers</span></span>
| <span data-ttu-id="a079e-121">标头</span><span class="sxs-lookup"><span data-stu-id="a079e-121">Header</span></span>       | <span data-ttu-id="a079e-122">值</span><span class="sxs-lookup"><span data-stu-id="a079e-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a079e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a079e-123">Authorization</span></span>  | <span data-ttu-id="a079e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a079e-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a079e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a079e-126">Request body</span></span>
<span data-ttu-id="a079e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a079e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a079e-128">响应</span><span class="sxs-lookup"><span data-stu-id="a079e-128">Response</span></span>

<span data-ttu-id="a079e-129">如果成功，此方法在响应正文中返回 `200 OK` [响应代码和 scopedRoleMembership](../resources/scopedrolemembership.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a079e-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a079e-130">示例</span><span class="sxs-lookup"><span data-stu-id="a079e-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a079e-131">请求</span><span class="sxs-lookup"><span data-stu-id="a079e-131">Request</span></span>
<span data-ttu-id="a079e-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a079e-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a079e-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="a079e-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedadministratorof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/me/scopedRoleMemberOf
```
# <a name="c"></a>[<span data-ttu-id="a079e-134">C#</span><span class="sxs-lookup"><span data-stu-id="a079e-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedadministratorof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a079e-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a079e-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedadministratorof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a079e-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a079e-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedadministratorof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a079e-137">Java</span><span class="sxs-lookup"><span data-stu-id="a079e-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedadministratorof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a079e-138">响应</span><span class="sxs-lookup"><span data-stu-id="a079e-138">Response</span></span>
<span data-ttu-id="a079e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a079e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
