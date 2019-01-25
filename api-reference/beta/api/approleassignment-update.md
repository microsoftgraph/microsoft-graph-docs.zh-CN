---
title: 更新 approleassignment
description: 更新 approleassignment 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 54c256e3b94a5bb2d62c2ffe31ecf777d472b93c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527918"
---
# <a name="update-approleassignment"></a><span data-ttu-id="777b3-103">更新 approleassignment</span><span class="sxs-lookup"><span data-stu-id="777b3-103">Update approleassignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="777b3-104">更新 approleassignment 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="777b3-104">Update the properties of approleassignment object.</span></span>
## <a name="permissions"></a><span data-ttu-id="777b3-105">权限</span><span class="sxs-lookup"><span data-stu-id="777b3-105">Permissions</span></span>
<span data-ttu-id="777b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="777b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="777b3-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="777b3-108">Permission type</span></span>      | <span data-ttu-id="777b3-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="777b3-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="777b3-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="777b3-110">Delegated (work or school account)</span></span> | <span data-ttu-id="777b3-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="777b3-111">Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="777b3-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="777b3-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="777b3-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="777b3-113">Not supported.</span></span>    |
|<span data-ttu-id="777b3-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="777b3-114">Application</span></span> | <span data-ttu-id="777b3-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="777b3-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="777b3-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="777b3-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /users/{id | userPrincipalName}/appRoleAssignments/{id}
PATCH /servicePrincipals/{id}/appRoleAssignedTo
PATCH /groups/{id}/appRoleAssignments/{id}
```
## <a name="request-headers"></a><span data-ttu-id="777b3-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="777b3-117">Request headers</span></span>
| <span data-ttu-id="777b3-118">名称</span><span class="sxs-lookup"><span data-stu-id="777b3-118">Name</span></span>       | <span data-ttu-id="777b3-119">类型</span><span class="sxs-lookup"><span data-stu-id="777b3-119">Type</span></span> | <span data-ttu-id="777b3-120">说明</span><span class="sxs-lookup"><span data-stu-id="777b3-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="777b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="777b3-121">Authorization</span></span>  | <span data-ttu-id="777b3-122">string</span><span class="sxs-lookup"><span data-stu-id="777b3-122">string</span></span>  | <span data-ttu-id="777b3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="777b3-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="777b3-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="777b3-125">Request body</span></span>
<span data-ttu-id="777b3-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="777b3-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="777b3-129">属性</span><span class="sxs-lookup"><span data-stu-id="777b3-129">Property</span></span>     | <span data-ttu-id="777b3-130">类型</span><span class="sxs-lookup"><span data-stu-id="777b3-130">Type</span></span>   |<span data-ttu-id="777b3-131">说明</span><span class="sxs-lookup"><span data-stu-id="777b3-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="777b3-132">creationTimestamp</span><span class="sxs-lookup"><span data-stu-id="777b3-132">creationTimestamp</span></span>|<span data-ttu-id="777b3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="777b3-133">DateTimeOffset</span></span>|<span data-ttu-id="777b3-134">授予创建时间。</span><span class="sxs-lookup"><span data-stu-id="777b3-134">The time when the grant was created.</span></span>|
|<span data-ttu-id="777b3-135">id</span><span class="sxs-lookup"><span data-stu-id="777b3-135">id</span></span>|<span data-ttu-id="777b3-136">Guid</span><span class="sxs-lookup"><span data-stu-id="777b3-136">Guid</span></span>|<span data-ttu-id="777b3-137">已分配给主体角色 id。</span><span class="sxs-lookup"><span data-stu-id="777b3-137">The role id that was assigned to the principal.</span></span>  <span data-ttu-id="777b3-138">必须由其**appRoles**属性中目标资源应用程序**resourceId**声明此角色。</span><span class="sxs-lookup"><span data-stu-id="777b3-138">This role must be declared by the target resource application **resourceId** in its **appRoles** property.</span></span> <span data-ttu-id="777b3-139">如果资源没有声明任何权限，必须指定默认 id (零 GUID)。</span><span class="sxs-lookup"><span data-stu-id="777b3-139">Where the resource does not declare any permissions, a default id (zero GUID) must be specified.</span></span>                            <span data-ttu-id="777b3-140">**注意：** 不可为 null。</span><span class="sxs-lookup"><span data-stu-id="777b3-140">**Notes**: not nullable.</span></span>            |
|<span data-ttu-id="777b3-141">principalDisplayName</span><span class="sxs-lookup"><span data-stu-id="777b3-141">principalDisplayName</span></span>|<span data-ttu-id="777b3-142">String</span><span class="sxs-lookup"><span data-stu-id="777b3-142">String</span></span>|<span data-ttu-id="777b3-143">已授予访问权限的主体的显示名称。</span><span class="sxs-lookup"><span data-stu-id="777b3-143">The display name of the principal that was granted the access.</span></span>|
|<span data-ttu-id="777b3-144">principalId</span><span class="sxs-lookup"><span data-stu-id="777b3-144">principalId</span></span>|<span data-ttu-id="777b3-145">Guid</span><span class="sxs-lookup"><span data-stu-id="777b3-145">Guid</span></span>|<span data-ttu-id="777b3-146">要授予访问权限的主体的唯一标识符 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="777b3-146">The unique identifier (**objectId**) for the principal being granted the access.</span></span>                            <span data-ttu-id="777b3-147">**说明**： 必需。</span><span class="sxs-lookup"><span data-stu-id="777b3-147">**Notes**: required.</span></span>            |
|<span data-ttu-id="777b3-148">principalType</span><span class="sxs-lookup"><span data-stu-id="777b3-148">principalType</span></span>|<span data-ttu-id="777b3-149">String</span><span class="sxs-lookup"><span data-stu-id="777b3-149">String</span></span>|<span data-ttu-id="777b3-150">主体的类型。</span><span class="sxs-lookup"><span data-stu-id="777b3-150">The type of principal.</span></span>  <span data-ttu-id="777b3-151">这可以是"User"，"组"或"ServicePrincipal"。</span><span class="sxs-lookup"><span data-stu-id="777b3-151">This can either be "User", "Group" or "ServicePrincipal".</span></span>|
|<span data-ttu-id="777b3-152">resourceDisplayName</span><span class="sxs-lookup"><span data-stu-id="777b3-152">resourceDisplayName</span></span>|<span data-ttu-id="777b3-153">String</span><span class="sxs-lookup"><span data-stu-id="777b3-153">String</span></span>|<span data-ttu-id="777b3-154">对其进行分配资源的显示名称。</span><span class="sxs-lookup"><span data-stu-id="777b3-154">The display name of the resource to which the assignment was made.</span></span>|
|<span data-ttu-id="777b3-155">resourceId</span><span class="sxs-lookup"><span data-stu-id="777b3-155">resourceId</span></span>|<span data-ttu-id="777b3-156">Guid</span><span class="sxs-lookup"><span data-stu-id="777b3-156">Guid</span></span>|<span data-ttu-id="777b3-157">为其进行工作分配的目标资源 （服务主体） 的唯一标识符 (**objectId**)。</span><span class="sxs-lookup"><span data-stu-id="777b3-157">The unique identifier (**objectId**) for the target resource (service principal) for which the assignment was made.</span></span>|

## <a name="response"></a><span data-ttu-id="777b3-158">响应</span><span class="sxs-lookup"><span data-stu-id="777b3-158">Response</span></span>

<span data-ttu-id="777b3-159">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="777b3-159">If successful, this method returns a `200 OK` response code and updated [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="777b3-160">示例</span><span class="sxs-lookup"><span data-stu-id="777b3-160">Example</span></span>
##### <a name="request"></a><span data-ttu-id="777b3-161">请求</span><span class="sxs-lookup"><span data-stu-id="777b3-161">Request</span></span>
<span data-ttu-id="777b3-162">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="777b3-162">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="777b3-163">响应</span><span class="sxs-lookup"><span data-stu-id="777b3-163">Response</span></span>
<span data-ttu-id="777b3-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="777b3-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Update approleassignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/approleassignment-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
