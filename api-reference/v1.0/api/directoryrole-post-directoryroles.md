---
title: Activate directoryRole
description: 激活目录角色。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下，只激活公司管理员和隐式的用户目录角色。 若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 (directoryRoleTemplate) 将其激活。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ada6d1aba533ad8eeabbd4cbf64046f130711ff4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517928"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="dfea8-106">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="dfea8-106">Activate directoryRole</span></span>

<span data-ttu-id="dfea8-107">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dfea8-107">Namespace: microsoft.graph</span></span>

<span data-ttu-id="dfea8-p102">激活目录角色。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，只激活公司管理员和隐式的用户目录角色。若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="dfea8-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="dfea8-112">权限</span><span class="sxs-lookup"><span data-stu-id="dfea8-112">Permissions</span></span>
<span data-ttu-id="dfea8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dfea8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dfea8-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="dfea8-115">Permission type</span></span>      | <span data-ttu-id="dfea8-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="dfea8-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="dfea8-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dfea8-117">Delegated (work or school account)</span></span> | <span data-ttu-id="dfea8-118">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="dfea8-118">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="dfea8-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dfea8-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="dfea8-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="dfea8-120">Not supported.</span></span>    |
|<span data-ttu-id="dfea8-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="dfea8-121">Application</span></span> | <span data-ttu-id="dfea8-122">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="dfea8-122">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="dfea8-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dfea8-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="dfea8-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="dfea8-124">Request headers</span></span>
| <span data-ttu-id="dfea8-125">名称</span><span class="sxs-lookup"><span data-stu-id="dfea8-125">Name</span></span>       | <span data-ttu-id="dfea8-126">类型</span><span class="sxs-lookup"><span data-stu-id="dfea8-126">Type</span></span> | <span data-ttu-id="dfea8-127">说明</span><span class="sxs-lookup"><span data-stu-id="dfea8-127">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="dfea8-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="dfea8-128">Authorization</span></span>  | <span data-ttu-id="dfea8-129">string</span><span class="sxs-lookup"><span data-stu-id="dfea8-129">string</span></span>  | <span data-ttu-id="dfea8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="dfea8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="dfea8-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="dfea8-132">Content-Type</span></span>  | <span data-ttu-id="dfea8-133">string</span><span class="sxs-lookup"><span data-stu-id="dfea8-133">string</span></span>  | <span data-ttu-id="dfea8-134">application/json</span><span class="sxs-lookup"><span data-stu-id="dfea8-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="dfea8-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="dfea8-135">Request body</span></span>
<span data-ttu-id="dfea8-136">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfea8-136">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="dfea8-137">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dfea8-137">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="dfea8-138">参数</span><span class="sxs-lookup"><span data-stu-id="dfea8-138">Parameter</span></span> | <span data-ttu-id="dfea8-139">类型</span><span class="sxs-lookup"><span data-stu-id="dfea8-139">Type</span></span> | <span data-ttu-id="dfea8-140">说明</span><span class="sxs-lookup"><span data-stu-id="dfea8-140">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="dfea8-141">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="dfea8-141">roleTemplateId</span></span> | <span data-ttu-id="dfea8-142">string</span><span class="sxs-lookup"><span data-stu-id="dfea8-142">string</span></span> | <span data-ttu-id="dfea8-143">必需。</span><span class="sxs-lookup"><span data-stu-id="dfea8-143">Required.</span></span> <span data-ttu-id="dfea8-144">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。</span><span class="sxs-lookup"><span data-stu-id="dfea8-144">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="dfea8-145">这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="dfea8-145">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="dfea8-146">响应</span><span class="sxs-lookup"><span data-stu-id="dfea8-146">Response</span></span>

<span data-ttu-id="dfea8-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dfea8-147">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dfea8-148">示例</span><span class="sxs-lookup"><span data-stu-id="dfea8-148">Example</span></span>
##### <a name="request"></a><span data-ttu-id="dfea8-149">请求</span><span class="sxs-lookup"><span data-stu-id="dfea8-149">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="dfea8-150">HTTP</span><span class="sxs-lookup"><span data-stu-id="dfea8-150">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="dfea8-151">C#</span><span class="sxs-lookup"><span data-stu-id="dfea8-151">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="dfea8-152">JavaScript</span><span class="sxs-lookup"><span data-stu-id="dfea8-152">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="dfea8-153">Objective-C</span><span class="sxs-lookup"><span data-stu-id="dfea8-153">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="dfea8-154">Java</span><span class="sxs-lookup"><span data-stu-id="dfea8-154">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="dfea8-155">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dfea8-155">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="dfea8-156">响应</span><span class="sxs-lookup"><span data-stu-id="dfea8-156">Response</span></span>
<span data-ttu-id="dfea8-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dfea8-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": "",
  "suppressions": [
  ]
}-->
