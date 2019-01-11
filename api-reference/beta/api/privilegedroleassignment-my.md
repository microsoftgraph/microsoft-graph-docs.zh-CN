---
title: privilegedRoleAssignment： 我
description: 获取请求者特权的角色分配。
localization_priority: Normal
ms.openlocfilehash: fca950413d2f0a50b6ea9e09b859d2ecf926261b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840255"
---
# <a name="privilegedroleassignment-my"></a><span data-ttu-id="fd288-103">privilegedRoleAssignment： 我</span><span class="sxs-lookup"><span data-stu-id="fd288-103">privilegedRoleAssignment: my</span></span>

> <span data-ttu-id="fd288-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fd288-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd288-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fd288-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd288-106">获取请求者特权的角色分配。</span><span class="sxs-lookup"><span data-stu-id="fd288-106">Get the requestor's privileged role assignments.</span></span>

## <a name="permissions"></a><span data-ttu-id="fd288-107">权限</span><span class="sxs-lookup"><span data-stu-id="fd288-107">Permissions</span></span>
<span data-ttu-id="fd288-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd288-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd288-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd288-110">Permission type</span></span>      | <span data-ttu-id="fd288-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd288-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd288-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd288-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fd288-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd288-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd288-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd288-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd288-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd288-115">Not supported.</span></span>    |
|<span data-ttu-id="fd288-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd288-116">Application</span></span> | <span data-ttu-id="fd288-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd288-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fd288-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd288-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoleAssignments/my
```
## <a name="request-headers"></a><span data-ttu-id="fd288-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd288-119">Request headers</span></span>
| <span data-ttu-id="fd288-120">名称</span><span class="sxs-lookup"><span data-stu-id="fd288-120">Name</span></span>       | <span data-ttu-id="fd288-121">说明</span><span class="sxs-lookup"><span data-stu-id="fd288-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd288-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd288-122">Authorization</span></span>  | <span data-ttu-id="fd288-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fd288-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fd288-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd288-125">Request body</span></span>
<span data-ttu-id="fd288-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fd288-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd288-127">响应</span><span class="sxs-lookup"><span data-stu-id="fd288-127">Response</span></span>

<span data-ttu-id="fd288-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRoleAssignment](../resources/privilegedroleassignment.md)集合的对象。</span><span class="sxs-lookup"><span data-stu-id="fd288-128">If successful, this method returns `200 OK` response code and [privilegedRoleAssignment](../resources/privilegedroleassignment.md) collection object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd288-129">示例</span><span class="sxs-lookup"><span data-stu-id="fd288-129">Example</span></span>
<span data-ttu-id="fd288-130">下面是一个如何调用此 API 的示例。</span><span class="sxs-lookup"><span data-stu-id="fd288-130">Here is an example of how to call this API.</span></span>
##### <a name="request"></a><span data-ttu-id="fd288-131">请求</span><span class="sxs-lookup"><span data-stu-id="fd288-131">Request</span></span>
<span data-ttu-id="fd288-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd288-132">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "privilegedroleassignment_my"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoleAssignments/my
```

##### <a name="response"></a><span data-ttu-id="fd288-133">响应</span><span class="sxs-lookup"><span data-stu-id="fd288-133">Response</span></span>
<span data-ttu-id="fd288-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd288-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "privilegedRoleAssignment: my",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
