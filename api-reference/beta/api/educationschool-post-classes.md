---
title: 将 educationClass 添加到 educationSchool
description: 向学校添加课程。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 890036aab7c7271a363357496892204261c93918
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35441441"
---
# <a name="add-educationclass-to-educationschool"></a><span data-ttu-id="a1b36-103">将 educationClass 添加到 educationSchool</span><span class="sxs-lookup"><span data-stu-id="a1b36-103">Add educationClass to educationSchool</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a1b36-104">向学校添加课程。</span><span class="sxs-lookup"><span data-stu-id="a1b36-104">Add a class to a school.</span></span>

## <a name="permissions"></a><span data-ttu-id="a1b36-105">权限</span><span class="sxs-lookup"><span data-stu-id="a1b36-105">Permissions</span></span>
<span data-ttu-id="a1b36-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1b36-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1b36-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1b36-108">Permission type</span></span>      | <span data-ttu-id="a1b36-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a1b36-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a1b36-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1b36-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a1b36-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1b36-111">Not supported.</span></span>  |
|<span data-ttu-id="a1b36-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1b36-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a1b36-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1b36-113">Not supported.</span></span>  |
|<span data-ttu-id="a1b36-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1b36-114">Application</span></span> | <span data-ttu-id="a1b36-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1b36-115">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a1b36-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1b36-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/schools/{id}/classes/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a1b36-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1b36-117">Request headers</span></span>
| <span data-ttu-id="a1b36-118">标头</span><span class="sxs-lookup"><span data-stu-id="a1b36-118">Header</span></span>       | <span data-ttu-id="a1b36-119">值</span><span class="sxs-lookup"><span data-stu-id="a1b36-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a1b36-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1b36-120">Authorization</span></span>  | <span data-ttu-id="a1b36-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a1b36-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a1b36-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a1b36-123">Content-Type</span></span>  | <span data-ttu-id="a1b36-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1b36-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a1b36-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1b36-125">Request body</span></span>
<span data-ttu-id="a1b36-126">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1b36-126">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="a1b36-127">响应</span><span class="sxs-lookup"><span data-stu-id="a1b36-127">Response</span></span>
<span data-ttu-id="a1b36-128">如果成功，此方法会在响应正文中返回 `204 No Content` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1b36-128">If successful, this method returns a `204 No Content` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1b36-129">示例</span><span class="sxs-lookup"><span data-stu-id="a1b36-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a1b36-130">请求</span><span class="sxs-lookup"><span data-stu-id="a1b36-130">Request</span></span>
<span data-ttu-id="a1b36-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a1b36-131">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="a1b36-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="a1b36-132">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="a1b36-133">Javascript</span><span class="sxs-lookup"><span data-stu-id="a1b36-133">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="a1b36-134">目标-C</span><span class="sxs-lookup"><span data-stu-id="a1b36-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="a1b36-135">响应</span><span class="sxs-lookup"><span data-stu-id="a1b36-135">Response</span></span> 
<span data-ttu-id="a1b36-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a1b36-136">The following is an example of the response.</span></span> 

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
<!--
{
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
