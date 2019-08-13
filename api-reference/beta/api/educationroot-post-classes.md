---
title: 创建 educationClass
description: 创建新课程。 此操作还会创建通用组。 当您使用此 API 创建类时, 它会将特殊属性添加到组中, 这将
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: eb72a1e557240a988c71ae47d0c855ea0c3025a5
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36323960"
---
# <a name="create-educationclass"></a><span data-ttu-id="17dfb-105">创建 educationClass</span><span class="sxs-lookup"><span data-stu-id="17dfb-105">Create educationClass</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="17dfb-106">创建新课程。</span><span class="sxs-lookup"><span data-stu-id="17dfb-106">Create a new class.</span></span> <span data-ttu-id="17dfb-107">此操作还会创建通用组。</span><span class="sxs-lookup"><span data-stu-id="17dfb-107">This will also create a universal group.</span></span> <span data-ttu-id="17dfb-108">当使用此 API 创建课程时，会向组添加特殊属性，继而在 Microsoft Teams 中添加分配和特殊处理等功能。</span><span class="sxs-lookup"><span data-stu-id="17dfb-108">When you use this API to create a class, it will add special properties to the group, which will add features such as assignments and special handling within Microsoft Teams.</span></span>

## <a name="permissions"></a><span data-ttu-id="17dfb-109">权限</span><span class="sxs-lookup"><span data-stu-id="17dfb-109">Permissions</span></span>
<span data-ttu-id="17dfb-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17dfb-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="17dfb-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="17dfb-112">Permission type</span></span>      | <span data-ttu-id="17dfb-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17dfb-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17dfb-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17dfb-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="17dfb-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="17dfb-115">Not supported.</span></span>  |
|<span data-ttu-id="17dfb-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17dfb-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="17dfb-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="17dfb-117">Not supported.</span></span>  |
|<span data-ttu-id="17dfb-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="17dfb-118">Application</span></span> | <span data-ttu-id="17dfb-119">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17dfb-119">EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="17dfb-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17dfb-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes
```
## <a name="request-headers"></a><span data-ttu-id="17dfb-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="17dfb-121">Request headers</span></span>
| <span data-ttu-id="17dfb-122">标头</span><span class="sxs-lookup"><span data-stu-id="17dfb-122">Header</span></span>       | <span data-ttu-id="17dfb-123">值</span><span class="sxs-lookup"><span data-stu-id="17dfb-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="17dfb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="17dfb-124">Authorization</span></span>  | <span data-ttu-id="17dfb-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17dfb-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="17dfb-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="17dfb-127">Content-Type</span></span>  | <span data-ttu-id="17dfb-128">application/json</span><span class="sxs-lookup"><span data-stu-id="17dfb-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="17dfb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="17dfb-129">Request body</span></span>
<span data-ttu-id="17dfb-130">在请求正文中，提供 [educationClass](../resources/educationclass.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="17dfb-130">In the request body, supply a JSON representation of an [educationClass](../resources/educationclass.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="17dfb-131">响应</span><span class="sxs-lookup"><span data-stu-id="17dfb-131">Response</span></span>
<span data-ttu-id="17dfb-132">如果成功，此方法会在响应正文中返回 `201 Created` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="17dfb-132">If successful, this method returns a `201 Created` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="17dfb-133">示例</span><span class="sxs-lookup"><span data-stu-id="17dfb-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17dfb-134">请求</span><span class="sxs-lookup"><span data-stu-id="17dfb-134">Request</span></span>
<span data-ttu-id="17dfb-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="17dfb-135">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="17dfb-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="17dfb-136">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="17dfb-137">C#</span><span class="sxs-lookup"><span data-stu-id="17dfb-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-educationclass-from-educationroot-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="17dfb-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="17dfb-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-educationclass-from-educationroot-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="17dfb-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="17dfb-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-educationclass-from-educationroot-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="17dfb-140">Java</span><span class="sxs-lookup"><span data-stu-id="17dfb-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-educationclass-from-educationroot-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="17dfb-141">响应</span><span class="sxs-lookup"><span data-stu-id="17dfb-141">Response</span></span>
<span data-ttu-id="17dfb-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="17dfb-142">The following is an example of the response.</span></span> 

><span data-ttu-id="17dfb-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="17dfb-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
