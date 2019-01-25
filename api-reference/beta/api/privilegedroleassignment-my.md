---
title: privilegedRoleAssignment： 我
description: 获取请求者特权的角色分配。
localization_priority: Normal
ms.openlocfilehash: fe3f0486d7c5f011abbac60deed831b798802aef
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29520058"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="59dcb-103">privilegedRoleAssignment： 我</span><span class="sxs-lookup"><span data-stu-id="59dcb-103">privilegedRoleAssignment: my</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="59dcb-104">获取请求者特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="59dcb-104">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="59dcb-105">权限</span><span class="sxs-lookup"><span data-stu-id="59dcb-105">Permissions</span></span>
<span data-ttu-id="59dcb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59dcb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59dcb-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="59dcb-108">Permission type</span></span>      | <span data-ttu-id="59dcb-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59dcb-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59dcb-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59dcb-110">Delegated (work or school account)</span></span> | <span data-ttu-id="59dcb-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="59dcb-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="59dcb-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59dcb-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59dcb-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="59dcb-113">Not supported.</span></span>    |
|<span data-ttu-id="59dcb-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="59dcb-114">Application</span></span> | <span data-ttu-id="59dcb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59dcb-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="59dcb-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59dcb-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="59dcb-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="59dcb-117">Request headers</span></span>
| <span data-ttu-id="59dcb-118">名称</span><span class="sxs-lookup"><span data-stu-id="59dcb-118">Name</span></span>       | <span data-ttu-id="59dcb-119">说明</span><span class="sxs-lookup"><span data-stu-id="59dcb-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="59dcb-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="59dcb-120">Authorization</span></span>  | <span data-ttu-id="59dcb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59dcb-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59dcb-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="59dcb-123">Request body</span></span>
<span data-ttu-id="59dcb-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59dcb-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59dcb-125">响应</span><span class="sxs-lookup"><span data-stu-id="59dcb-125">Response</span></span>

<span data-ttu-id="59dcb-126">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="59dcb-126">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59dcb-127">示例</span><span class="sxs-lookup"><span data-stu-id="59dcb-127">Example</span></span>
<span data-ttu-id="59dcb-128">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="59dcb-128">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="59dcb-129">请求</span><span class="sxs-lookup"><span data-stu-id="59dcb-129">Request</span></span>
<span data-ttu-id="59dcb-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="59dcb-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="59dcb-131">响应</span><span class="sxs-lookup"><span data-stu-id="59dcb-131">Response</span></span>
<span data-ttu-id="59dcb-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="59dcb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRoleAssignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 237

{
  "value": [
    {
      "id": "id-value",
      "userId": "userId-value",
      "roleId": "roleId-value",
      "isElevated": true,
      "expirationDateTime": "2016-10-19T10:37:00Z",
      "resultMessage": "resultMessage-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedroleassignment-my.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
