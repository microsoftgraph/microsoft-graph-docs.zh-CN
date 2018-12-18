---
title: 创建 educationSubmissionResource
description: '将资源添加到资源列表中。 此操作仅可通过学生为其分配此提交。 此操作不会成功，如果未设置**allowStudentsToAddResources**标志，则为 true。 如果呼叫者想要创建新的基于文件的资源，该文件必须上载到提交与关联的资源文件夹中。 如果文件不存在或不在该文件夹中，在 POST 请求将失败。 '
author: dipakboyed
ms.openlocfilehash: 71d06e996213c133ed9c48d5d3e320a785e122ae
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27321299"
---
# <a name="create-educationsubmissionresource"></a><span data-ttu-id="bfdd9-107">创建 educationSubmissionResource</span><span class="sxs-lookup"><span data-stu-id="bfdd9-107">Create educationSubmissionResource</span></span>

> <span data-ttu-id="bfdd9-108">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-108">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bfdd9-109">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-109">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bfdd9-110">将资源添加到资源列表中。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-110">Adds a resource to the resources list.</span></span> <span data-ttu-id="bfdd9-111">此操作仅可通过学生为其分配此提交。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-111">This action can only be done by the student to whom this submission is assigned.</span></span> <span data-ttu-id="bfdd9-112">此操作不会成功，如果未设置**allowStudentsToAddResources**标志，则为 true。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-112">This action will not succeed if the **allowStudentsToAddResources** flag is not set to true.</span></span> <span data-ttu-id="bfdd9-113">如果呼叫者想要创建新的基于文件的资源，该文件必须上载到提交与关联的资源文件夹中。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-113">If the caller wants to create a new file-based resource, the file must be uploaded to the resources folder that is associated with the submission.</span></span> <span data-ttu-id="bfdd9-114">如果文件不存在或不在该文件夹中，在 POST 请求将失败。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-114">If the file does not exist or is not in that folder, the POST request will fail.</span></span> 

## <a name="permissions"></a><span data-ttu-id="bfdd9-115">权限</span><span class="sxs-lookup"><span data-stu-id="bfdd9-115">Permissions</span></span>
<span data-ttu-id="bfdd9-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bfdd9-118">权限类型</span><span class="sxs-lookup"><span data-stu-id="bfdd9-118">Permission type</span></span>      | <span data-ttu-id="bfdd9-119">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bfdd9-119">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bfdd9-120">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bfdd9-120">Delegated (work or school account)</span></span> |  <span data-ttu-id="bfdd9-121">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="bfdd9-121">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>  |
|<span data-ttu-id="bfdd9-122">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bfdd9-122">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bfdd9-123">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-123">Not supported.</span></span>  |
|<span data-ttu-id="bfdd9-124">应用程序</span><span class="sxs-lookup"><span data-stu-id="bfdd9-124">Application</span></span> | <span data-ttu-id="bfdd9-125">不支持。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-125">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="bfdd9-126">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bfdd9-126">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /education/classes/{id}/assignments/{id}/submissions/{id}/resources

```
## <a name="request-headers"></a><span data-ttu-id="bfdd9-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="bfdd9-127">Request headers</span></span>
| <span data-ttu-id="bfdd9-128">标头</span><span class="sxs-lookup"><span data-stu-id="bfdd9-128">Header</span></span>       | <span data-ttu-id="bfdd9-129">值</span><span class="sxs-lookup"><span data-stu-id="bfdd9-129">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bfdd9-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="bfdd9-130">Authorization</span></span>  | <span data-ttu-id="bfdd9-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bfdd9-133">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bfdd9-133">Content-Type</span></span>  | <span data-ttu-id="bfdd9-134">application/json</span><span class="sxs-lookup"><span data-stu-id="bfdd9-134">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="bfdd9-135">请求正文</span><span class="sxs-lookup"><span data-stu-id="bfdd9-135">Request body</span></span>
<span data-ttu-id="bfdd9-136">在请求正文中，提供[educationSubmissionResource](../resources/educationsubmissionresource.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-136">In the request body, supply a JSON representation of the [educationSubmissionResource](../resources/educationsubmissionresource.md) object.</span></span>


## <a name="response"></a><span data-ttu-id="bfdd9-137">响应</span><span class="sxs-lookup"><span data-stu-id="bfdd9-137">Response</span></span>
<span data-ttu-id="bfdd9-138">如果成功，此方法返回`201 Created`响应代码和响应正文中的[educationSubmissionResource](../resources/educationsubmissionresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-138">If successful, this method returns a `201 Created` response code and an [educationSubmissionResource](../resources/educationsubmissionresource.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bfdd9-139">示例</span><span class="sxs-lookup"><span data-stu-id="bfdd9-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="bfdd9-140">请求</span><span class="sxs-lookup"><span data-stu-id="bfdd9-140">Request</span></span>
<span data-ttu-id="bfdd9-141">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-141">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "create_educationsubmissionresource_from_educationsubmission"
}-->
```
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

##### <a name="response"></a><span data-ttu-id="bfdd9-142">响应</span><span class="sxs-lookup"><span data-stu-id="bfdd9-142">Response</span></span>
<span data-ttu-id="bfdd9-143">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-143">The following is an example of the response.</span></span> 

><span data-ttu-id="bfdd9-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bfdd9-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Create educationSubmissionResource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->