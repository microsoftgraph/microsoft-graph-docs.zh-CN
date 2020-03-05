---
title: 创建 educationCategory
description: 创建新类别。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: db552b9b452453c3efed72c7d94fc14fa1cbe6c1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42426421"
---
# <a name="create-educationcategory"></a><span data-ttu-id="2f194-103">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="2f194-103">Create educationCategory</span></span>

<span data-ttu-id="2f194-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="2f194-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f194-105">在[educationClass](../resources/educationclass.md)上创建新的[educationCategory](../resources/educationcategory.md) 。</span><span class="sxs-lookup"><span data-stu-id="2f194-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2f194-106">权限</span><span class="sxs-lookup"><span data-stu-id="2f194-106">Permissions</span></span>
<span data-ttu-id="2f194-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2f194-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2f194-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2f194-109">Permission type</span></span>      | <span data-ttu-id="2f194-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2f194-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2f194-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2f194-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="2f194-112">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="2f194-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="2f194-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2f194-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="2f194-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f194-114">Not supported.</span></span>  |
|<span data-ttu-id="2f194-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2f194-115">Application</span></span> | <span data-ttu-id="2f194-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2f194-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="2f194-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2f194-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="2f194-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2f194-118">Request headers</span></span>
| <span data-ttu-id="2f194-119">标头</span><span class="sxs-lookup"><span data-stu-id="2f194-119">Header</span></span>       | <span data-ttu-id="2f194-120">值</span><span class="sxs-lookup"><span data-stu-id="2f194-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="2f194-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2f194-121">Authorization</span></span>  | <span data-ttu-id="2f194-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2f194-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2f194-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2f194-124">Content-Type</span></span>  | <span data-ttu-id="2f194-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2f194-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2f194-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2f194-126">Request body</span></span>
<span data-ttu-id="2f194-127">在请求正文中，提供[educationCategory](../resources/educationcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f194-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="2f194-128">响应</span><span class="sxs-lookup"><span data-stu-id="2f194-128">Response</span></span>
<span data-ttu-id="2f194-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和[educationCategory](../resources/educationcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2f194-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2f194-130">示例</span><span class="sxs-lookup"><span data-stu-id="2f194-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2f194-131">请求</span><span class="sxs-lookup"><span data-stu-id="2f194-131">Request</span></span>
<span data-ttu-id="2f194-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2f194-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11019/assignmentCategories
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="2f194-133">在请求正文中，提供[educationCategory](../resources/educationcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f194-133">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="2f194-134">响应</span><span class="sxs-lookup"><span data-stu-id="2f194-134">Response</span></span>
<span data-ttu-id="2f194-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2f194-135">The following is an example of the response.</span></span> 

><span data-ttu-id="2f194-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2f194-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 85

{
    "displayName": "Quizzes",
    "id": "ec98f158-341d-4fea-9f8c-14a250d489ac"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
