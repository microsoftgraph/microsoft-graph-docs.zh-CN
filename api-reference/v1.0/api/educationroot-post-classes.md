---
title: 创建 educationClass
description: 创建新课程。 此操作还会创建通用组。 使用此 API 创建类时，它将向组添加特殊属性，这将
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 1e4a27c831f910c8952455c53322bda588f58e17
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52053137"
---
# <a name="create-educationclass"></a><span data-ttu-id="018d3-105">创建 educationClass</span><span class="sxs-lookup"><span data-stu-id="018d3-105">Create educationClass</span></span>

<span data-ttu-id="018d3-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="018d3-106">Namespace: microsoft.graph</span></span>

<span data-ttu-id="018d3-107">创建新课程。</span><span class="sxs-lookup"><span data-stu-id="018d3-107">Create a new class.</span></span> <span data-ttu-id="018d3-108">此操作还会创建通用组。</span><span class="sxs-lookup"><span data-stu-id="018d3-108">This will also create a universal group.</span></span> <span data-ttu-id="018d3-109">使用此 API 创建课程时，它会向组添加特殊属性，这将在使用组创建团队时在 Microsoft Teams 中添加分配和特殊处理等功能。</span><span class="sxs-lookup"><span data-stu-id="018d3-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="018d3-110">请注意，此 API 仅创建通用组，不会创建团队。</span><span class="sxs-lookup"><span data-stu-id="018d3-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="018d3-111">Microsoft Teams为教师提供用户界面，以使用此 API 创建的组创建自己的班级团队。</span><span class="sxs-lookup"><span data-stu-id="018d3-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="018d3-112">权限</span><span class="sxs-lookup"><span data-stu-id="018d3-112">Permissions</span></span>
<span data-ttu-id="018d3-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="018d3-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="018d3-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="018d3-115">Permission type</span></span>      | <span data-ttu-id="018d3-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="018d3-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="018d3-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="018d3-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="018d3-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="018d3-118">Not supported.</span></span>  |
|<span data-ttu-id="018d3-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="018d3-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="018d3-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="018d3-120">Not supported.</span></span>  |
|<span data-ttu-id="018d3-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="018d3-121">Application</span></span> | <span data-ttu-id="018d3-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="018d3-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="018d3-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="018d3-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="018d3-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="018d3-124">Request headers</span></span>
| <span data-ttu-id="018d3-125">标头</span><span class="sxs-lookup"><span data-stu-id="018d3-125">Header</span></span>       | <span data-ttu-id="018d3-126">值</span><span class="sxs-lookup"><span data-stu-id="018d3-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="018d3-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="018d3-127">Authorization</span></span>  | <span data-ttu-id="018d3-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="018d3-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="018d3-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="018d3-130">Content-Type</span></span>  | <span data-ttu-id="018d3-131">application/json</span><span class="sxs-lookup"><span data-stu-id="018d3-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="018d3-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="018d3-132">Request body</span></span>
<span data-ttu-id="018d3-133">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="018d3-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="018d3-134">响应</span><span class="sxs-lookup"><span data-stu-id="018d3-134">Response</span></span>
<span data-ttu-id="018d3-135">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="018d3-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="018d3-136">示例</span><span class="sxs-lookup"><span data-stu-id="018d3-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="018d3-137">请求</span><span class="sxs-lookup"><span data-stu-id="018d3-137">Request</span></span>
<span data-ttu-id="018d3-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="018d3-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="018d3-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="018d3-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes
Content-type: application/json
Content-length: 224

{
  "description": "Health Level 1",
  "classCode": "Health 501",
  "displayName": "Health 1",
  "externalId": "11019",
  "externalName": "Health Level 1",
  "externalSource": "sis",
  "mailNickname": "fineartschool.net"
}
```
# <a name="c"></a>[<span data-ttu-id="018d3-140">C#</span><span class="sxs-lookup"><span data-stu-id="018d3-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="018d3-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="018d3-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="018d3-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="018d3-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="018d3-143">Java</span><span class="sxs-lookup"><span data-stu-id="018d3-143">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="018d3-144">响应</span><span class="sxs-lookup"><span data-stu-id="018d3-144">Response</span></span>
<span data-ttu-id="018d3-145">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="018d3-145">The following is an example of the response.</span></span> 

><span data-ttu-id="018d3-146">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="018d3-146">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 224

{
    "id": "11019",
    "description": "Health Level 1",
    "classCode": "Health 501",
    "createdBy": {
      "user": {
        "displayName": "Susana Rocha",
        "id": "14012",
      }
    },
    "displayName": "Health 1",
    "externalId": "11019",
    "externalName": "Health Level 1",
    "externalSource": "sis",
    "mailNickname": "fineartschool.net"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create educationClass",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

