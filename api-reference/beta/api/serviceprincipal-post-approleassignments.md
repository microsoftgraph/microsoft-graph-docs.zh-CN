---
title: 创建 appRoleAssignment
description: 使用此 API 创建新的 appRoleAssignment。
localization_priority: Normal
ms.openlocfilehash: cb171e4d6149de5ba169dbf7ad48e87cb055fb47
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33335806"
---
# <a name="create-approleassignment"></a><span data-ttu-id="92d93-103">创建 appRoleAssignment</span><span class="sxs-lookup"><span data-stu-id="92d93-103">Create appRoleAssignment</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="92d93-104">使用此 API 创建新的 appRoleAssignment。</span><span class="sxs-lookup"><span data-stu-id="92d93-104">Use this API to create a new appRoleAssignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="92d93-105">权限</span><span class="sxs-lookup"><span data-stu-id="92d93-105">Permissions</span></span>
<span data-ttu-id="92d93-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="92d93-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92d93-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="92d93-108">Permission type</span></span>      | <span data-ttu-id="92d93-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="92d93-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="92d93-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="92d93-110">Delegated (work or school account)</span></span> | <span data-ttu-id="92d93-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="92d93-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="92d93-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="92d93-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="92d93-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="92d93-113">Not supported.</span></span>    |
|<span data-ttu-id="92d93-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="92d93-114">Application</span></span> | <span data-ttu-id="92d93-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="92d93-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="92d93-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="92d93-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /servicePrincipals/{id}/appRoleAssignments

```
## <a name="request-headers"></a><span data-ttu-id="92d93-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="92d93-117">Request headers</span></span>
| <span data-ttu-id="92d93-118">名称</span><span class="sxs-lookup"><span data-stu-id="92d93-118">Name</span></span>       | <span data-ttu-id="92d93-119">类型</span><span class="sxs-lookup"><span data-stu-id="92d93-119">Type</span></span> | <span data-ttu-id="92d93-120">说明</span><span class="sxs-lookup"><span data-stu-id="92d93-120">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="92d93-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="92d93-121">Authorization</span></span>  | <span data-ttu-id="92d93-122">string</span><span class="sxs-lookup"><span data-stu-id="92d93-122">string</span></span>  | <span data-ttu-id="92d93-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="92d93-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="92d93-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="92d93-125">Request body</span></span>
<span data-ttu-id="92d93-126">在请求正文中, 提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92d93-126">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="92d93-127">响应</span><span class="sxs-lookup"><span data-stu-id="92d93-127">Response</span></span>

<span data-ttu-id="92d93-128">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[appRoleAssignment](../resources/approleassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="92d93-128">If successful, this method returns `201 Created` response code and [appRoleAssignment](../resources/approleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92d93-129">示例</span><span class="sxs-lookup"><span data-stu-id="92d93-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="92d93-130">请求</span><span class="sxs-lookup"><span data-stu-id="92d93-130">Request</span></span>
<span data-ttu-id="92d93-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="92d93-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_approleassignment_from_serviceprincipal"
}-->
```http
POST https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
Content-type: application/json
Content-length: 233

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```
<span data-ttu-id="92d93-132">在请求正文中, 提供[appRoleAssignment](../resources/approleassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="92d93-132">In the request body, supply a JSON representation of [appRoleAssignment](../resources/approleassignment.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="92d93-133">响应</span><span class="sxs-lookup"><span data-stu-id="92d93-133">Response</span></span>
<span data-ttu-id="92d93-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="92d93-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.appRoleAssignment"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 253

{
  "creationTimestamp": "2016-10-19T10:37:00Z",
  "id": "id-value",
  "principalDisplayName": "principalDisplayName-value",
  "principalId": "principalId-value",
  "principalType": "principalType-value",
  "resourceDisplayName": "resourceDisplayName-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create appRoleAssignment",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
