---
title: 更新 educationAssignmentResource
description: '更新与工作分配相关联的资源的属性。 只有课堂中的教师才能更改工作分配资源对象。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 34b1c05937f57fe46d5d854d21a7c2e0b68240d2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32457954"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="38359-104">更新 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="38359-104">Update educationAssignmentResource</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="38359-105">更新与工作分配相关联的资源的属性。</span><span class="sxs-lookup"><span data-stu-id="38359-105">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="38359-106">只有课堂中的教师才能更改工作分配资源对象。</span><span class="sxs-lookup"><span data-stu-id="38359-106">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="38359-107">权限</span><span class="sxs-lookup"><span data-stu-id="38359-107">Permissions</span></span>
<span data-ttu-id="38359-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="38359-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="38359-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="38359-110">Permission type</span></span>      | <span data-ttu-id="38359-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="38359-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="38359-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="38359-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="38359-113">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="38359-113">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="38359-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="38359-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="38359-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="38359-115">Not supported.</span></span>  |
|<span data-ttu-id="38359-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="38359-116">Application</span></span> | <span data-ttu-id="38359-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="38359-117">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="38359-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="38359-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="38359-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="38359-119">Request headers</span></span>
| <span data-ttu-id="38359-120">标头</span><span class="sxs-lookup"><span data-stu-id="38359-120">Header</span></span>       | <span data-ttu-id="38359-121">值</span><span class="sxs-lookup"><span data-stu-id="38359-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="38359-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="38359-122">Authorization</span></span>  | <span data-ttu-id="38359-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="38359-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="38359-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="38359-125">Content-Type</span></span>  | <span data-ttu-id="38359-126">application/json</span><span class="sxs-lookup"><span data-stu-id="38359-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="38359-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="38359-127">Request body</span></span>
<span data-ttu-id="38359-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="38359-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="38359-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="38359-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="38359-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="38359-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="38359-131">属性</span><span class="sxs-lookup"><span data-stu-id="38359-131">Property</span></span>     | <span data-ttu-id="38359-132">类型</span><span class="sxs-lookup"><span data-stu-id="38359-132">Type</span></span>   |<span data-ttu-id="38359-133">说明</span><span class="sxs-lookup"><span data-stu-id="38359-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="38359-134">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="38359-134">distributeForStudentWork</span></span>|<span data-ttu-id="38359-135">布尔</span><span class="sxs-lookup"><span data-stu-id="38359-135">Boolean</span></span>| <span data-ttu-id="38359-136">指示在发布工作分配时是否应将此资源复制到每个学生的资源对象。</span><span class="sxs-lookup"><span data-stu-id="38359-136">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="38359-137">资源</span><span class="sxs-lookup"><span data-stu-id="38359-137">resource</span></span>|<span data-ttu-id="38359-138">educationResource</span><span class="sxs-lookup"><span data-stu-id="38359-138">educationResource</span></span>| <span data-ttu-id="38359-139">Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="38359-139">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="38359-140">响应</span><span class="sxs-lookup"><span data-stu-id="38359-140">Response</span></span>
<span data-ttu-id="38359-141">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="38359-141">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="38359-142">示例</span><span class="sxs-lookup"><span data-stu-id="38359-142">Example</span></span>
##### <a name="request"></a><span data-ttu-id="38359-143">请求</span><span class="sxs-lookup"><span data-stu-id="38359-143">Request</span></span>
<span data-ttu-id="38359-144">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="38359-144">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="38359-145">响应</span><span class="sxs-lookup"><span data-stu-id="38359-145">Response</span></span>
<span data-ttu-id="38359-146">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="38359-146">The following is an example of the response.</span></span> 

><span data-ttu-id="38359-147">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="38359-147">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="38359-148">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="38359-148">All of the properties will be returned from an actual call.</span></span>


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
