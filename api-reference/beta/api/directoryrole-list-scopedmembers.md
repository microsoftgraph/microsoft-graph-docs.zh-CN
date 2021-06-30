---
title: 列出目录角色的 scopedMembers
description: 检索目录角色的 scopedRoleMembership 对象列表。
author: abhijeetsinha
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: d5f915debcdecba1effdf96bae6ae36da0331783
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53207697"
---
# <a name="list-scopedmembers-for-a-directory-role"></a><span data-ttu-id="2b2a7-103">列出目录角色的 scopedMembers</span><span class="sxs-lookup"><span data-stu-id="2b2a7-103">List scopedMembers for a directory role</span></span>

<span data-ttu-id="2b2a7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b2a7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2b2a7-105">检索目录角色 [的 scopedRoleMembership](../resources/scopedrolemembership.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-105">Retrieve a list of [scopedRoleMembership](../resources/scopedrolemembership.md) objects for a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="2b2a7-106">权限</span><span class="sxs-lookup"><span data-stu-id="2b2a7-106">Permissions</span></span>
<span data-ttu-id="2b2a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2b2a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2b2a7-109">Permission type</span></span>      | <span data-ttu-id="2b2a7-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2b2a7-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2b2a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2b2a7-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2b2a7-112">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="2b2a7-112">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2b2a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2b2a7-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2b2a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-114">Not supported.</span></span>    |
|<span data-ttu-id="2b2a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2b2a7-115">Application</span></span> | <span data-ttu-id="2b2a7-116">RoleManagement.Read.Directory、Directory.Read.All、RoleManagement.ReadWrite.Directory、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b2a7-116">RoleManagement.Read.Directory, Directory.Read.All, RoleManagement.ReadWrite.Directory, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2b2a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2b2a7-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryroles/{role-id}/scopedMembers
GET /directoryroles/roleTemplateId={roleTemplateId}/scopedMembers
```
## <a name="optional-query-parameters"></a><span data-ttu-id="2b2a7-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2b2a7-118">Optional query parameters</span></span>
<span data-ttu-id="2b2a7-119">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="2b2a7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2b2a7-120">Request headers</span></span>
| <span data-ttu-id="2b2a7-121">名称</span><span class="sxs-lookup"><span data-stu-id="2b2a7-121">Name</span></span>      |<span data-ttu-id="2b2a7-122">说明</span><span class="sxs-lookup"><span data-stu-id="2b2a7-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2b2a7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2b2a7-123">Authorization</span></span>  | <span data-ttu-id="2b2a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2b2a7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2b2a7-126">Request body</span></span>
<span data-ttu-id="2b2a7-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2b2a7-128">响应</span><span class="sxs-lookup"><span data-stu-id="2b2a7-128">Response</span></span>

<span data-ttu-id="2b2a7-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [scopedRoleMembership](../resources/scopedrolemembership.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-129">If successful, this method returns a `200 OK` response code and a collection of [scopedRoleMembership](../resources/scopedrolemembership.md) objects in the response body.</span></span>
## <a name="examples"></a><span data-ttu-id="2b2a7-130">示例</span><span class="sxs-lookup"><span data-stu-id="2b2a7-130">Examples</span></span>

### <a name="example-1--get-the-scoped-members-of-a-directory-role-using-role-id"></a><span data-ttu-id="2b2a7-131">示例 1：使用角色 ID 获取目录角色的作用域成员</span><span class="sxs-lookup"><span data-stu-id="2b2a7-131">Example 1:  Get the scoped members of a directory role using role id</span></span>

#### <a name="request"></a><span data-ttu-id="2b2a7-132">请求</span><span class="sxs-lookup"><span data-stu-id="2b2a7-132">Request</span></span>
<span data-ttu-id="2b2a7-133">下面是一个请求目录角色 **ID 的示例** `41d12a2f-caa8-4e3e-ba14-05e5102ce085` 。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-133">The following is an example of a request for a directory role **id** `41d12a2f-caa8-4e3e-ba14-05e5102ce085`.</span></span>

# <a name="http"></a>[<span data-ttu-id="2b2a7-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b2a7-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/41d12a2f-caa8-4e3e-ba14-05e5102ce085/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="2b2a7-135">C#</span><span class="sxs-lookup"><span data-stu-id="2b2a7-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b2a7-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b2a7-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b2a7-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b2a7-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b2a7-138">Java</span><span class="sxs-lookup"><span data-stu-id="2b2a7-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="2b2a7-139">响应</span><span class="sxs-lookup"><span data-stu-id="2b2a7-139">Response</span></span>
<span data-ttu-id="2b2a7-140">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-140">The following example shows the response.</span></span> 
><span data-ttu-id="2b2a7-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-141">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
            }
        }
    ]
}
```

### <a name="example-2--get-the-scoped-members-of-a-directory-role-using-roletemplateid"></a><span data-ttu-id="2b2a7-142">示例 2：使用 roleTemplateId 获取目录角色的作用域成员</span><span class="sxs-lookup"><span data-stu-id="2b2a7-142">Example 2:  Get the scoped members of a directory role using roleTemplateId</span></span>

#### <a name="request"></a><span data-ttu-id="2b2a7-143">请求</span><span class="sxs-lookup"><span data-stu-id="2b2a7-143">Request</span></span>
<span data-ttu-id="2b2a7-144">以下是对 **roleTemplateId** 为 的目录角色的请求示例 `fdd7a751-b60b-444a-984c-02652fe8fa1c` 。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-144">The following is an example of a request for a directory role with **roleTemplateId** `fdd7a751-b60b-444a-984c-02652fe8fa1c`.</span></span>


# <a name="http"></a>[<span data-ttu-id="2b2a7-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="2b2a7-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_scopedmembers_directoryrole_templateId"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/directoryRoles/roleTemplateId=fdd7a751-b60b-444a-984c-02652fe8fa1c/scopedMembers
```
# <a name="c"></a>[<span data-ttu-id="2b2a7-146">C#</span><span class="sxs-lookup"><span data-stu-id="2b2a7-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-scopedmembers-directoryrole-templateid-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2b2a7-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2b2a7-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-scopedmembers-directoryrole-templateid-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2b2a7-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2b2a7-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-scopedmembers-directoryrole-templateid-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2b2a7-149">Java</span><span class="sxs-lookup"><span data-stu-id="2b2a7-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-scopedmembers-directoryrole-templateid-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="2b2a7-150">响应</span><span class="sxs-lookup"><span data-stu-id="2b2a7-150">Response</span></span>
<span data-ttu-id="2b2a7-151">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-151">The following example shows the response.</span></span> 
><span data-ttu-id="2b2a7-152">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2b2a7-152">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.scopedRoleMembership",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#scopedRoleMemberships",
    "value": [
        {
            "id": "LyrRQajKPk66FAXlECzghXFuYtw3SOtAvkq8KdiKEXiTwZeOU-r8RIHrq2vQ4F1wU",
            "roleId": "41d12a2f-caa8-4e3e-ba14-05e5102ce085",
            "administrativeUnitId": "dc626e71-4837-40eb-be4a-bc29d88a1178",
            "roleMemberInfo": {
                "id": "8e97c193-ea53-44fc-81eb-ab6bd0e05d70",
                "displayName": "Adele Vance"
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
