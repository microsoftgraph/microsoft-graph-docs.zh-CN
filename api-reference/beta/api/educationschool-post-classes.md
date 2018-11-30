---
title: 将 educationClass 添加到 educationSchool
description: 向学校添加课程。
ms.openlocfilehash: 0502031c8349d659f0596a8a6ff387bdc83fde85
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043929"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="e36db-103">将 educationClass 添加到 educationSchool</span><span class="sxs-lookup"><span data-stu-id="e36db-103">Add educationClass to educationSchool</span></span>

> <span data-ttu-id="e36db-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e36db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e36db-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e36db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e36db-106">向学校添加课程。</span><span class="sxs-lookup"><span data-stu-id="e36db-106">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="e36db-107">权限</span><span class="sxs-lookup"><span data-stu-id="e36db-107">Permissions</span></span>
<span data-ttu-id="e36db-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e36db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e36db-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e36db-110">Permission type</span></span>      | <span data-ttu-id="e36db-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e36db-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e36db-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e36db-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="e36db-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e36db-113">Not supported.</span></span>  |
|<span data-ttu-id="e36db-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e36db-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e36db-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e36db-115">Not supported.</span></span>  |
|<span data-ttu-id="e36db-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="e36db-116">Application</span></span> | <span data-ttu-id="e36db-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e36db-117">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e36db-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e36db-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="e36db-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e36db-119">Request headers</span></span>
| <span data-ttu-id="e36db-120">标头</span><span class="sxs-lookup"><span data-stu-id="e36db-120">Header</span></span>       | <span data-ttu-id="e36db-121">值</span><span class="sxs-lookup"><span data-stu-id="e36db-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e36db-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e36db-122">Authorization</span></span>  | <span data-ttu-id="e36db-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e36db-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e36db-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e36db-125">Content-Type</span></span>  | <span data-ttu-id="e36db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e36db-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e36db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e36db-127">Request body</span></span>
<span data-ttu-id="e36db-128">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e36db-128">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e36db-129">响应</span><span class="sxs-lookup"><span data-stu-id="e36db-129">Response</span></span>
<span data-ttu-id="e36db-130">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e36db-130">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e36db-131">示例</span><span class="sxs-lookup"><span data-stu-id="e36db-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e36db-132">请求</span><span class="sxs-lookup"><span data-stu-id="e36db-132">Request</span></span>
<span data-ttu-id="e36db-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e36db-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/beta/education/schools/10002/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/beta/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="e36db-134">响应</span><span class="sxs-lookup"><span data-stu-id="e36db-134">Response</span></span> 
<span data-ttu-id="e36db-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e36db-135">The following is an example of the response.</span></span> 

<!-- Add the educationClass resource to the response. -->

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->