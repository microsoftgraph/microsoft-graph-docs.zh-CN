---
title: Activate directoryRole
description: 激活目录角色。 要读取目录角色或更新其成员，首先必须在租户中将其激活。 默认情况下仅激活公司管理员和隐式用户目录角色。 若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 (directoryRoleTemplate) 将其激活。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 53b61830da0803dcda8374d4b18adfbbbb7affd2
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655920"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="07f30-106">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="07f30-106">Activate directoryRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="07f30-107">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="07f30-107">Activate a directory role.</span></span> <span data-ttu-id="07f30-108">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="07f30-108">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="07f30-109">默认情况下仅激活公司管理员和隐式用户目录角色。</span><span class="sxs-lookup"><span data-stu-id="07f30-109">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="07f30-110">若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="07f30-110">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="07f30-111">权限</span><span class="sxs-lookup"><span data-stu-id="07f30-111">Permissions</span></span>
<span data-ttu-id="07f30-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07f30-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07f30-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="07f30-114">Permission type</span></span>      | <span data-ttu-id="07f30-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07f30-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="07f30-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07f30-116">Delegated (work or school account)</span></span> | <span data-ttu-id="07f30-117">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="07f30-117">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="07f30-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07f30-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="07f30-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="07f30-119">Not supported.</span></span>    |
|<span data-ttu-id="07f30-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="07f30-120">Application</span></span> | <span data-ttu-id="07f30-121">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07f30-121">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="07f30-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07f30-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="07f30-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="07f30-123">Request headers</span></span>
| <span data-ttu-id="07f30-124">名称</span><span class="sxs-lookup"><span data-stu-id="07f30-124">Name</span></span>       | <span data-ttu-id="07f30-125">类型</span><span class="sxs-lookup"><span data-stu-id="07f30-125">Type</span></span> | <span data-ttu-id="07f30-126">说明</span><span class="sxs-lookup"><span data-stu-id="07f30-126">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07f30-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="07f30-127">Authorization</span></span>  | <span data-ttu-id="07f30-128">string</span><span class="sxs-lookup"><span data-stu-id="07f30-128">string</span></span>  | <span data-ttu-id="07f30-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="07f30-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="07f30-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="07f30-131">Request body</span></span>
<span data-ttu-id="07f30-132">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07f30-132">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="07f30-133">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07f30-133">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="07f30-134">必需的参数</span><span class="sxs-lookup"><span data-stu-id="07f30-134">Required parameter</span></span> | <span data-ttu-id="07f30-135">类型</span><span class="sxs-lookup"><span data-stu-id="07f30-135">Type</span></span> | <span data-ttu-id="07f30-136">说明</span><span class="sxs-lookup"><span data-stu-id="07f30-136">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="07f30-137">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="07f30-137">roleTemplateId</span></span> | <span data-ttu-id="07f30-138">string</span><span class="sxs-lookup"><span data-stu-id="07f30-138">string</span></span> | <span data-ttu-id="07f30-p105">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="07f30-p105">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="07f30-141">响应</span><span class="sxs-lookup"><span data-stu-id="07f30-141">Response</span></span>

<span data-ttu-id="07f30-142">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07f30-142">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07f30-143">示例</span><span class="sxs-lookup"><span data-stu-id="07f30-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="07f30-144">请求</span><span class="sxs-lookup"><span data-stu-id="07f30-144">Request</span></span>
<span data-ttu-id="07f30-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07f30-145">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_directoryrole_from_directoryroles"
}-->
```http
POST https://graph.microsoft.com/beta/directoryRoles
Content-type: application/json
Content-length: 153

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value"
}
```
<span data-ttu-id="07f30-146">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07f30-146">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="07f30-147">响应</span><span class="sxs-lookup"><span data-stu-id="07f30-147">Response</span></span>
<span data-ttu-id="07f30-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07f30-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 175

{
  "description": "description-value",
  "displayName": "displayName-value",
  "roleTemplateId": "roleTemplateId-value",
  "id": "id-value"
}
```
#### <a name="sdk-sample-code"></a><span data-ttu-id="07f30-151">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="07f30-151">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="07f30-152">C#</span><span class="sxs-lookup"><span data-stu-id="07f30-152">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="07f30-153">Javascript</span><span class="sxs-lookup"><span data-stu-id="07f30-153">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/create_directoryrole_from_directoryroles-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/directoryrole-post-directoryroles.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
