---
title: 创建 privilegedRoleAssignment
description: 使用此 API 创建新的 privilegedRoleAssignment。
localization_priority: Normal
ms.openlocfilehash: 5522956b129eae8a19fd00b0e70b41380dbdd25e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32538591"
---
# <a name="create-privilegedroleassignment"></a><span data-ttu-id="e1322-103">创建 privilegedRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="e1322-103">Create privilegedRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e1322-104">使用此 API 创建新的[privilegedRoleAssignment](../resources/privilegedroleassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="e1322-104">Use this API to create a new  [privilegedRoleAssignment](../resources/privilegedroleassignment.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="e1322-105">权限</span><span class="sxs-lookup"><span data-stu-id="e1322-105">Permissions</span></span>
<span data-ttu-id="e1322-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e1322-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e1322-108">请求者需要具有_特权角色管理员_角色。</span><span class="sxs-lookup"><span data-stu-id="e1322-108">The requestor needs to have _Privileged Role Administrator_ role.</span></span> 

|<span data-ttu-id="e1322-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e1322-109">Permission type</span></span>      | <span data-ttu-id="e1322-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e1322-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e1322-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e1322-111">Delegated (work or school account)</span></span> | <span data-ttu-id="e1322-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e1322-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e1322-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e1322-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e1322-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1322-114">Not supported.</span></span>    |
|<span data-ttu-id="e1322-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e1322-115">Application</span></span> | <span data-ttu-id="e1322-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e1322-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="e1322-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e1322-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoleAssignments
```
## <a name="request-headers"></a><span data-ttu-id="e1322-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e1322-118">Request headers</span></span>
| <span data-ttu-id="e1322-119">名称</span><span class="sxs-lookup"><span data-stu-id="e1322-119">Name</span></span>       | <span data-ttu-id="e1322-120">说明</span><span class="sxs-lookup"><span data-stu-id="e1322-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="e1322-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e1322-121">Authorization</span></span>  | <span data-ttu-id="e1322-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e1322-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="e1322-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e1322-124">Request body</span></span>
<span data-ttu-id="e1322-125">在请求正文中, 提供[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1322-125">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="e1322-126">响应</span><span class="sxs-lookup"><span data-stu-id="e1322-126">Response</span></span>

<span data-ttu-id="e1322-127">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e1322-127">If successful, this method returns `201 Created` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="e1322-128">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="e1322-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="e1322-129">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="e1322-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="e1322-130">示例</span><span class="sxs-lookup"><span data-stu-id="e1322-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e1322-131">请求</span><span class="sxs-lookup"><span data-stu-id="e1322-131">Request</span></span>
<span data-ttu-id="e1322-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e1322-132">Here is an example of the request.</span></span>
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
<span data-ttu-id="e1322-133">在请求正文中, 提供[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e1322-133">In the request body, supply a JSON representation of [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="e1322-134">响应</span><span class="sxs-lookup"><span data-stu-id="e1322-134">Response</span></span>
<span data-ttu-id="e1322-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e1322-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-post-privilegedroleassignments.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
