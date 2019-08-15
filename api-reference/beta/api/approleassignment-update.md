---
title: 更新 approleassignment
description: 更新 approleassignment 对象的属性。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 34f01f3cf8d03158df41dfd74e17fd8f767244b8
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/15/2019
ms.locfileid: "36408162"
---
# <a name="update-approleassignment"></a><span data-ttu-id="9774b-103">更新 approleassignment</span><span class="sxs-lookup"><span data-stu-id="9774b-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9774b-104">更新 approleassignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9774b-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9774b-105">权限</span><span class="sxs-lookup"><span data-stu-id="9774b-105">Permissions</span></span>
<span data-ttu-id="9774b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9774b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9774b-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="9774b-108">Permission type</span></span>      | <span data-ttu-id="9774b-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9774b-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9774b-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9774b-110">Delegated (work or school account)</span></span> | <span data-ttu-id="9774b-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9774b-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="9774b-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9774b-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9774b-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="9774b-113">Not supported.</span></span>    |
|<span data-ttu-id="9774b-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="9774b-114">Application</span></span> | <span data-ttu-id="9774b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9774b-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9774b-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9774b-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9774b-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="9774b-117">Request headers</span></span>
| <span data-ttu-id="9774b-118">名称</span><span class="sxs-lookup"><span data-stu-id="9774b-118">Name</span></span>       | <span data-ttu-id="9774b-119">类型</span><span class="sxs-lookup"><span data-stu-id="9774b-119">Type</span></span> | <span data-ttu-id="9774b-120">说明</span><span class="sxs-lookup"><span data-stu-id="9774b-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9774b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="9774b-121">Authorization</span></span>  | <span data-ttu-id="9774b-122">string</span><span class="sxs-lookup"><span data-stu-id="9774b-122">string</span></span>  | <span data-ttu-id="9774b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9774b-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9774b-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9774b-125">Request body</span></span>
<span data-ttu-id="9774b-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9774b-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9774b-129">属性</span><span class="sxs-lookup"><span data-stu-id="9774b-129">Property</span></span>     | <span data-ttu-id="9774b-130">类型</span><span class="sxs-lookup"><span data-stu-id="9774b-130">Type</span></span>   |<span data-ttu-id="9774b-131">说明</span><span class="sxs-lookup"><span data-stu-id="9774b-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9774b-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="9774b-132">creationTimestamp</span></span>|<span data-ttu-id="9774b-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9774b-133">DateTimeOffset</span></span>|<span data-ttu-id="9774b-134">创建授予的时间。</span><span class="sxs-lookup"><span data-stu-id="9774b-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="9774b-135">id</span><span class="sxs-lookup"><span data-stu-id="9774b-135">id</span></span>|<span data-ttu-id="9774b-136">Guid</span><span class="sxs-lookup"><span data-stu-id="9774b-136">Guid</span></span>|<span data-ttu-id="9774b-137">向主体分配的角色 id。</span><span class="sxs-lookup"><span data-stu-id="9774b-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="9774b-138">此角色必须由目标资源应用程序 **resourceId** 在其 **appRoles** 属性中声明。</span><span class="sxs-lookup"><span data-stu-id="9774b-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="9774b-139">如果资源未声明任何权限，则必须指定默认 id (0 GUID)。</span><span class="sxs-lookup"><span data-stu-id="9774b-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="9774b-140">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9774b-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="9774b-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="9774b-141">principalDisplayName</span></span>|<span data-ttu-id="9774b-142">String</span><span class="sxs-lookup"><span data-stu-id="9774b-142">String</span></span>|<span data-ttu-id="9774b-143">已授权访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9774b-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="9774b-144">principalId</span><span class="sxs-lookup"><span data-stu-id="9774b-144">principalId</span></span>|<span data-ttu-id="9774b-145">Guid</span><span class="sxs-lookup"><span data-stu-id="9774b-145">Guid</span></span>|<span data-ttu-id="9774b-146">要向其授予访问权限的主体的唯一标识符 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="9774b-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="9774b-147">**备注**: 必需。</span><span class="sxs-lookup"><span data-stu-id="9774b-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="9774b-148">principalType</span><span class="sxs-lookup"><span data-stu-id="9774b-148">principalType</span></span>|<span data-ttu-id="9774b-149">String</span><span class="sxs-lookup"><span data-stu-id="9774b-149">String</span></span>|<span data-ttu-id="9774b-150">主体类型。</span><span class="sxs-lookup"><span data-stu-id="9774b-150">The type of principal.</span></span>  <span data-ttu-id="9774b-151">它可以是“User”、“Group”或“ServicePrincipal”。</span><span class="sxs-lookup"><span data-stu-id="9774b-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="9774b-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9774b-152">resourceDisplayName</span></span>|<span data-ttu-id="9774b-153">String</span><span class="sxs-lookup"><span data-stu-id="9774b-153">String</span></span>|<span data-ttu-id="9774b-154">已对其进行分配的资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9774b-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="9774b-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="9774b-155">resourceId</span></span>|<span data-ttu-id="9774b-156">Guid</span><span class="sxs-lookup"><span data-stu-id="9774b-156">Guid</span></span>|<span data-ttu-id="9774b-157">为其进行了分配的目标资源 (服务主体) 的唯一标识符 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="9774b-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="9774b-158">响应</span><span class="sxs-lookup"><span data-stu-id="9774b-158">Response</span></span>

<span data-ttu-id="9774b-159">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9774b-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9774b-160">示例</span><span class="sxs-lookup"><span data-stu-id="9774b-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9774b-161">请求</span><span class="sxs-lookup"><span data-stu-id="9774b-161">Request</span></span>
<span data-ttu-id="9774b-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9774b-162">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="9774b-163">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="9774b-163">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="9774b-164">C#</span><span class="sxs-lookup"><span data-stu-id="9774b-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-approleassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="9774b-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9774b-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-approleassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="9774b-166">目标-C</span><span class="sxs-lookup"><span data-stu-id="9774b-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-approleassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="9774b-167">响应</span><span class="sxs-lookup"><span data-stu-id="9774b-167">Response</span></span>
<span data-ttu-id="9774b-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9774b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
