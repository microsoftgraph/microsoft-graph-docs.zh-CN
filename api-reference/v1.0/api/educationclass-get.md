---
title: 获取 educationClass
description: 从系统检索类
localization_priority: Normal
author: mlafleur
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 52f24e1f3c02b955874a78cdba447b697485f4a3
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232009"
---
# <a name="get-educationclass"></a><span data-ttu-id="0afd7-103">获取 educationClass</span><span class="sxs-lookup"><span data-stu-id="0afd7-103">Get educationClass</span></span>

<span data-ttu-id="0afd7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0afd7-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0afd7-105">从系统检索课程。</span><span class="sxs-lookup"><span data-stu-id="0afd7-105">Retrieve a class from the system.</span></span> <span data-ttu-id="0afd7-106">课程是带特殊属性的通用组，向系统表明该组是课程。</span><span class="sxs-lookup"><span data-stu-id="0afd7-106">A class is a universal group with a special property that indicates to the system that the group is a class.</span></span> <span data-ttu-id="0afd7-107">Group members represent the students;组管理员表示班级中的教师。</span><span class="sxs-lookup"><span data-stu-id="0afd7-107">Group members represent the students; group admins represent the teachers in the class.</span></span> <span data-ttu-id="0afd7-108">如果使用的是委派令牌，用户只会看到他们作为成员的课程。</span><span class="sxs-lookup"><span data-stu-id="0afd7-108">If you're using the delegated token, the user will only see classes in which they are members.</span></span>

## <a name="permissions"></a><span data-ttu-id="0afd7-109">权限</span><span class="sxs-lookup"><span data-stu-id="0afd7-109">Permissions</span></span>
<span data-ttu-id="0afd7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0afd7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0afd7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0afd7-112">Permission type</span></span>      | <span data-ttu-id="0afd7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0afd7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0afd7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0afd7-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="0afd7-115">EduRoster.ReadBasic</span><span class="sxs-lookup"><span data-stu-id="0afd7-115">EduRoster.ReadBasic</span></span>  |
|<span data-ttu-id="0afd7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0afd7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0afd7-117">不支持</span><span class="sxs-lookup"><span data-stu-id="0afd7-117">Not supported</span></span>  |
|<span data-ttu-id="0afd7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0afd7-118">Application</span></span> | <span data-ttu-id="0afd7-119">EduRoster.Read.All、EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0afd7-119">EduRoster.Read.All, EduRoster.ReadWrite.All</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0afd7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0afd7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0afd7-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0afd7-121">Optional query parameters</span></span>
<span data-ttu-id="0afd7-122">可以使用 `$select` 获取特定组属性，包括非默认返回的属性。</span><span class="sxs-lookup"><span data-stu-id="0afd7-122">You can use `$select` to get specific group properties, including those that are not returned by default.</span></span>

<span data-ttu-id="0afd7-123">有关 OData 查询选项的详细信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0afd7-123">For more information on OData query options, see [OData Query Parameters](/graph/query-parameters).</span></span>
## <a name="request-headers"></a><span data-ttu-id="0afd7-124">请求头</span><span class="sxs-lookup"><span data-stu-id="0afd7-124">Request headers</span></span>
| <span data-ttu-id="0afd7-125">标头</span><span class="sxs-lookup"><span data-stu-id="0afd7-125">Header</span></span>       | <span data-ttu-id="0afd7-126">值</span><span class="sxs-lookup"><span data-stu-id="0afd7-126">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0afd7-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="0afd7-127">Authorization</span></span>  | <span data-ttu-id="0afd7-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0afd7-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0afd7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="0afd7-130">Request body</span></span>
<span data-ttu-id="0afd7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0afd7-131">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="0afd7-132">响应</span><span class="sxs-lookup"><span data-stu-id="0afd7-132">Response</span></span>
<span data-ttu-id="0afd7-133">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0afd7-133">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0afd7-134">示例</span><span class="sxs-lookup"><span data-stu-id="0afd7-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0afd7-135">请求</span><span class="sxs-lookup"><span data-stu-id="0afd7-135">Request</span></span>
<span data-ttu-id="0afd7-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0afd7-136">Here is an example of the request.</span></span>

<span data-ttu-id="0afd7-137">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [educationClass](../resources/educationclass.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0afd7-137">If successful, this method returns a `200 OK` response code and an [educationClass](../resources/educationclass.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0afd7-138">示例</span><span class="sxs-lookup"><span data-stu-id="0afd7-138">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0afd7-139">请求</span><span class="sxs-lookup"><span data-stu-id="0afd7-139">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationclass"
}
-->

```http
GET /education/classes/{educationClassId}
```

### <a name="response"></a><span data-ttu-id="0afd7-140">响应</span><span class="sxs-lookup"><span data-stu-id="0afd7-140">Response</span></span>

><span data-ttu-id="0afd7-141">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0afd7-141">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationClass"
}
-->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": {
    "@odata.type": "#microsoft.graph.educationClass",
    "id": "64ef8ce5-8ce5-64ef-e58c-ef64e58cef64",
    "displayName": "String",
    "mailNickname": "String",
    "description": "String",
    "createdBy": {
      "@odata.type": "microsoft.graph.identitySet"
    },
    "classCode": "String",
    "externalName": "String",
    "externalId": "String",
    "externalSource": "String",
    "externalSourceDetail": "String",
    "grade": "String",
    "term": {
      "@odata.type": "microsoft.graph.educationTerm"
    }
  }
}
```
