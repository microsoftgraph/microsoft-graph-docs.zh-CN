---
title: 添加教师
description: 向课程添加教师。
ms.openlocfilehash: 05692196e89f927b0a0a510c0491741313d38e70
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008893"
---
# <a name="add-teacher"></a><span data-ttu-id="01bb2-103">添加教师</span><span class="sxs-lookup"><span data-stu-id="01bb2-103">Add teacher</span></span>

<span data-ttu-id="01bb2-104">向课程添加教师。</span><span class="sxs-lookup"><span data-stu-id="01bb2-104">Add a teacher to a class.</span></span>

## <a name="permissions"></a><span data-ttu-id="01bb2-105">权限</span><span class="sxs-lookup"><span data-stu-id="01bb2-105">Permissions</span></span>
<span data-ttu-id="01bb2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01bb2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01bb2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="01bb2-108">Permission type</span></span>      | <span data-ttu-id="01bb2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01bb2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01bb2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01bb2-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="01bb2-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="01bb2-111">Not supported.</span></span>  |
|<span data-ttu-id="01bb2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01bb2-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="01bb2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="01bb2-113">Not supported.</span></span>  |
|<span data-ttu-id="01bb2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="01bb2-114">Application</span></span> | <span data-ttu-id="01bb2-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01bb2-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="01bb2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01bb2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/teachers/$ref
```
## <a name="request-headers"></a><span data-ttu-id="01bb2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="01bb2-117">Request headers</span></span>
| <span data-ttu-id="01bb2-118">标头</span><span class="sxs-lookup"><span data-stu-id="01bb2-118">Header</span></span>       | <span data-ttu-id="01bb2-119">值</span><span class="sxs-lookup"><span data-stu-id="01bb2-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="01bb2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="01bb2-120">Authorization</span></span>  | <span data-ttu-id="01bb2-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01bb2-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="01bb2-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="01bb2-123">Content-Type</span></span>  | <span data-ttu-id="01bb2-124">application/json</span><span class="sxs-lookup"><span data-stu-id="01bb2-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="01bb2-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="01bb2-125">Request body</span></span>
<span data-ttu-id="01bb2-126">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01bb2-126">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="01bb2-127">响应</span><span class="sxs-lookup"><span data-stu-id="01bb2-127">Response</span></span>
<span data-ttu-id="01bb2-128">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="01bb2-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01bb2-129">示例</span><span class="sxs-lookup"><span data-stu-id="01bb2-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01bb2-130">请求</span><span class="sxs-lookup"><span data-stu-id="01bb2-130">Request</span></span>
<span data-ttu-id="01bb2-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="01bb2-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/{class-id}/teachers/$ref
Content-type: application/json
Content-length: 508

{
  "@odata.id":"https://graph.microsoft.com/v1.0/education/users/14011"
}
```

##### <a name="response"></a><span data-ttu-id="01bb2-132">响应</span><span class="sxs-lookup"><span data-stu-id="01bb2-132">Response</span></span>
<span data-ttu-id="01bb2-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="01bb2-133">The following is an example of the response.</span></span> 

<!-- Add the educationClass object to the response -->

><span data-ttu-id="01bb2-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="01bb2-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
