---
title: 向 educationSchool 添加 educationUser
description: 向学校添加用户。
ms.openlocfilehash: cdccc9147f8a6eb0ba8bd2c79b8ce28ecddb514f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042362"
---
# <a name="add-educationuser-to-an-educationschool"></a><span data-ttu-id="da9ac-103">向 educationSchool 添加 educationUser</span><span class="sxs-lookup"><span data-stu-id="da9ac-103">Add educationUser to an educationSchool</span></span>

> <span data-ttu-id="da9ac-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da9ac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da9ac-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da9ac-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="da9ac-106">向学校添加用户。</span><span class="sxs-lookup"><span data-stu-id="da9ac-106">Add a user to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="da9ac-107">权限</span><span class="sxs-lookup"><span data-stu-id="da9ac-107">Permissions</span></span>
<span data-ttu-id="da9ac-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da9ac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da9ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da9ac-110">Permission type</span></span>      | <span data-ttu-id="da9ac-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da9ac-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="da9ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da9ac-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="da9ac-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="da9ac-113">Not supported.</span></span>  |
|<span data-ttu-id="da9ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da9ac-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="da9ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da9ac-115">Not supported.</span></span>  |
|<span data-ttu-id="da9ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da9ac-116">Application</span></span> | <span data-ttu-id="da9ac-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da9ac-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="da9ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da9ac-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/users/$ref
```
## <a name="request-headers"></a><span data-ttu-id="da9ac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="da9ac-119">Request headers</span></span>
| <span data-ttu-id="da9ac-120">标头</span><span class="sxs-lookup"><span data-stu-id="da9ac-120">Header</span></span>       | <span data-ttu-id="da9ac-121">值</span><span class="sxs-lookup"><span data-stu-id="da9ac-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="da9ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="da9ac-122">Authorization</span></span>  | <span data-ttu-id="da9ac-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="da9ac-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="da9ac-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="da9ac-125">Content-Type</span></span>  | <span data-ttu-id="da9ac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da9ac-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="da9ac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da9ac-127">Request body</span></span>
<span data-ttu-id="da9ac-128">在请求正文中，提供 [educationUser](../resources/educationuser.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da9ac-128">In the request body, supply a JSON representation of an [educationUser](../resources/educationuser.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="da9ac-129">响应</span><span class="sxs-lookup"><span data-stu-id="da9ac-129">Response</span></span>
<span data-ttu-id="da9ac-130">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da9ac-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da9ac-131">示例</span><span class="sxs-lookup"><span data-stu-id="da9ac-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="da9ac-132">请求</span><span class="sxs-lookup"><span data-stu-id="da9ac-132">Request</span></span>
<span data-ttu-id="da9ac-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="da9ac-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationuser_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/<id>/users/$ref
Content-type: application/json
Content-length: 56

{
  "@odata.id":"https://graph.microsoft.com/beta/education/users/14008"
}
```

##### <a name="response"></a><span data-ttu-id="da9ac-134">响应</span><span class="sxs-lookup"><span data-stu-id="da9ac-134">Response</span></span>
<span data-ttu-id="da9ac-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="da9ac-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

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