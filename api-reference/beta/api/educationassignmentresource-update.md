---
title: 更新 educationAssignmentResource
description: '更新资源分配相关联的属性。 仅在类的教师可以更改工作分配的资源对象。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 34b1c05937f57fe46d5d854d21a7c2e0b68240d2
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29527953"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="b4172-104">更新 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="b4172-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b4172-105">更新资源分配相关联的属性。</span><span class="sxs-lookup"><span data-stu-id="b4172-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="b4172-106">仅在类的教师可以更改工作分配的资源对象。</span><span class="sxs-lookup"><span data-stu-id="b4172-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="b4172-107">权限</span><span class="sxs-lookup"><span data-stu-id="b4172-107">Permissions</span></span>
<span data-ttu-id="b4172-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4172-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4172-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4172-110">Permission type</span></span>      | <span data-ttu-id="b4172-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b4172-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b4172-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4172-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="b4172-113">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b4172-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="b4172-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4172-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="b4172-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4172-115">Not supported.</span></span>  |
|<span data-ttu-id="b4172-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4172-116">Application</span></span> | <span data-ttu-id="b4172-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4172-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="b4172-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4172-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="b4172-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4172-119">Request headers</span></span>
| <span data-ttu-id="b4172-120">标头</span><span class="sxs-lookup"><span data-stu-id="b4172-120">Header</span></span>       | <span data-ttu-id="b4172-121">值</span><span class="sxs-lookup"><span data-stu-id="b4172-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="b4172-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4172-122">Authorization</span></span>  | <span data-ttu-id="b4172-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b4172-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b4172-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b4172-125">Content-Type</span></span>  | <span data-ttu-id="b4172-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4172-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="b4172-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4172-127">Request body</span></span>
<span data-ttu-id="b4172-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b4172-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b4172-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b4172-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b4172-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b4172-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b4172-131">属性</span><span class="sxs-lookup"><span data-stu-id="b4172-131">Property</span></span>     | <span data-ttu-id="b4172-132">类型</span><span class="sxs-lookup"><span data-stu-id="b4172-132">Type</span></span>   |<span data-ttu-id="b4172-133">说明</span><span class="sxs-lookup"><span data-stu-id="b4172-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b4172-134">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="b4172-134">distributeForStudentWork</span></span>|<span data-ttu-id="b4172-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="b4172-135">Boolean</span></span>| <span data-ttu-id="b4172-136">指示工作分配发布时是否应将此资源复制到每个学生的资源对象。</span><span class="sxs-lookup"><span data-stu-id="b4172-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="b4172-137">资源</span><span class="sxs-lookup"><span data-stu-id="b4172-137">resource</span></span>|<span data-ttu-id="b4172-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="b4172-138">educationResource</span></span>| <span data-ttu-id="b4172-139">Resource 对象</span><span class="sxs-lookup"><span data-stu-id="b4172-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="b4172-140">响应</span><span class="sxs-lookup"><span data-stu-id="b4172-140">Response</span></span>
<span data-ttu-id="b4172-141">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b4172-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="b4172-142">示例</span><span class="sxs-lookup"><span data-stu-id="b4172-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="b4172-143">请求</span><span class="sxs-lookup"><span data-stu-id="b4172-143">Request</span></span>
<span data-ttu-id="b4172-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b4172-144">The following is an example of the request.</span></span>
<!-- {
  "blockType": "ignored",
  "name": "update_educationassignmentresource"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/classes/11021/assignments/19002/resources/850f51b7-1df9-4ec0-bd62-64a0214b9cbf
Content-type: application/json
Content-length: 822

{
  "distributeForStudentWork": "false"
}
```
##### <a name="response"></a><span data-ttu-id="b4172-145">响应</span><span class="sxs-lookup"><span data-stu-id="b4172-145">Response</span></span>
<span data-ttu-id="b4172-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b4172-146">The following is an example of the response.</span></span> 

><span data-ttu-id="b4172-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b4172-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b4172-148">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4172-148">All of the properties will be returned from an actual call.</span></span>


<!-- {
  "blockType": "ignored",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationAssignmentResource"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 832

{
  "distributeForStudentWork": false,
  "resource": {
      "@odata.type": "#microsoft.graph.educationLinkResource",
      "displayName": "Microsoft Homepage",
      "createdDateTime": "2017-10-21T07:52:45.5675913Z",
      "createdBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "lastModifiedDateTime": "2017-10-21T07:52:45.5675913Z",
      "lastModifiedBy": {
          "application": null,
          "device": null,
          "user": {
              "id": "63cc91d2-59c7-4732-9594-35b91a26b340",
              "displayName": null
          }
      },
      "link": "https://www.microsoft.com"
  },
  "id": "850f51b7-1df9-4ec0-bd62-64a0214b9cbf"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/educationassignmentresource-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
