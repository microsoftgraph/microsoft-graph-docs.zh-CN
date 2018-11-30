---
title: 更新 educationAssignmentResource
description: '更新资源分配相关联的属性。 仅在类的教师可以更改工作分配的资源对象。  '
ms.openlocfilehash: 761dc4f656a41d8d984443b17d87b1b0961a2a8b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042360"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="160c7-104">更新 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="160c7-104">Update educationAssignmentResource</span></span>

> <span data-ttu-id="160c7-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="160c7-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="160c7-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="160c7-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="160c7-107">更新资源分配相关联的属性。</span><span class="sxs-lookup"><span data-stu-id="160c7-107">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="160c7-108">仅在类的教师可以更改工作分配的资源对象。</span><span class="sxs-lookup"><span data-stu-id="160c7-108">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="160c7-109">权限</span><span class="sxs-lookup"><span data-stu-id="160c7-109">Permissions</span></span>
<span data-ttu-id="160c7-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="160c7-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="160c7-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="160c7-112">Permission type</span></span>      | <span data-ttu-id="160c7-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="160c7-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="160c7-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="160c7-114">Delegated (work or school account)</span></span> |  <span data-ttu-id="160c7-115">EduAssignments.ReadWriteBasic EduAssignments.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="160c7-115">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="160c7-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="160c7-116">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="160c7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="160c7-117">Not supported.</span></span>  |
|<span data-ttu-id="160c7-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="160c7-118">Application</span></span> | <span data-ttu-id="160c7-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="160c7-119">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="160c7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="160c7-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="160c7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="160c7-121">Request headers</span></span>
| <span data-ttu-id="160c7-122">标头</span><span class="sxs-lookup"><span data-stu-id="160c7-122">Header</span></span>       | <span data-ttu-id="160c7-123">值</span><span class="sxs-lookup"><span data-stu-id="160c7-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="160c7-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="160c7-124">Authorization</span></span>  | <span data-ttu-id="160c7-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="160c7-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="160c7-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="160c7-127">Content-Type</span></span>  | <span data-ttu-id="160c7-128">application/json</span><span class="sxs-lookup"><span data-stu-id="160c7-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="160c7-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="160c7-129">Request body</span></span>
<span data-ttu-id="160c7-130">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="160c7-130">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="160c7-131">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="160c7-131">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="160c7-132">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="160c7-132">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="160c7-133">属性</span><span class="sxs-lookup"><span data-stu-id="160c7-133">Property</span></span>     | <span data-ttu-id="160c7-134">类型</span><span class="sxs-lookup"><span data-stu-id="160c7-134">Type</span></span>   |<span data-ttu-id="160c7-135">说明</span><span class="sxs-lookup"><span data-stu-id="160c7-135">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="160c7-136">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="160c7-136">distributeForStudentWork</span></span>|<span data-ttu-id="160c7-137">布尔</span><span class="sxs-lookup"><span data-stu-id="160c7-137">Boolean</span></span>| <span data-ttu-id="160c7-138">指示工作分配发布时是否应将此资源复制到每个学生的资源对象。</span><span class="sxs-lookup"><span data-stu-id="160c7-138">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="160c7-139">resource</span><span class="sxs-lookup"><span data-stu-id="160c7-139">resource</span></span>|<span data-ttu-id="160c7-140">educationResource</span><span class="sxs-lookup"><span data-stu-id="160c7-140">educationResource</span></span>| <span data-ttu-id="160c7-141">资源对象。</span><span class="sxs-lookup"><span data-stu-id="160c7-141">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="160c7-142">响应</span><span class="sxs-lookup"><span data-stu-id="160c7-142">Response</span></span>
<span data-ttu-id="160c7-143">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="160c7-143">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="160c7-144">示例</span><span class="sxs-lookup"><span data-stu-id="160c7-144">Example</span></span>
##### <a name="request"></a><span data-ttu-id="160c7-145">请求</span><span class="sxs-lookup"><span data-stu-id="160c7-145">Request</span></span>
<span data-ttu-id="160c7-146">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="160c7-146">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="160c7-147">响应</span><span class="sxs-lookup"><span data-stu-id="160c7-147">Response</span></span>
<span data-ttu-id="160c7-148">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="160c7-148">The following is an example of the response.</span></span> 

><span data-ttu-id="160c7-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="160c7-149">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="160c7-150">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="160c7-150">All of the properties will be returned from an actual call.</span></span>


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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationassignmentresource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
