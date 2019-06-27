---
title: Activate directoryRole
description: 激活目录角色。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下，只激活公司管理员和隐式的用户目录角色。 若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 (directoryRoleTemplate) 将其激活。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 2ccf9f55d705d5d389d972bc9edf8866c886e0f8
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35272369"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="d0f4d-106">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="d0f4d-106">Activate directoryRole</span></span>

<span data-ttu-id="d0f4d-p102">激活目录角色。要读取目录角色或更新其成员，首先必须在租户中将其激活。默认情况下，只激活公司管理员和隐式的用户目录角色。若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p102">Activate a directory role. To read a directory role or update its members, it must first be activated in the tenant. Only the Company Administrators and the implicit Users directory roles are activated by default. To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="d0f4d-111">权限</span><span class="sxs-lookup"><span data-stu-id="d0f4d-111">Permissions</span></span>
<span data-ttu-id="d0f4d-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0f4d-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0f4d-114">Permission type</span></span>      | <span data-ttu-id="d0f4d-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d0f4d-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d0f4d-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0f4d-116">Delegated (work or school account)</span></span> | <span data-ttu-id="d0f4d-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d0f4d-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d0f4d-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0f4d-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d0f4d-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-119">Not supported.</span></span>    |
|<span data-ttu-id="d0f4d-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0f4d-120">Application</span></span> | <span data-ttu-id="d0f4d-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d0f4d-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d0f4d-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0f4d-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="d0f4d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0f4d-123">Request headers</span></span>
| <span data-ttu-id="d0f4d-124">名称</span><span class="sxs-lookup"><span data-stu-id="d0f4d-124">Name</span></span>       | <span data-ttu-id="d0f4d-125">类型</span><span class="sxs-lookup"><span data-stu-id="d0f4d-125">Type</span></span> | <span data-ttu-id="d0f4d-126">说明</span><span class="sxs-lookup"><span data-stu-id="d0f4d-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="d0f4d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0f4d-127">Authorization</span></span>  | <span data-ttu-id="d0f4d-128">string</span><span class="sxs-lookup"><span data-stu-id="d0f4d-128">string</span></span>  | <span data-ttu-id="d0f4d-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="d0f4d-131">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d0f4d-131">Content-Type</span></span>  | <span data-ttu-id="d0f4d-132">string</span><span class="sxs-lookup"><span data-stu-id="d0f4d-132">string</span></span>  | <span data-ttu-id="d0f4d-133">application/json</span><span class="sxs-lookup"><span data-stu-id="d0f4d-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="d0f4d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0f4d-134">Request body</span></span>
<span data-ttu-id="d0f4d-135">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-135">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="d0f4d-136">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-136">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="d0f4d-137">参数</span><span class="sxs-lookup"><span data-stu-id="d0f4d-137">Parameter</span></span> | <span data-ttu-id="d0f4d-138">类型</span><span class="sxs-lookup"><span data-stu-id="d0f4d-138">Type</span></span> | <span data-ttu-id="d0f4d-139">说明</span><span class="sxs-lookup"><span data-stu-id="d0f4d-139">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="d0f4d-140">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="d0f4d-140">roleTemplateId</span></span> | <span data-ttu-id="d0f4d-141">string</span><span class="sxs-lookup"><span data-stu-id="d0f4d-141">string</span></span> | <span data-ttu-id="d0f4d-142">必需。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-142">Required.</span></span> <span data-ttu-id="d0f4d-143">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-143">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on.</span></span> <span data-ttu-id="d0f4d-144">这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-144">This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="d0f4d-145">响应</span><span class="sxs-lookup"><span data-stu-id="d0f4d-145">Response</span></span>

<span data-ttu-id="d0f4d-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-146">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0f4d-147">示例</span><span class="sxs-lookup"><span data-stu-id="d0f4d-147">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d0f4d-148">请求</span><span class="sxs-lookup"><span data-stu-id="d0f4d-148">Request</span></span>

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
<span data-ttu-id="d0f4d-149">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-149">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="d0f4d-150">响应</span><span class="sxs-lookup"><span data-stu-id="d0f4d-150">Response</span></span>
<span data-ttu-id="d0f4d-p106">注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0f4d-p106">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
#### <a name="sdk-sample-code"></a><span data-ttu-id="d0f4d-153">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="d0f4d-153">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="d0f4d-154">C#</span><span class="sxs-lookup"><span data-stu-id="d0f4d-154">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d0f4d-155">Javascript</span><span class="sxs-lookup"><span data-stu-id="d0f4d-155">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="d0f4d-156">目标-C</span><span class="sxs-lookup"><span data-stu-id="d0f4d-156">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
