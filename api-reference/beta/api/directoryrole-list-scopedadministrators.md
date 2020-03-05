---
title: 列出目录角色的 scopedMembers
description: 检索目录角色的 scopedRoleMembership 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4d17e1531c2c2a7fd0504d7109c017d96185bedd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42434397"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="dffd2-103">列出目录角色的 scopedMembers</span><span class="sxs-lookup"><span data-stu-id="dffd2-103">List scopedMembers for a directory role</span></span>

<span data-ttu-id="dffd2-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="dffd2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dffd2-105">检索目录角色的[scopedRoleMembership](../resources/scopedrolemembership.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="dffd2-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="dffd2-106">权限</span><span class="sxs-lookup"><span data-stu-id="dffd2-106">Permissions</span></span>
<span data-ttu-id="dffd2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dffd2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dffd2-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="dffd2-109">Permission type</span></span>      | <span data-ttu-id="dffd2-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dffd2-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dffd2-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dffd2-111">Delegated (work or school account)</span></span> | <span data-ttu-id="dffd2-112">RoleManagement、RoleManagement、Directory.accessasuser.all、all、、all、all 和的所有子目录。</span><span class="sxs-lookup"><span data-stu-id="dffd2-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dffd2-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dffd2-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dffd2-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="dffd2-114">Not supported.</span></span>    |
|<span data-ttu-id="dffd2-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="dffd2-115">Application</span></span> | <span data-ttu-id="dffd2-116">RoleManagement、RoleManagement、目录和所有读写的所有子目录。所有</span><span class="sxs-lookup"><span data-stu-id="dffd2-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="dffd2-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dffd2-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{id}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="dffd2-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="dffd2-118">Optional query parameters</span></span>
<span data-ttu-id="dffd2-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="dffd2-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="dffd2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dffd2-120">Request headers</span></span>
| <span data-ttu-id="dffd2-121">名称</span><span class="sxs-lookup"><span data-stu-id="dffd2-121">Name</span></span>      |<span data-ttu-id="dffd2-122">说明</span><span class="sxs-lookup"><span data-stu-id="dffd2-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="dffd2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dffd2-123">Authorization</span></span>  | <span data-ttu-id="dffd2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dffd2-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="dffd2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dffd2-126">Request body</span></span>
<span data-ttu-id="dffd2-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="dffd2-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dffd2-128">响应</span><span class="sxs-lookup"><span data-stu-id="dffd2-128">Response</span></span>

<span data-ttu-id="dffd2-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[scopedRoleMembership](../resources/scopedrolemembership.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="dffd2-129">If successful, this method returns a `200 OK` response code and collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="dffd2-130">示例</span><span class="sxs-lookup"><span data-stu-id="dffd2-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dffd2-131">请求</span><span class="sxs-lookup"><span data-stu-id="dffd2-131">Request</span></span>
<span data-ttu-id="dffd2-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dffd2-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="dffd2-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="dffd2-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/{id}/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="dffd2-134">C#</span><span class="sxs-lookup"><span data-stu-id="dffd2-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dffd2-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dffd2-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dffd2-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dffd2-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="dffd2-137">响应</span><span class="sxs-lookup"><span data-stu-id="dffd2-137">Response</span></span>
<span data-ttu-id="dffd2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dffd2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "id": "id-value",
      "roleId": "roleId-value",
      "administrativeUnitId": "administrativeUnitId-value",
      "roleMemberInfo": {
        "id": "id-value",
        "displayName": "displayName-value",
        "userPrincipalName": "userPrincipalName-value"
      }
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List scopedmembers",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
