---
title: 创建 privilegedRoleAssignment
description: 使用此 API 创建新 privilegedRoleAssignment。
localization_priority: Normal
ms.openlocfilehash: 7957aa964361890572de11c375753a49a3a9e9e6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27852211"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="02060-103">创建 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="02060-103">Create privilegedRoleAssignment</span></span>

> <span data-ttu-id="02060-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="02060-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02060-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="02060-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02060-106">使用此 API 创建新[privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="02060-106">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="02060-107">权限</span><span class="sxs-lookup"><span data-stu-id="02060-107">Permissions</span></span>
<span data-ttu-id="02060-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02060-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="02060-110">请求者需要有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="02060-110">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="02060-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02060-111">Permission type</span></span>      | <span data-ttu-id="02060-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="02060-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="02060-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02060-113">Delegated (work or school account)</span></span> | <span data-ttu-id="02060-114">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="02060-114">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="02060-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02060-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="02060-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02060-116">Not supported.</span></span>    |
|<span data-ttu-id="02060-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02060-117">Application</span></span> | <span data-ttu-id="02060-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="02060-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="02060-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02060-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="02060-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02060-120">Request headers</span></span>
| <span data-ttu-id="02060-121">名称</span><span class="sxs-lookup"><span data-stu-id="02060-121">Name</span></span>       | <span data-ttu-id="02060-122">说明</span><span class="sxs-lookup"><span data-stu-id="02060-122">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="02060-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02060-123">Authorization</span></span>  | <span data-ttu-id="02060-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="02060-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="02060-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="02060-126">Request body</span></span>
<span data-ttu-id="02060-127">在请求正文中，提供[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02060-127">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="02060-128">响应</span><span class="sxs-lookup"><span data-stu-id="02060-128">Response</span></span>

<span data-ttu-id="02060-129">如果成功，此方法返回`201 Created`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="02060-129">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="02060-130">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="02060-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="02060-131">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="02060-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="02060-132">示例</span><span class="sxs-lookup"><span data-stu-id="02060-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="02060-133">请求</span><span class="sxs-lookup"><span data-stu-id="02060-133">Request</span></span>
<span data-ttu-id="02060-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02060-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_privilegedroleassignment_from_privilegedroleassignments"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoleAssignments
Content-type: application/json
Content-length: 164

{
  "userId": "userId-value",
  "roleId": "roleId-value"
}
```
<span data-ttu-id="02060-135">在请求正文中，提供[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02060-135">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="02060-136">响应</span><span class="sxs-lookup"><span data-stu-id="02060-136">Response</span></span>
<span data-ttu-id="02060-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02060-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 184

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "isElevated": true,
  "expirationDateTime": "2016-10-19T10:37:00Z",
  "resultMessage": "resultMessage-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
