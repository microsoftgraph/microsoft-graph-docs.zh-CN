---
title: 更新 approleassignment
description: 更新 approleassignment 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4f1f499cb54ac135f5393e795e24cea6c7962685
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441359"
---
# <a name="update-approleassignment"></a><span data-ttu-id="17691-103">更新 approleassignment</span><span class="sxs-lookup"><span data-stu-id="17691-103">Update approleassignment</span></span>

<span data-ttu-id="17691-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="17691-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17691-105">更新 approleassignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="17691-105">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="17691-106">权限</span><span class="sxs-lookup"><span data-stu-id="17691-106">Permissions</span></span>
<span data-ttu-id="17691-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17691-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17691-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="17691-109">Permission type</span></span>      | <span data-ttu-id="17691-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17691-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17691-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17691-111">Delegated (work or school account)</span></span> | <span data-ttu-id="17691-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17691-112">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="17691-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17691-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17691-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="17691-114">Not supported.</span></span>    |
|<span data-ttu-id="17691-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="17691-115">Application</span></span> | <span data-ttu-id="17691-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="17691-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="17691-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17691-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="17691-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="17691-118">Request headers</span></span>
| <span data-ttu-id="17691-119">名称</span><span class="sxs-lookup"><span data-stu-id="17691-119">Name</span></span>       | <span data-ttu-id="17691-120">类型</span><span class="sxs-lookup"><span data-stu-id="17691-120">Type</span></span> | <span data-ttu-id="17691-121">说明</span><span class="sxs-lookup"><span data-stu-id="17691-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="17691-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="17691-122">Authorization</span></span>  | <span data-ttu-id="17691-123">string</span><span class="sxs-lookup"><span data-stu-id="17691-123">string</span></span>  | <span data-ttu-id="17691-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17691-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17691-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="17691-126">Request body</span></span>
<span data-ttu-id="17691-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="17691-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="17691-130">属性</span><span class="sxs-lookup"><span data-stu-id="17691-130">Property</span></span>     | <span data-ttu-id="17691-131">类型</span><span class="sxs-lookup"><span data-stu-id="17691-131">Type</span></span>   |<span data-ttu-id="17691-132">说明</span><span class="sxs-lookup"><span data-stu-id="17691-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="17691-133">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="17691-133">creationTimestamp</span></span>|<span data-ttu-id="17691-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="17691-134">DateTimeOffset</span></span>|<span data-ttu-id="17691-135">创建授予的时间。</span><span class="sxs-lookup"><span data-stu-id="17691-135">The time when the grant was created.</span></span>|
|<span data-ttu-id="17691-136">id</span><span class="sxs-lookup"><span data-stu-id="17691-136">id</span></span>|<span data-ttu-id="17691-137">Guid</span><span class="sxs-lookup"><span data-stu-id="17691-137">Guid</span></span>|<span data-ttu-id="17691-138">向主体分配的角色 id。</span><span class="sxs-lookup"><span data-stu-id="17691-138">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="17691-139">此角色必须由目标资源应用程序 **resourceId** 在其 **appRoles** 属性中声明。</span><span class="sxs-lookup"><span data-stu-id="17691-139">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="17691-140">如果资源未声明任何权限，则必须指定默认 id (0 GUID)。</span><span class="sxs-lookup"><span data-stu-id="17691-140">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="17691-141">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="17691-141">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="17691-142">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="17691-142">principalDisplayName</span></span>|<span data-ttu-id="17691-143">String</span><span class="sxs-lookup"><span data-stu-id="17691-143">String</span></span>|<span data-ttu-id="17691-144">已授权访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="17691-144">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="17691-145">principalId</span><span class="sxs-lookup"><span data-stu-id="17691-145">principalId</span></span>|<span data-ttu-id="17691-146">Guid</span><span class="sxs-lookup"><span data-stu-id="17691-146">Guid</span></span>|<span data-ttu-id="17691-147">要向其授予访问权限的主体的唯一标识符（**objectId**）。</span><span class="sxs-lookup"><span data-stu-id="17691-147">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="17691-148">**备注**：必需。</span><span class="sxs-lookup"><span data-stu-id="17691-148">**Notes**: required.</span></span>            |
|<span data-ttu-id="17691-149">principalType</span><span class="sxs-lookup"><span data-stu-id="17691-149">principalType</span></span>|<span data-ttu-id="17691-150">String</span><span class="sxs-lookup"><span data-stu-id="17691-150">String</span></span>|<span data-ttu-id="17691-151">主体类型。</span><span class="sxs-lookup"><span data-stu-id="17691-151">The type of principal.</span></span>  <span data-ttu-id="17691-152">它可以是“User”、“Group”或“ServicePrincipal”。</span><span class="sxs-lookup"><span data-stu-id="17691-152">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="17691-153">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="17691-153">resourceDisplayName</span></span>|<span data-ttu-id="17691-154">String</span><span class="sxs-lookup"><span data-stu-id="17691-154">String</span></span>|<span data-ttu-id="17691-155">已对其进行分配的资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="17691-155">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="17691-156">resourceId</span><span class="sxs-lookup"><span data-stu-id="17691-156">resourceId</span></span>|<span data-ttu-id="17691-157">Guid</span><span class="sxs-lookup"><span data-stu-id="17691-157">Guid</span></span>|<span data-ttu-id="17691-158">为其进行了分配的目标资源（服务主体）的唯一标识符（**objectId**）。</span><span class="sxs-lookup"><span data-stu-id="17691-158">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="17691-159">响应</span><span class="sxs-lookup"><span data-stu-id="17691-159">Response</span></span>

<span data-ttu-id="17691-160">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="17691-160">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17691-161">示例</span><span class="sxs-lookup"><span data-stu-id="17691-161">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17691-162">请求</span><span class="sxs-lookup"><span data-stu-id="17691-162">Request</span></span>
<span data-ttu-id="17691-163">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17691-163">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="17691-164">HTTP</span><span class="sxs-lookup"><span data-stu-id="17691-164">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_approleassignment"
}-->
```http
PATCH https://graph.microsoft.com/beta/appRoleAssignments/{id}
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
# <a name="c"></a>[<span data-ttu-id="17691-165">C#</span><span class="sxs-lookup"><span data-stu-id="17691-165">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="17691-166">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17691-166">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="17691-167">Objective-C</span><span class="sxs-lookup"><span data-stu-id="17691-167">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="17691-168">响应</span><span class="sxs-lookup"><span data-stu-id="17691-168">Response</span></span>
<span data-ttu-id="17691-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17691-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
