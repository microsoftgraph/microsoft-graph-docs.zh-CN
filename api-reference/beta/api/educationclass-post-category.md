---
title: 创建 educationCategory
description: 创建新类别。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 16f7f4bf6ea58aa5d29ae63b95f4b104d0dd1d93
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35955365"
---
# <a name="create-educationcategory"></a><span data-ttu-id="e12a6-103">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="e12a6-103">Create educationCategory</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e12a6-104">在[educationClass](../resources/educationclass.md)上创建新的[educationCategory](../resources/educationcategory.md) 。</span><span class="sxs-lookup"><span data-stu-id="e12a6-104">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e12a6-105">权限</span><span class="sxs-lookup"><span data-stu-id="e12a6-105">Permissions</span></span>
<span data-ttu-id="e12a6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e12a6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e12a6-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e12a6-108">Permission type</span></span>      | <span data-ttu-id="e12a6-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e12a6-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e12a6-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e12a6-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="e12a6-111">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="e12a6-111">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="e12a6-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e12a6-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="e12a6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="e12a6-113">Not supported.</span></span>  |
|<span data-ttu-id="e12a6-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e12a6-114">Application</span></span> | <span data-ttu-id="e12a6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e12a6-115">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="e12a6-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e12a6-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories

```
## <a name="request-headers"></a><span data-ttu-id="e12a6-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="e12a6-117">Request headers</span></span>
| <span data-ttu-id="e12a6-118">标头</span><span class="sxs-lookup"><span data-stu-id="e12a6-118">Header</span></span>       | <span data-ttu-id="e12a6-119">值</span><span class="sxs-lookup"><span data-stu-id="e12a6-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e12a6-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="e12a6-120">Authorization</span></span>  | <span data-ttu-id="e12a6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e12a6-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e12a6-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e12a6-123">Content-Type</span></span>  | <span data-ttu-id="e12a6-124">application/json</span><span class="sxs-lookup"><span data-stu-id="e12a6-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e12a6-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="e12a6-125">Request body</span></span>
<span data-ttu-id="e12a6-126">在请求正文中, 提供[educationCategory](../resources/educationcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e12a6-126">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="e12a6-127">响应</span><span class="sxs-lookup"><span data-stu-id="e12a6-127">Response</span></span>
<span data-ttu-id="e12a6-128">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[educationCategory](../resources/educationcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e12a6-128">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e12a6-129">示例</span><span class="sxs-lookup"><span data-stu-id="e12a6-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e12a6-130">请求</span><span class="sxs-lookup"><span data-stu-id="e12a6-130">Request</span></span>
<span data-ttu-id="e12a6-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e12a6-131">The following is an example of the request.</span></span>
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
<span data-ttu-id="e12a6-132">在请求正文中, 提供[educationCategory](../resources/educationcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e12a6-132">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

##### <a name="response"></a><span data-ttu-id="e12a6-133">响应</span><span class="sxs-lookup"><span data-stu-id="e12a6-133">Response</span></span>
<span data-ttu-id="e12a6-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e12a6-134">The following is an example of the response.</span></span> 

><span data-ttu-id="e12a6-p103">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e12a6-p103">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
