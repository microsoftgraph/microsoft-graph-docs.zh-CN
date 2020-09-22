---
title: Activate directoryRole
description: 激活目录角色。
localization_priority: Normal
author: abhijeetsinha
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aef27a02deee36693c921051677dbaa355c04568
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48008748"
---
# <a name="activate-directoryrole"></a><span data-ttu-id="943fe-103">Activate directoryRole</span><span class="sxs-lookup"><span data-stu-id="943fe-103">Activate directoryRole</span></span>

<span data-ttu-id="943fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="943fe-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="943fe-105">激活目录角色。</span><span class="sxs-lookup"><span data-stu-id="943fe-105">Activate a directory role.</span></span> <span data-ttu-id="943fe-106">要读取目录角色或更新其成员，首先必须在租户中将其激活。</span><span class="sxs-lookup"><span data-stu-id="943fe-106">To read a directory role or update its members, it must first be activated in the tenant.</span></span> <span data-ttu-id="943fe-107">默认情况下仅激活公司管理员和隐式用户目录角色。</span><span class="sxs-lookup"><span data-stu-id="943fe-107">Only the Company Administrators  and the implicit Users directory roles are activated by default.</span></span> <span data-ttu-id="943fe-108">若要访问成员并将分配到另一个目录角色，首先必须通过相应的目录角色模板 ([directoryRoleTemplate](../resources/directoryroletemplate.md)) 将其激活。</span><span class="sxs-lookup"><span data-stu-id="943fe-108">To access and assign members to another directory role, you must first activate it with its corresponding directory role template ([directoryRoleTemplate](../resources/directoryroletemplate.md)).</span></span>

## <a name="permissions"></a><span data-ttu-id="943fe-109">权限</span><span class="sxs-lookup"><span data-stu-id="943fe-109">Permissions</span></span>
<span data-ttu-id="943fe-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="943fe-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="943fe-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="943fe-112">Permission type</span></span>      | <span data-ttu-id="943fe-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="943fe-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="943fe-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="943fe-114">Delegated (work or school account)</span></span> | <span data-ttu-id="943fe-115">RoleManagement、Directory.accessasuser.all 和所有子目录。</span><span class="sxs-lookup"><span data-stu-id="943fe-115">RoleManagement.ReadWrite.Directory, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="943fe-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="943fe-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="943fe-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="943fe-117">Not supported.</span></span>    |
|<span data-ttu-id="943fe-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="943fe-118">Application</span></span> | <span data-ttu-id="943fe-119">RoleManagement.ReadWrite.Directory</span><span class="sxs-lookup"><span data-stu-id="943fe-119">RoleManagement.ReadWrite.Directory</span></span> |

## <a name="http-request"></a><span data-ttu-id="943fe-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="943fe-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /directoryRoles

```
## <a name="request-headers"></a><span data-ttu-id="943fe-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="943fe-121">Request headers</span></span>
| <span data-ttu-id="943fe-122">名称</span><span class="sxs-lookup"><span data-stu-id="943fe-122">Name</span></span>       | <span data-ttu-id="943fe-123">类型</span><span class="sxs-lookup"><span data-stu-id="943fe-123">Type</span></span> | <span data-ttu-id="943fe-124">说明</span><span class="sxs-lookup"><span data-stu-id="943fe-124">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="943fe-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="943fe-125">Authorization</span></span>  | <span data-ttu-id="943fe-126">string</span><span class="sxs-lookup"><span data-stu-id="943fe-126">string</span></span>  | <span data-ttu-id="943fe-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="943fe-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="943fe-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="943fe-129">Request body</span></span>
<span data-ttu-id="943fe-130">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="943fe-130">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>

<span data-ttu-id="943fe-131">下表显示激活目录角色时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="943fe-131">The following table shows the properties that are required when you activate a directory role.</span></span>

|<span data-ttu-id="943fe-132">必需的参数</span><span class="sxs-lookup"><span data-stu-id="943fe-132">Required parameter</span></span> | <span data-ttu-id="943fe-133">类型</span><span class="sxs-lookup"><span data-stu-id="943fe-133">Type</span></span> | <span data-ttu-id="943fe-134">说明</span><span class="sxs-lookup"><span data-stu-id="943fe-134">Description</span></span>|
|:---------|:---------|:---------|
|<span data-ttu-id="943fe-135">roleTemplateId</span><span class="sxs-lookup"><span data-stu-id="943fe-135">roleTemplateId</span></span> | <span data-ttu-id="943fe-136">string</span><span class="sxs-lookup"><span data-stu-id="943fe-136">string</span></span> | <span data-ttu-id="943fe-p104">角色所基于的 [directoryRoleTemplate](../resources/directoryroletemplate.md) 的 ID。这是唯一可以在请求中指定的属性。</span><span class="sxs-lookup"><span data-stu-id="943fe-p104">The ID of the [directoryRoleTemplate](../resources/directoryroletemplate.md) that the role is based on. This is the only property that may be specified in the request.</span></span>|

## <a name="response"></a><span data-ttu-id="943fe-139">响应</span><span class="sxs-lookup"><span data-stu-id="943fe-139">Response</span></span>

<span data-ttu-id="943fe-140">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [directoryRole](../resources/directoryrole.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="943fe-140">If successful, this method returns `201 Created` response code and [directoryRole](../resources/directoryrole.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="943fe-141">示例</span><span class="sxs-lookup"><span data-stu-id="943fe-141">Example</span></span>
##### <a name="request"></a><span data-ttu-id="943fe-142">请求</span><span class="sxs-lookup"><span data-stu-id="943fe-142">Request</span></span>
<span data-ttu-id="943fe-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="943fe-143">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="943fe-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="943fe-144">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="943fe-145">C#</span><span class="sxs-lookup"><span data-stu-id="943fe-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryrole-from-directoryroles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="943fe-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="943fe-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryrole-from-directoryroles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="943fe-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="943fe-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryrole-from-directoryroles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="943fe-148">在请求正文中，提供 [directoryRole](../resources/directoryrole.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="943fe-148">In the request body, supply a JSON representation of [directoryRole](../resources/directoryrole.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="943fe-149">响应</span><span class="sxs-lookup"><span data-stu-id="943fe-149">Response</span></span>
<span data-ttu-id="943fe-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="943fe-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create directoryRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


