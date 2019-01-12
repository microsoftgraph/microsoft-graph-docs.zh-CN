---
title: Activate directoryRole
description: 激活目录角色。 若要读取目录角色或更新其成员，它必须首先激活在租户中。 默认情况下将激活只有公司管理员和隐式用户目录角色。 若要访问和分配给另一个目录角色的成员，必须先激活它使用其相应的目录角色模板 (directoryRoleTemplate)。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 44c447515a8bc9600a708b3c4a41562bd15c4e59
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975447"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="f2452-106">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="f2452-106">Activate directoryRole</span></span>

> <span data-ttu-id="f2452-107">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f2452-107">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2452-108">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f2452-108">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f2452-109">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="f2452-109">Activate a directory role.</span></span> <span data-ttu-id="f2452-110">若要读取目录角色或更新其成员，它必须首先激活在租户中。</span><span class="sxs-lookup"><span data-stu-id="f2452-110">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="f2452-111">默认情况下将激活只有公司管理员和隐式用户目录角色。</span><span class="sxs-lookup"><span data-stu-id="f2452-111">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="f2452-112">若要访问和分配给另一个目录角色的成员，必须先激活它使用其相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md))。</span><span class="sxs-lookup"><span data-stu-id="f2452-112">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2452-113">权限</span><span class="sxs-lookup"><span data-stu-id="f2452-113">Permissions</span></span>
<span data-ttu-id="f2452-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2452-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2452-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2452-116">Permission type</span></span>      | <span data-ttu-id="f2452-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2452-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f2452-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2452-118">Delegated (work or school account)</span></span> | <span data-ttu-id="f2452-119">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f2452-119">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f2452-120">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2452-120">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f2452-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2452-121">Not supported.</span></span>    |
|<span data-ttu-id="f2452-122">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2452-122">Application</span></span> | <span data-ttu-id="f2452-123">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2452-123">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2452-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2452-124">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="f2452-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2452-125">Request headers</span></span>
| <span data-ttu-id="f2452-126">名称</span><span class="sxs-lookup"><span data-stu-id="f2452-126">Name</span></span>       | <span data-ttu-id="f2452-127">类型</span><span class="sxs-lookup"><span data-stu-id="f2452-127">Type</span></span> | <span data-ttu-id="f2452-128">说明</span><span class="sxs-lookup"><span data-stu-id="f2452-128">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="f2452-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2452-129">Authorization</span></span>  | <span data-ttu-id="f2452-130">string</span><span class="sxs-lookup"><span data-stu-id="f2452-130">string</span></span>  | <span data-ttu-id="f2452-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2452-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f2452-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2452-133">Request body</span></span>
<span data-ttu-id="f2452-134">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2452-134">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="f2452-135">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f2452-135">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="f2452-136">必需的参数</span><span class="sxs-lookup"><span data-stu-id="f2452-136">Required parameter</span></span> | <span data-ttu-id="f2452-137">类型</span><span class="sxs-lookup"><span data-stu-id="f2452-137">Type</span></span> | <span data-ttu-id="f2452-138">说明</span><span class="sxs-lookup"><span data-stu-id="f2452-138">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="f2452-139">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="f2452-139">roleTemplateId</span></span> | <span data-ttu-id="f2452-140">string</span><span class="sxs-lookup"><span data-stu-id="f2452-140">string</span></span> | <span data-ttu-id="f2452-p106">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="f2452-p106">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="f2452-143">响应</span><span class="sxs-lookup"><span data-stu-id="f2452-143">Response</span></span>

<span data-ttu-id="f2452-144">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f2452-144">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2452-145">示例</span><span class="sxs-lookup"><span data-stu-id="f2452-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="f2452-146">请求</span><span class="sxs-lookup"><span data-stu-id="f2452-146">Request</span></span>
<span data-ttu-id="f2452-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f2452-147">Here is an example of the request.</span></span>
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
<span data-ttu-id="f2452-148">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2452-148">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="f2452-149">响应</span><span class="sxs-lookup"><span data-stu-id="f2452-149">Response</span></span>
<span data-ttu-id="f2452-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f2452-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
