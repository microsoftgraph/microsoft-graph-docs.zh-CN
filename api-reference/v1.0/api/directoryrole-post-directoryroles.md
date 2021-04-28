---
title: Activate directoryRole
description: 激活目录角色。
localization_priority: Normal
author: abhijeetsinha
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 6295e6d60d35eb434e1e5b1d91dae3fc60eda84f
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52050519"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="03575-103">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="03575-103">Activate directoryRole</span></span>

<span data-ttu-id="03575-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03575-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="03575-p101">激活目录角色。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，只激活公司管理员和隐式的用户目录角色。若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="03575-p101">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="03575-109">权限</span><span class="sxs-lookup"><span data-stu-id="03575-109">Permissions</span></span>
<span data-ttu-id="03575-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="03575-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03575-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="03575-112">Permission type</span></span>      | <span data-ttu-id="03575-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="03575-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="03575-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03575-114">Delegated (work or school account)</span></span> | <span data-ttu-id="03575-115">RoleManagement.ReadWrite.Directory、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="03575-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="03575-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03575-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="03575-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="03575-117">Not supported.</span></span>    |
|<span data-ttu-id="03575-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="03575-118">Application</span></span> | <span data-ttu-id="03575-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="03575-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="03575-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03575-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="03575-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="03575-121">Request headers</span></span>
| <span data-ttu-id="03575-122">名称</span><span class="sxs-lookup"><span data-stu-id="03575-122">Name</span></span>       | <span data-ttu-id="03575-123">类型</span><span class="sxs-lookup"><span data-stu-id="03575-123">Type</span></span> | <span data-ttu-id="03575-124">说明</span><span class="sxs-lookup"><span data-stu-id="03575-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="03575-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="03575-125">Authorization</span></span>  | <span data-ttu-id="03575-126">string</span><span class="sxs-lookup"><span data-stu-id="03575-126">string</span></span>  | <span data-ttu-id="03575-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="03575-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="03575-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="03575-129">Content-Type</span></span>  | <span data-ttu-id="03575-130">string</span><span class="sxs-lookup"><span data-stu-id="03575-130">string</span></span>  | <span data-ttu-id="03575-131">application/json</span><span class="sxs-lookup"><span data-stu-id="03575-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="03575-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="03575-132">Request body</span></span>
<span data-ttu-id="03575-133">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03575-133">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="03575-134">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03575-134">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="03575-135">参数</span><span class="sxs-lookup"><span data-stu-id="03575-135">Parameter</span></span> | <span data-ttu-id="03575-136">类型</span><span class="sxs-lookup"><span data-stu-id="03575-136">Type</span></span> | <span data-ttu-id="03575-137">说明</span><span class="sxs-lookup"><span data-stu-id="03575-137">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="03575-138">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="03575-138">roleTemplateId</span></span> | <span data-ttu-id="03575-139">string</span><span class="sxs-lookup"><span data-stu-id="03575-139">string</span></span> | <span data-ttu-id="03575-140">必需。</span><span class="sxs-lookup"><span data-stu-id="03575-140">Required.</span></span> <span data-ttu-id="03575-141">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。</span><span class="sxs-lookup"><span data-stu-id="03575-141">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="03575-142">这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="03575-142">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="03575-143">响应</span><span class="sxs-lookup"><span data-stu-id="03575-143">Response</span></span>

<span data-ttu-id="03575-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03575-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03575-145">示例</span><span class="sxs-lookup"><span data-stu-id="03575-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="03575-146">请求</span><span class="sxs-lookup"><span data-stu-id="03575-146">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="03575-147">HTTP</span><span class="sxs-lookup"><span data-stu-id="03575-147">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="03575-148">C#</span><span class="sxs-lookup"><span data-stu-id="03575-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="03575-149">JavaScript</span><span class="sxs-lookup"><span data-stu-id="03575-149">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="03575-150">Objective-C</span><span class="sxs-lookup"><span data-stu-id="03575-150">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="03575-151">Java</span><span class="sxs-lookup"><span data-stu-id="03575-151">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-directoryrole-from-directoryroles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="03575-152">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03575-152">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="03575-153">响应</span><span class="sxs-lookup"><span data-stu-id="03575-153">Response</span></span>
<span data-ttu-id="03575-154">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="03575-154">Note: The response object shown here might be shortened for readability.</span></span>
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

