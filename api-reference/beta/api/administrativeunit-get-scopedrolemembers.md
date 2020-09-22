---
title: 获取 scopedRoleMember
description: 检索特定的 scopedRoleMembership 资源。
author: anandyadavMSFT
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 93c6825c0b02bad092007d4314e1fd20bd0f972f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991737"
---
# <a name="get-a-scopedrolemember"></a><span data-ttu-id="6ad5a-103">获取 scopedRoleMember</span><span class="sxs-lookup"><span data-stu-id="6ad5a-103">Get a scopedRoleMember</span></span>

<span data-ttu-id="6ad5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ad5a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ad5a-105">检索特定的 [scopedRoleMembership](../resources/scopedrolemembership.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-105">Retrieve a specific [scopedRoleMembership](../resources/scopedrolemembership.md) resource.</span></span>
## <a name="permissions"></a><span data-ttu-id="6ad5a-106">权限</span><span class="sxs-lookup"><span data-stu-id="6ad5a-106">Permissions</span></span>
<span data-ttu-id="6ad5a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6ad5a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ad5a-109">Permission type</span></span>      | <span data-ttu-id="6ad5a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ad5a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ad5a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ad5a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ad5a-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ad5a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ad5a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ad5a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-114">Not supported.</span></span>    |
|<span data-ttu-id="6ad5a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ad5a-115">Application</span></span> | <span data-ttu-id="6ad5a-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="6ad5a-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6ad5a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ad5a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /administrativeUnits/{id}/scopedRoleMembers/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6ad5a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6ad5a-118">Optional query parameters</span></span>
<span data-ttu-id="6ad5a-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6ad5a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ad5a-120">Request headers</span></span>
| <span data-ttu-id="6ad5a-121">名称</span><span class="sxs-lookup"><span data-stu-id="6ad5a-121">Name</span></span>      |<span data-ttu-id="6ad5a-122">说明</span><span class="sxs-lookup"><span data-stu-id="6ad5a-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6ad5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ad5a-123">Authorization</span></span>  | <span data-ttu-id="6ad5a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6ad5a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ad5a-126">Request body</span></span>
<span data-ttu-id="6ad5a-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6ad5a-128">响应</span><span class="sxs-lookup"><span data-stu-id="6ad5a-128">Response</span></span>

<span data-ttu-id="6ad5a-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和请求的 [scopedRoleMembership](../resources/scopedrolemembership.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-129">If successful, this method returns a `200 OK` response code and the requested [scopedRoleMembership](../resources/scopedrolemembership.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6ad5a-130">示例</span><span class="sxs-lookup"><span data-stu-id="6ad5a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6ad5a-131">请求</span><span class="sxs-lookup"><span data-stu-id="6ad5a-131">Request</span></span>
<span data-ttu-id="6ad5a-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ad5a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ad5a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedrolemember"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/administrativeUnits/{id}/scopedRoleMembers/{id}
```
# <a name="c"></a>[<span data-ttu-id="6ad5a-134">C#</span><span class="sxs-lookup"><span data-stu-id="6ad5a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedrolemember-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6ad5a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ad5a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedrolemember-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ad5a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ad5a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedrolemember-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="6ad5a-137">响应</span><span class="sxs-lookup"><span data-stu-id="6ad5a-137">Response</span></span>
<span data-ttu-id="6ad5a-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6ad5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


