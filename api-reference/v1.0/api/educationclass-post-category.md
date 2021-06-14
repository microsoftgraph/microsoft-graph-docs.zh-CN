---
title: 创建 educationCategory
description: 创建新类别。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: b6a2c92740db75350b5c1cefcd35c2b50723b55c
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52911395"
---
# <a name="create-educationcategory"></a><span data-ttu-id="8eccd-103">创建 educationCategory</span><span class="sxs-lookup"><span data-stu-id="8eccd-103">Create educationCategory</span></span>

<span data-ttu-id="8eccd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8eccd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8eccd-105">在[educationClass 上创建新的 educationCategory。](../resources/educationcategory.md) [](../resources/educationclass.md)</span><span class="sxs-lookup"><span data-stu-id="8eccd-105">Creates a new [educationCategory](../resources/educationcategory.md) on an [educationClass](../resources/educationclass.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8eccd-106">权限</span><span class="sxs-lookup"><span data-stu-id="8eccd-106">Permissions</span></span>
<span data-ttu-id="8eccd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8eccd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8eccd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8eccd-109">Permission type</span></span>      | <span data-ttu-id="8eccd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8eccd-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8eccd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8eccd-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="8eccd-112">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="8eccd-112">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="8eccd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8eccd-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="8eccd-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eccd-114">Not supported.</span></span>  |
|<span data-ttu-id="8eccd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8eccd-115">Application</span></span> | <span data-ttu-id="8eccd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="8eccd-116">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="8eccd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8eccd-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignmentCategories/$entity
```
## <a name="request-headers"></a><span data-ttu-id="8eccd-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8eccd-118">Request headers</span></span>
| <span data-ttu-id="8eccd-119">标头</span><span class="sxs-lookup"><span data-stu-id="8eccd-119">Header</span></span>       | <span data-ttu-id="8eccd-120">值</span><span class="sxs-lookup"><span data-stu-id="8eccd-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="8eccd-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8eccd-121">Authorization</span></span>  | <span data-ttu-id="8eccd-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8eccd-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="8eccd-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="8eccd-124">Content-Type</span></span>  | <span data-ttu-id="8eccd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8eccd-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="8eccd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8eccd-126">Request body</span></span>
<span data-ttu-id="8eccd-127">在请求正文中，提供 [educationCategory](../resources/educationcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8eccd-127">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="8eccd-128">响应</span><span class="sxs-lookup"><span data-stu-id="8eccd-128">Response</span></span>
<span data-ttu-id="8eccd-129">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationCategory](../resources/educationcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="8eccd-129">If successful, this method returns a `201 Created` response code and an [educationCategory](../resources/educationcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8eccd-130">示例</span><span class="sxs-lookup"><span data-stu-id="8eccd-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="8eccd-131">请求</span><span class="sxs-lookup"><span data-stu-id="8eccd-131">Request</span></span>
<span data-ttu-id="8eccd-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8eccd-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "sampleKeys": ["60eaa744-aa87-4276-b985-1633683119f8"],
  "name": "create_educationcategory_from_educationclass"
}-->
```http
POST https://graph.microsoft.com/v1.0/education/classes/60eaa744-aa87-4276-b985-1633683119f8/assignmentCategories/$entity
Content-type: application/json
Content-length: 33

{ 
  "displayName": "Quizzes"
}
```
<span data-ttu-id="8eccd-133">在请求正文中，提供 [educationCategory](../resources/educationcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8eccd-133">In the request body, supply a JSON representation of an [educationCategory](../resources/educationcategory.md) object.</span></span>

### <a name="response"></a><span data-ttu-id="8eccd-134">响应</span><span class="sxs-lookup"><span data-stu-id="8eccd-134">Response</span></span>
<span data-ttu-id="8eccd-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8eccd-135">The following is an example of the response.</span></span> 

><span data-ttu-id="8eccd-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8eccd-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationCategory"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 120

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#education/classes('60eaa744-aa87-4276-b985-1633683119f8')/assignmentCategories/$entity",
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


