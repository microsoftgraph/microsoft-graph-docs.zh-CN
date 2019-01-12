---
title: 获取 educationSubmissionResource
description: 检索特定资源提交相关联的属性。 此资源是工作中资源列表中，应考虑工作进程中的由一个学生。 如果它已从分配复制回工作分配资源的可能指针与包装此资源。
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 47dd803e4a8503017d68f00c0e95c78ad271c870
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27940349"
---
# <a name="get-educationsubmissionresource"></a><span data-ttu-id="a7e93-105">获取 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="a7e93-105">Get educationSubmissionResource</span></span>

> <span data-ttu-id="a7e93-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a7e93-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7e93-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a7e93-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a7e93-108">检索特定资源提交相关联的属性。</span><span class="sxs-lookup"><span data-stu-id="a7e93-108">Retrieves the properties of a specific resource associated with the submission.</span></span> <span data-ttu-id="a7e93-109">此资源是"工作"资源列表中，应考虑工作进程中的由一个学生。</span><span class="sxs-lookup"><span data-stu-id="a7e93-109">This resource is in the "working" resource list and should be considered work in process by a student.</span></span> <span data-ttu-id="a7e93-110">如果它已从分配复制回工作分配资源的可能指针与包装此资源。</span><span class="sxs-lookup"><span data-stu-id="a7e93-110">This resource is wrapped with a possible pointer back to the assignment resource if it was copied from the assignment.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7e93-111">权限</span><span class="sxs-lookup"><span data-stu-id="a7e93-111">Permissions</span></span>
<span data-ttu-id="a7e93-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7e93-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7e93-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7e93-114">Permission type</span></span>      | <span data-ttu-id="a7e93-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7e93-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a7e93-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7e93-116">Delegated (work or school account)</span></span> |  <span data-ttu-id="a7e93-117">EduAssignments.ReadBasic，EduAssignments.ReadWriteBasic，EduAssignments.Read EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="a7e93-117">EduAssignments.ReadBasic, EduAssignments.ReadWriteBasic, EduAssignments.Read, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="a7e93-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7e93-118">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a7e93-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7e93-119">Not supported.</span></span>  |
|<span data-ttu-id="a7e93-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="a7e93-120">Application</span></span> | <span data-ttu-id="a7e93-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7e93-121">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="a7e93-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7e93-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /education/classes/{id}/assignments/{id}/submissions/{id}/resources/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="a7e93-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a7e93-123">Optional query parameters</span></span>
<span data-ttu-id="a7e93-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a7e93-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a7e93-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7e93-125">Request headers</span></span>
| <span data-ttu-id="a7e93-126">标头</span><span class="sxs-lookup"><span data-stu-id="a7e93-126">Header</span></span>       | <span data-ttu-id="a7e93-127">值</span><span class="sxs-lookup"><span data-stu-id="a7e93-127">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a7e93-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7e93-128">Authorization</span></span>  | <span data-ttu-id="a7e93-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7e93-p105">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a7e93-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7e93-131">Request body</span></span>
<span data-ttu-id="a7e93-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a7e93-132">Do not supply a request body for this method.</span></span>
## <a name="response"></a><span data-ttu-id="a7e93-133">响应</span><span class="sxs-lookup"><span data-stu-id="a7e93-133">Response</span></span>
<span data-ttu-id="a7e93-134">如果成功，此方法返回`200 OK`响应代码和响应正文中的[educationSubmissionResource](../resources/educationsubmissionresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a7e93-134">If successful, this method returns a `200 OK` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7e93-135">示例</span><span class="sxs-lookup"><span data-stu-id="a7e93-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7e93-136">请求</span><span class="sxs-lookup"><span data-stu-id="a7e93-136">Request</span></span>
<span data-ttu-id="a7e93-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a7e93-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "get_educationsubmissionresource"
}-->
```http 
GET https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources/f2387c3b-ec39-4bf2-a399-d7242677f024
```
##### <a name="response"></a><span data-ttu-id="a7e93-138">响应</span><span class="sxs-lookup"><span data-stu-id="a7e93-138">Response</span></span>
<span data-ttu-id="a7e93-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a7e93-139">The following is an example of the response.</span></span> 

><span data-ttu-id="a7e93-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a7e93-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "ignored",
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
<!-- {
  "type": "#page.annotation",
  "description": "Get educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
