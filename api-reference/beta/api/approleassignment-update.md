---
title: 更新 approleassignment
description: 更新 approleassignment 对象的属性。
ms.openlocfilehash: 3c861afde396d9cab2f745c15c7de1d9a81c5dcc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042042"
---
# <a name="update-approleassignment"></a><span data-ttu-id="9d868-103">更新 approleassignment</span><span class="sxs-lookup"><span data-stu-id="9d868-103">Update approleassignment</span></span>

> <span data-ttu-id="9d868-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9d868-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9d868-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9d868-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="9d868-106">更新 approleassignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9d868-106">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="9d868-107">权限</span><span class="sxs-lookup"><span data-stu-id="9d868-107">Permissions</span></span>
<span data-ttu-id="9d868-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9d868-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9d868-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9d868-110">Permission type</span></span>      | <span data-ttu-id="9d868-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9d868-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="9d868-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9d868-112">Delegated (work or school account)</span></span> | <span data-ttu-id="9d868-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="9d868-113">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="9d868-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9d868-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="9d868-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d868-115">Not supported.</span></span>    |
|<span data-ttu-id="9d868-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9d868-116">Application</span></span> | <span data-ttu-id="9d868-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="9d868-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="9d868-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9d868-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="9d868-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9d868-119">Request headers</span></span>
| <span data-ttu-id="9d868-120">名称</span><span class="sxs-lookup"><span data-stu-id="9d868-120">Name</span></span>       | <span data-ttu-id="9d868-121">类型</span><span class="sxs-lookup"><span data-stu-id="9d868-121">Type</span></span> | <span data-ttu-id="9d868-122">说明</span><span class="sxs-lookup"><span data-stu-id="9d868-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="9d868-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9d868-123">Authorization</span></span>  | <span data-ttu-id="9d868-124">string</span><span class="sxs-lookup"><span data-stu-id="9d868-124">string</span></span>  | <span data-ttu-id="9d868-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9d868-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="9d868-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9d868-127">Request body</span></span>
<span data-ttu-id="9d868-p104">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="9d868-p104">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="9d868-131">属性</span><span class="sxs-lookup"><span data-stu-id="9d868-131">Property</span></span>     | <span data-ttu-id="9d868-132">类型</span><span class="sxs-lookup"><span data-stu-id="9d868-132">Type</span></span>   |<span data-ttu-id="9d868-133">说明</span><span class="sxs-lookup"><span data-stu-id="9d868-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9d868-134">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="9d868-134">creationTimestamp</span></span>|<span data-ttu-id="9d868-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9d868-135">DateTimeOffset</span></span>|<span data-ttu-id="9d868-136">授予创建时间。</span><span class="sxs-lookup"><span data-stu-id="9d868-136">The time when the grant was created.</span></span>|
|<span data-ttu-id="9d868-137">id</span><span class="sxs-lookup"><span data-stu-id="9d868-137">id</span></span>|<span data-ttu-id="9d868-138">Guid</span><span class="sxs-lookup"><span data-stu-id="9d868-138">Guid</span></span>|<span data-ttu-id="9d868-139">已分配给主体角色 id。</span><span class="sxs-lookup"><span data-stu-id="9d868-139">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="9d868-140">必须由其**appRoles**属性中目标资源应用程序**resourceId**声明此角色。</span><span class="sxs-lookup"><span data-stu-id="9d868-140">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="9d868-141">如果资源没有声明任何权限，必须指定默认 id (零 GUID)。</span><span class="sxs-lookup"><span data-stu-id="9d868-141">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="9d868-142">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="9d868-142">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="9d868-143">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d868-143">principalDisplayName</span></span>|<span data-ttu-id="9d868-144">字符串</span><span class="sxs-lookup"><span data-stu-id="9d868-144">String</span></span>|<span data-ttu-id="9d868-145">已授予访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d868-145">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="9d868-146">principalId</span><span class="sxs-lookup"><span data-stu-id="9d868-146">principalId</span></span>|<span data-ttu-id="9d868-147">Guid</span><span class="sxs-lookup"><span data-stu-id="9d868-147">Guid</span></span>|<span data-ttu-id="9d868-148">要授予访问权限的主体的唯一标识符 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="9d868-148">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="9d868-149">**说明**： 必需。</span><span class="sxs-lookup"><span data-stu-id="9d868-149">**Notes**: required.</span></span>            |
|<span data-ttu-id="9d868-150">principalType</span><span class="sxs-lookup"><span data-stu-id="9d868-150">principalType</span></span>|<span data-ttu-id="9d868-151">字符串</span><span class="sxs-lookup"><span data-stu-id="9d868-151">String</span></span>|<span data-ttu-id="9d868-152">主体的类型。</span><span class="sxs-lookup"><span data-stu-id="9d868-152">The type of principal.</span></span>  <span data-ttu-id="9d868-153">这可以是"User"，"组"或"ServicePrincipal"。</span><span class="sxs-lookup"><span data-stu-id="9d868-153">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="9d868-154">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="9d868-154">resourceDisplayName</span></span>|<span data-ttu-id="9d868-155">字符串</span><span class="sxs-lookup"><span data-stu-id="9d868-155">String</span></span>|<span data-ttu-id="9d868-156">对其进行分配资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9d868-156">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="9d868-157">resourceId</span><span class="sxs-lookup"><span data-stu-id="9d868-157">resourceId</span></span>|<span data-ttu-id="9d868-158">Guid</span><span class="sxs-lookup"><span data-stu-id="9d868-158">Guid</span></span>|<span data-ttu-id="9d868-159">为其进行工作分配的目标资源 （服务主体） 的唯一标识符 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="9d868-159">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="9d868-160">响应</span><span class="sxs-lookup"><span data-stu-id="9d868-160">Response</span></span>

<span data-ttu-id="9d868-161">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9d868-161">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="9d868-162">示例</span><span class="sxs-lookup"><span data-stu-id="9d868-162">Example</span></span>
##### <a name="request"></a><span data-ttu-id="9d868-163">请求</span><span class="sxs-lookup"><span data-stu-id="9d868-163">Request</span></span>
<span data-ttu-id="9d868-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9d868-164">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="9d868-165">响应</span><span class="sxs-lookup"><span data-stu-id="9d868-165">Response</span></span>
<span data-ttu-id="9d868-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9d868-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment"
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
<!-- {
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->