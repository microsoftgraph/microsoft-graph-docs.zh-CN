---
title: 创建 educationSubmissionResource
description: '将资源添加到资源列表。 此操作仅能由分配了此提交的学生执行。 如果未将 **allowStudentsToAddResources** 标志设置为 true，此操作将不会成功。 如果调用方想要创建新的基于文件的资源，则必须将该文件上载到与提交关联的资源文件夹。 如果文件不存在或不在该文件夹中，POST 请求将失败。 '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 24363b7158ccfad72db22158d25298fdb75d040d
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52664760"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="55271-107">创建 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="55271-107">Create educationSubmissionResource</span></span>

<span data-ttu-id="55271-108">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="55271-108">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="55271-109">将资源添加到资源列表。</span><span class="sxs-lookup"><span data-stu-id="55271-109">Adds a resource to the resources list.</span></span> <span data-ttu-id="55271-110">此操作仅能由分配了此提交的学生执行。</span><span class="sxs-lookup"><span data-stu-id="55271-110">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="55271-111">如果未将 **allowStudentsToAddResources** 标志设置为 true，此操作将不会成功。</span><span class="sxs-lookup"><span data-stu-id="55271-111">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="55271-112">如果调用方想要创建新的基于文件的资源，则必须将该文件上载到与提交关联的资源文件夹。</span><span class="sxs-lookup"><span data-stu-id="55271-112">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="55271-113">如果文件不存在或不在该文件夹中，POST 请求将失败。</span><span class="sxs-lookup"><span data-stu-id="55271-113">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="55271-114">权限</span><span class="sxs-lookup"><span data-stu-id="55271-114">Permissions</span></span>
<span data-ttu-id="55271-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="55271-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55271-117">权限类型</span><span class="sxs-lookup"><span data-stu-id="55271-117">Permission type</span></span>      | <span data-ttu-id="55271-118">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="55271-118">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="55271-119">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="55271-119">Delegated (work or school account)</span></span> |  <span data-ttu-id="55271-120">EduAssignments.ReadWriteBasic、EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="55271-120">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="55271-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="55271-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="55271-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="55271-122">Not supported.</span></span>  |
|<span data-ttu-id="55271-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="55271-123">Application</span></span> | <span data-ttu-id="55271-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="55271-124">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="55271-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="55271-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources
```

## <a name="request-headers"></a><span data-ttu-id="55271-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="55271-126">Request headers</span></span>
| <span data-ttu-id="55271-127">标头</span><span class="sxs-lookup"><span data-stu-id="55271-127">Header</span></span>       | <span data-ttu-id="55271-128">值</span><span class="sxs-lookup"><span data-stu-id="55271-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="55271-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="55271-129">Authorization</span></span>  | <span data-ttu-id="55271-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="55271-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="55271-132">Content-Type</span><span class="sxs-lookup"><span data-stu-id="55271-132">Content-Type</span></span>  | <span data-ttu-id="55271-133">application/json</span><span class="sxs-lookup"><span data-stu-id="55271-133">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="55271-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="55271-134">Request body</span></span>
<span data-ttu-id="55271-135">在请求正文中，提供 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="55271-135">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="55271-136">响应</span><span class="sxs-lookup"><span data-stu-id="55271-136">Response</span></span>
<span data-ttu-id="55271-137">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [educationSubmissionResource](../resources/educationsubmissionresource.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="55271-137">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="55271-138">示例</span><span class="sxs-lookup"><span data-stu-id="55271-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="55271-139">请求</span><span class="sxs-lookup"><span data-stu-id="55271-139">Request</span></span>
<span data-ttu-id="55271-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="55271-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```http
POST https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/submissions/850f51b7/resources
Content-type: application/json
Content-length: 1097

{
  "assignmentResourceUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeT456457AdW9f/items/017NJZI25NOB5XZNLABF7646XAMDZTQQ6T",
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
  },
  "@odata.type": "microsoft.graph.educationResource"
}
```

##### <a name="response"></a><span data-ttu-id="55271-141">响应</span><span class="sxs-lookup"><span data-stu-id="55271-141">Response</span></span>
<span data-ttu-id="55271-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="55271-142">The following is an example of the response.</span></span> 

><span data-ttu-id="55271-143">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="55271-143">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSubmissionResource"
} -->
```http
HTTP/1.1 201 Created
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
      "fileUrl": "https://graph.microsoft.com/v1.0/drives/b!8-QjN2tsv0WyGnTv7vOvnQkmGHbbeMNLqYKONmHLVnvCVmBYIGpeTZ_iul5AdW9f/items/017NJZI27BCN2QI2H7HJGLIVPXR6SD2DH6",
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


