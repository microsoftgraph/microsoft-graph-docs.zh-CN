---
title: 创建 educationClass
description: 创建新课程。 此操作还会创建通用组。 当您使用此 API 创建类时，它会将特殊属性添加到组中，这将
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f17c356b4e6177fa3cba6a7e7aa9991c768c0e75
ms.sourcegitcommit: ef9e0fd8fb6047fa9272e98310eaed2c4e0a2660
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44353229"
---
# <a name="create-educationclass"></a><span data-ttu-id="4cd18-105">创建 educationClass</span><span class="sxs-lookup"><span data-stu-id="4cd18-105">Create educationClass</span></span>

<span data-ttu-id="4cd18-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4cd18-106">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4cd18-107">创建新课程。</span><span class="sxs-lookup"><span data-stu-id="4cd18-107">Create a new class.</span></span> <span data-ttu-id="4cd18-108">此操作还会创建通用组。</span><span class="sxs-lookup"><span data-stu-id="4cd18-108">This will also create a universal group.</span></span> <span data-ttu-id="4cd18-109">当您使用此 API 创建一个类时，它会将特殊的属性添加到组中，这将在使用组创建团队时，将在 Microsoft 团队中添加工作分配和特殊处理等功能。</span><span class="sxs-lookup"><span data-stu-id="4cd18-109">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams when teams are created using the group.</span></span> <span data-ttu-id="4cd18-110">请注意，此 API 仅创建通用组，不创建团队。</span><span class="sxs-lookup"><span data-stu-id="4cd18-110">Please note that this API only creates the universal group and does not create a team.</span></span> <span data-ttu-id="4cd18-111">Microsoft 团队为教师提供了用户界面，以使用此 API 创建的组为自己的类创建团队。</span><span class="sxs-lookup"><span data-stu-id="4cd18-111">Microsoft Teams provides a user interface for teachers to create teams for their own classes using the groups created by this API.</span></span>

## <a name="permissions"></a><span data-ttu-id="4cd18-112">权限</span><span class="sxs-lookup"><span data-stu-id="4cd18-112">Permissions</span></span>
<span data-ttu-id="4cd18-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4cd18-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4cd18-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="4cd18-115">Permission type</span></span>      | <span data-ttu-id="4cd18-116">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4cd18-116">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4cd18-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4cd18-117">Delegated (work or school account)</span></span> |  <span data-ttu-id="4cd18-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cd18-118">Not supported.</span></span>  |
|<span data-ttu-id="4cd18-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4cd18-119">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4cd18-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="4cd18-120">Not supported.</span></span>  |
|<span data-ttu-id="4cd18-121">Application</span><span class="sxs-lookup"><span data-stu-id="4cd18-121">Application</span></span> | <span data-ttu-id="4cd18-122">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4cd18-122">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="4cd18-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4cd18-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="4cd18-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="4cd18-124">Request headers</span></span>
| <span data-ttu-id="4cd18-125">标头</span><span class="sxs-lookup"><span data-stu-id="4cd18-125">Header</span></span>       | <span data-ttu-id="4cd18-126">值</span><span class="sxs-lookup"><span data-stu-id="4cd18-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4cd18-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="4cd18-127">Authorization</span></span>  | <span data-ttu-id="4cd18-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4cd18-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4cd18-130">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4cd18-130">Content-Type</span></span>  | <span data-ttu-id="4cd18-131">application/json</span><span class="sxs-lookup"><span data-stu-id="4cd18-131">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4cd18-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="4cd18-132">Request body</span></span>
<span data-ttu-id="4cd18-133">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4cd18-133">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="4cd18-134">响应</span><span class="sxs-lookup"><span data-stu-id="4cd18-134">Response</span></span>
<span data-ttu-id="4cd18-135">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4cd18-135">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4cd18-136">示例</span><span class="sxs-lookup"><span data-stu-id="4cd18-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4cd18-137">请求</span><span class="sxs-lookup"><span data-stu-id="4cd18-137">Request</span></span>
<span data-ttu-id="4cd18-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4cd18-138">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4cd18-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="4cd18-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_educationclass_from_educationroot"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes
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
# <a name="c"></a>[<span data-ttu-id="4cd18-140">C#</span><span class="sxs-lookup"><span data-stu-id="4cd18-140">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4cd18-141">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4cd18-141">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4cd18-142">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4cd18-142">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="4cd18-143">响应</span><span class="sxs-lookup"><span data-stu-id="4cd18-143">Response</span></span>
<span data-ttu-id="4cd18-144">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4cd18-144">The following is an example of the response.</span></span> 

><span data-ttu-id="4cd18-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="4cd18-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
