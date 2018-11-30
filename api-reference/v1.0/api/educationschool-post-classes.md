---
title: 将 educationClass 添加到 educationSchool
description: 向学校添加课程。
ms.openlocfilehash: bfd02ef790867d863485ddf301ebcf1f6985e028
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011533"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="2f2a7-103">将 educationClass 添加到 educationSchool</span><span class="sxs-lookup"><span data-stu-id="2f2a7-103">Add educationClass to educationSchool</span></span>

<span data-ttu-id="2f2a7-104">向学校添加课程。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="2f2a7-105">权限</span><span class="sxs-lookup"><span data-stu-id="2f2a7-105">Permissions</span></span>
<span data-ttu-id="2f2a7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f2a7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f2a7-108">Permission type</span></span>      | <span data-ttu-id="2f2a7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f2a7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f2a7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f2a7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f2a7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-111">Not supported.</span></span>  |
|<span data-ttu-id="2f2a7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f2a7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f2a7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-113">Not supported.</span></span>  |
|<span data-ttu-id="2f2a7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f2a7-114">Application</span></span> | <span data-ttu-id="2f2a7-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2f2a7-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f2a7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f2a7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="2f2a7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f2a7-117">Request headers</span></span>
| <span data-ttu-id="2f2a7-118">标头</span><span class="sxs-lookup"><span data-stu-id="2f2a7-118">Header</span></span>       | <span data-ttu-id="2f2a7-119">值</span><span class="sxs-lookup"><span data-stu-id="2f2a7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f2a7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f2a7-120">Authorization</span></span>  | <span data-ttu-id="2f2a7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f2a7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f2a7-123">Content-Type</span></span>  | <span data-ttu-id="2f2a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2f2a7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f2a7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f2a7-125">Request body</span></span>
<span data-ttu-id="2f2a7-126">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2f2a7-127">响应</span><span class="sxs-lookup"><span data-stu-id="2f2a7-127">Response</span></span>
<span data-ttu-id="2f2a7-128">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f2a7-129">示例</span><span class="sxs-lookup"><span data-stu-id="2f2a7-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f2a7-130">请求</span><span class="sxs-lookup"><span data-stu-id="2f2a7-130">Request</span></span>
<span data-ttu-id="2f2a7-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-131">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationschool"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/schools/{school-id}/classes/$ref
Content-type: application/json
Content-length: 224

{
 "@odata.id":"https://graph.microsoft.com/v1.0/education/classes/11006"
}
```

##### <a name="response"></a><span data-ttu-id="2f2a7-132">响应</span><span class="sxs-lookup"><span data-stu-id="2f2a7-132">Response</span></span> 
<span data-ttu-id="2f2a7-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f2a7-133">The following is an example of the response.</span></span> 

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