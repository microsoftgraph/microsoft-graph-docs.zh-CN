---
title: 列表提交
description: 列出与此工作分配相关联的所有提交。 教师可以获取所有提交，而学生只能获取与之关联的提交。
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 4effa4f3e6bf9d708acd9a2a4d03eaae573642c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48007775"
---
# <a name="list-submissions"></a><span data-ttu-id="c401f-104">列表提交</span><span class="sxs-lookup"><span data-stu-id="c401f-104">List submissions</span></span>

<span data-ttu-id="c401f-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c401f-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c401f-106">列出与此工作分配相关联的所有提交。</span><span class="sxs-lookup"><span data-stu-id="c401f-106">List all the submissions associated with this assignment.</span></span> <span data-ttu-id="c401f-107">教师可以获取所有提交，而学生只能获取与之关联的提交。</span><span class="sxs-lookup"><span data-stu-id="c401f-107">A teacher can get all the submissions while a student can only get submissions that they are associated with.</span></span>

## <a name="permissions"></a><span data-ttu-id="c401f-108">权限</span><span class="sxs-lookup"><span data-stu-id="c401f-108">Permissions</span></span>
<span data-ttu-id="c401f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c401f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c401f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c401f-111">Permission type</span></span>      | <span data-ttu-id="c401f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c401f-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c401f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c401f-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="c401f-114">EduAssignments、EduAssignments、EduAssignments、Read、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="c401f-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="c401f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c401f-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c401f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c401f-116">Not supported.</span></span>  |
|<span data-ttu-id="c401f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c401f-117">Application</span></span> | <span data-ttu-id="c401f-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c401f-118">Not Supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="c401f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c401f-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions
```
## <a name="optional-query-parameters"></a><span data-ttu-id="c401f-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c401f-120">Optional query parameters</span></span>
<span data-ttu-id="c401f-121">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c401f-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c401f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="c401f-122">Request headers</span></span>
| <span data-ttu-id="c401f-123">标头</span><span class="sxs-lookup"><span data-stu-id="c401f-123">Header</span></span>       | <span data-ttu-id="c401f-124">值</span><span class="sxs-lookup"><span data-stu-id="c401f-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c401f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="c401f-125">Authorization</span></span>  | <span data-ttu-id="c401f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c401f-p104">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c401f-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c401f-128">Request body</span></span>
<span data-ttu-id="c401f-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c401f-129">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="c401f-130">响应</span><span class="sxs-lookup"><span data-stu-id="c401f-130">Response</span></span>
<span data-ttu-id="c401f-131">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [educationSubmission](../resources/educationsubmission.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c401f-131">If successful, this method returns a `200 OK` response code and collection of [educationSubmission](../resources/educationsubmission.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c401f-132">示例</span><span class="sxs-lookup"><span data-stu-id="c401f-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c401f-133">请求</span><span class="sxs-lookup"><span data-stu-id="c401f-133">Request</span></span>
<span data-ttu-id="c401f-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c401f-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_submissions"
}-->
```http
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions
```
##### <a name="response"></a><span data-ttu-id="c401f-135">响应</span><span class="sxs-lookup"><span data-stu-id="c401f-135">Response</span></span>
<span data-ttu-id="c401f-136">下面介绍响应示例。</span><span class="sxs-lookup"><span data-stu-id="c401f-136">The following is an example of the response.</span></span> 

><span data-ttu-id="c401f-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c401f-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c401f-138">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c401f-138">All of the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmission",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 873

{
  "value": [
    {
      "id": "33223",
      "recipient": {
        "userId": "13015",
        "@Odata.type":"microsoft.graph.educationSubmissionRecipient"
      },
      "releasedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "releasedDateTime": "2014-01-01T00:00:00Z",
      "resourcesFolderUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
      "status": "working",
      "submittedBy": {
          "user": {
            "displayName": "Susana Rocha",
            "id": "14012"
          },
        },
      "submittedDateTime": "2014-01-01T00:00:00Z"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List submissions",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


