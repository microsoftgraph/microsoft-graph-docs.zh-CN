---
title: Activate directoryRole
description: 激活目录角色。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，只激活公司管理员和隐式的用户目录角色。若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 (directoryRoleTemplate) 将其激活。
localization_priority: Normal
ms.openlocfilehash: 9e3e962de4e25422cbf35f9efa8a83499cfe81bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885146"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="adb53-106">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="adb53-106">Activate directoryRole</span></span>

<span data-ttu-id="adb53-p102">激活目录角色。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，只激活公司管理员和隐式的用户目录角色。若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="adb53-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="adb53-111">权限</span><span class="sxs-lookup"><span data-stu-id="adb53-111">Permissions</span></span>
<span data-ttu-id="adb53-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="adb53-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adb53-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="adb53-114">Permission type</span></span>      | <span data-ttu-id="adb53-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="adb53-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="adb53-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="adb53-116">Delegated (work or school account)</span></span> | <span data-ttu-id="adb53-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="adb53-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="adb53-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="adb53-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="adb53-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="adb53-119">Not supported.</span></span>    |
|<span data-ttu-id="adb53-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="adb53-120">Application</span></span> | <span data-ttu-id="adb53-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="adb53-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="adb53-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="adb53-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="adb53-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="adb53-123">Request headers</span></span>
| <span data-ttu-id="adb53-124">名称</span><span class="sxs-lookup"><span data-stu-id="adb53-124">Name</span></span>       | <span data-ttu-id="adb53-125">类型</span><span class="sxs-lookup"><span data-stu-id="adb53-125">Type</span></span> | <span data-ttu-id="adb53-126">说明</span><span class="sxs-lookup"><span data-stu-id="adb53-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="adb53-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="adb53-127">Authorization</span></span>  | <span data-ttu-id="adb53-128">string</span><span class="sxs-lookup"><span data-stu-id="adb53-128">string</span></span>  | <span data-ttu-id="adb53-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="adb53-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="adb53-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="adb53-131">Content-Type</span></span>  | <span data-ttu-id="adb53-132">string</span><span class="sxs-lookup"><span data-stu-id="adb53-132">string</span></span>  | <span data-ttu-id="adb53-133">application/json</span><span class="sxs-lookup"><span data-stu-id="adb53-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="adb53-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="adb53-134">Request body</span></span>
<span data-ttu-id="adb53-135">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adb53-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="adb53-136">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="adb53-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="adb53-137">参数</span><span class="sxs-lookup"><span data-stu-id="adb53-137">Parameter</span></span> | <span data-ttu-id="adb53-138">类型</span><span class="sxs-lookup"><span data-stu-id="adb53-138">Type</span></span> | <span data-ttu-id="adb53-139">说明</span><span class="sxs-lookup"><span data-stu-id="adb53-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="adb53-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="adb53-140">roleTemplateId</span></span> | <span data-ttu-id="adb53-141">string</span><span class="sxs-lookup"><span data-stu-id="adb53-141">string</span></span> | <span data-ttu-id="adb53-142">必需。</span><span class="sxs-lookup"><span data-stu-id="adb53-142">Required.</span></span> <span data-ttu-id="adb53-143">基于角色的[directoryRoleTemplate](../resources/directoryroletemplate.md)的 ID。</span><span class="sxs-lookup"><span data-stu-id="adb53-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="adb53-144">这是唯一可以请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="adb53-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="adb53-145">响应</span><span class="sxs-lookup"><span data-stu-id="adb53-145">Response</span></span>

<span data-ttu-id="adb53-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="adb53-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adb53-147">示例</span><span class="sxs-lookup"><span data-stu-id="adb53-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="adb53-148">请求</span><span class="sxs-lookup"><span data-stu-id="adb53-148">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/v1.0/directoryRoles
Content-type: application/json

{
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="adb53-149">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="adb53-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="adb53-150">响应</span><span class="sxs-lookup"><span data-stu-id="adb53-150">Response</span></span>
<span data-ttu-id="adb53-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="adb53-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
