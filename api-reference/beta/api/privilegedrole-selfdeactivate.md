---
title: 'privilegedRole: selfDeactivate'
description: 停用的角色分配给请求者。
localization_priority: Normal
ms.openlocfilehash: 7175af64e7e36087bd048cd6e160393e2bf6377e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528688"
---
# <a name="privilegedrole-selfdeactivate"></a><span data-ttu-id="1e59c-103">privilegedRole: selfDeactivate</span><span class="sxs-lookup"><span data-stu-id="1e59c-103">privilegedRole: selfDeactivate</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e59c-104">停用的角色分配给请求者。</span><span class="sxs-lookup"><span data-stu-id="1e59c-104">Deactivate the role that is assigned to the requestor.</span></span>
## <a name="permissions"></a><span data-ttu-id="1e59c-105">权限</span><span class="sxs-lookup"><span data-stu-id="1e59c-105">Permissions</span></span>
<span data-ttu-id="1e59c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e59c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="1e59c-108">请求者只能调用```selfDeactivate```角色分配给他。</span><span class="sxs-lookup"><span data-stu-id="1e59c-108">The requestor can only call ```selfDeactivate``` for the role that is assigned to him.</span></span> 

|<span data-ttu-id="1e59c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e59c-109">Permission type</span></span>      | <span data-ttu-id="1e59c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e59c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1e59c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e59c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1e59c-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1e59c-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1e59c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e59c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e59c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e59c-114">Not supported.</span></span>    |
|<span data-ttu-id="1e59c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e59c-115">Application</span></span> | <span data-ttu-id="1e59c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e59c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1e59c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e59c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedRoles/{id}/selfDeactivate
```

<span data-ttu-id="1e59c-118">请注意，``<id>``是目标角色 id。</span><span class="sxs-lookup"><span data-stu-id="1e59c-118">Note that ``<id>`` is the target role id.</span></span>
## <a name="request-headers"></a><span data-ttu-id="1e59c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e59c-119">Request headers</span></span>
| <span data-ttu-id="1e59c-120">名称</span><span class="sxs-lookup"><span data-stu-id="1e59c-120">Name</span></span>       | <span data-ttu-id="1e59c-121">说明</span><span class="sxs-lookup"><span data-stu-id="1e59c-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1e59c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e59c-122">Authorization</span></span>  | <span data-ttu-id="1e59c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e59c-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1e59c-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e59c-125">Request body</span></span>
<span data-ttu-id="1e59c-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e59c-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e59c-127">响应</span><span class="sxs-lookup"><span data-stu-id="1e59c-127">Response</span></span>

<span data-ttu-id="1e59c-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1e59c-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) object in the response body.</span></span>

<span data-ttu-id="1e59c-129">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="1e59c-129">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1e59c-130">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="1e59c-130">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="1e59c-131">示例</span><span class="sxs-lookup"><span data-stu-id="1e59c-131">Example</span></span>
<span data-ttu-id="1e59c-132">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="1e59c-132">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="1e59c-133">请求</span><span class="sxs-lookup"><span data-stu-id="1e59c-133">Request</span></span>
<span data-ttu-id="1e59c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1e59c-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedrole_selfdeactivate"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedRoles/{id}/selfDeactivate
```

##### <a name="response"></a><span data-ttu-id="1e59c-135">响应</span><span class="sxs-lookup"><span data-stu-id="1e59c-135">Response</span></span>
<span data-ttu-id="1e59c-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1e59c-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
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
  "description": "privilegedRole: selfDeactivate",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-selfdeactivate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
