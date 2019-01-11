---
title: 添加学生
description: 向课程添加成员。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 2fda89865e706fb64deb40d3791431cac0a57e1b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27824197"
---
# <a name="add-a-student"></a><span data-ttu-id="e8d81-103">添加学生</span><span class="sxs-lookup"><span data-stu-id="e8d81-103">Add a student</span></span>

> <span data-ttu-id="e8d81-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8d81-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8d81-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8d81-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8d81-106">向课程添加成员。</span><span class="sxs-lookup"><span data-stu-id="e8d81-106">Add a member to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="e8d81-107">权限</span><span class="sxs-lookup"><span data-stu-id="e8d81-107">Permissions</span></span>
<span data-ttu-id="e8d81-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8d81-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8d81-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8d81-110">Permission type</span></span>      | <span data-ttu-id="e8d81-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e8d81-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e8d81-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8d81-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e8d81-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8d81-113">Not supported.</span></span>  |
|<span data-ttu-id="e8d81-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8d81-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e8d81-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8d81-115">Not supported.</span></span>  |
|<span data-ttu-id="e8d81-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8d81-116">Application</span></span> | <span data-ttu-id="e8d81-117">EduRoster.ReadWrite.All 以及 Member.Read.Hidden</span><span class="sxs-lookup"><span data-stu-id="e8d81-117">EduRoster.ReadWrite.All plus Member.Read.Hidden</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e8d81-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8d81-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e8d81-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8d81-119">Request headers</span></span>
| <span data-ttu-id="e8d81-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8d81-120">Header</span></span>       | <span data-ttu-id="e8d81-121">值</span><span class="sxs-lookup"><span data-stu-id="e8d81-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e8d81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8d81-122">Authorization</span></span>  | <span data-ttu-id="e8d81-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e8d81-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e8d81-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e8d81-125">Content-Type</span></span>  | <span data-ttu-id="e8d81-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8d81-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e8d81-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8d81-127">Request body</span></span>
<span data-ttu-id="e8d81-128">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8d81-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e8d81-129">响应</span><span class="sxs-lookup"><span data-stu-id="e8d81-129">Response</span></span>
<span data-ttu-id="e8d81-130">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e8d81-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8d81-131">示例</span><span class="sxs-lookup"><span data-stu-id="e8d81-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e8d81-132">请求</span><span class="sxs-lookup"><span data-stu-id="e8d81-132">Request</span></span>
<span data-ttu-id="e8d81-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e8d81-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11011/members/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/13015"
}
```

##### <a name="response"></a><span data-ttu-id="e8d81-134">响应</span><span class="sxs-lookup"><span data-stu-id="e8d81-134">Response</span></span>
<span data-ttu-id="e8d81-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e8d81-135">The following is an example of the response.</span></span> 


<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
