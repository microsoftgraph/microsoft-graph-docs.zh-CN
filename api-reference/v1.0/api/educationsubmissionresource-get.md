---
title: 获取 educationSubmissionResource
description: 检索与提交关联的特定资源的属性。
author: sharad-sharma-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 086f6c965252b528377feaabbd06ad2110c67139
ms.sourcegitcommit: f77c1385306fd40557aceb24fdfe4832cbb60a27
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/12/2021
ms.locfileid: "52912258"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="98870-103">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="98870-103">Get educationSubmissionResource</span></span>

<span data-ttu-id="98870-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="98870-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="98870-105">检索与提交关联的特定资源 [的属性](../resources/educationsubmissionresource.md)。</span><span class="sxs-lookup"><span data-stu-id="98870-105">Retrieve the properties of a specific resource associated with a [submission](../resources/educationsubmissionresource.md).</span></span> 

<span data-ttu-id="98870-106">此资源位于"工作"资源列表中，应视为学生正在处理的工作。</span><span class="sxs-lookup"><span data-stu-id="98870-106">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="98870-107">如果此资源是从工作分配复制的，则用可能的指针将资源打包回工作分配资源。</span><span class="sxs-lookup"><span data-stu-id="98870-107">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="98870-108">权限</span><span class="sxs-lookup"><span data-stu-id="98870-108">Permissions</span></span>
<span data-ttu-id="98870-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="98870-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="98870-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="98870-111">Permission type</span></span>      | <span data-ttu-id="98870-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="98870-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="98870-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="98870-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="98870-114">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98870-114">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="98870-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="98870-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="98870-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="98870-116">Not supported.</span></span>  |
|<span data-ttu-id="98870-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="98870-117">Application</span></span> | <span data-ttu-id="98870-118">EduAssignments.ReadBasic、EduAssignments.ReadWriteBasic、EduAssignments.Read、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="98870-118">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span> | 

## <a name="http-request"></a><span data-ttu-id="98870-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="98870-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/cf6005fc-9e13-44a2-a6ac-a53322006454/submissions/d1bee293-d8bb-48d4-af3e-c8cb0e3c7fe7/resources/8b01c1d0-aafc-4f8c-bd73-89faa3df1c1c
```
## <a name="optional-query-parameters"></a><span data-ttu-id="98870-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="98870-120">Optional query parameters</span></span>
<span data-ttu-id="98870-121">此方法支持使用 [OData 查询参数](/graph/query-parameters)来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="98870-121">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="98870-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="98870-122">Request headers</span></span>
| <span data-ttu-id="98870-123">标头</span><span class="sxs-lookup"><span data-stu-id="98870-123">Header</span></span>       | <span data-ttu-id="98870-124">值</span><span class="sxs-lookup"><span data-stu-id="98870-124">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="98870-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="98870-125">Authorization</span></span>  | <span data-ttu-id="98870-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="98870-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="98870-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="98870-128">Request body</span></span>
<span data-ttu-id="98870-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="98870-129">Don't supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="98870-130">响应</span><span class="sxs-lookup"><span data-stu-id="98870-130">Response</span></span>
<span data-ttu-id="98870-131">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="98870-131">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="98870-132">示例</span><span class="sxs-lookup"><span data-stu-id="98870-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="98870-133">请求</span><span class="sxs-lookup"><span data-stu-id="98870-133">Request</span></span>
<span data-ttu-id="98870-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="98870-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_educationsubmissionresource"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/education/classes/acdefc6b-2dc6-4e71-b1e9-6d9810ab1793/assignments/ad8afb28-c138-4ad7-b7f5-a6986c2655a8/submissions/fbe51c90-78b7-418a-b5f3-871bf8d8d21e/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```

### <a name="response"></a><span data-ttu-id="98870-135">响应</span><span class="sxs-lookup"><span data-stu-id="98870-135">Response</span></span>
<span data-ttu-id="98870-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="98870-136">The following is an example of the response.</span></span> 

><span data-ttu-id="98870-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="98870-137">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1152

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
  "id": "f2387c3b-ec39-4bf2-a399-d7242677f024",
  "resource": {
      "@odata.type": "#microsoft.graph.educationWordResource",
      "displayName": "Report.docx",
      "createdDateTime": "2017-10-21T07:52:53.9863696Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:53.9863696Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
