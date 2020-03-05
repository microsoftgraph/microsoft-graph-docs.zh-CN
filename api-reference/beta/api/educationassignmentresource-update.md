---
title: 更新 educationAssignmentResource
description: '更新与工作分配相关联的资源的属性。 只有课堂中的教师才能更改工作分配资源对象。  '
author: dipakboyed
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: cb210affa5d98bdbc9a5cd012adc20a5c4ac49ea
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42427086"
---
# <a name="update-educationassignmentresource"></a><span data-ttu-id="0c2cd-104">更新 educationAssignmentResource</span><span class="sxs-lookup"><span data-stu-id="0c2cd-104">Update educationAssignmentResource</span></span>

<span data-ttu-id="0c2cd-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0c2cd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0c2cd-106">更新与工作分配相关联的资源的属性。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-106">Update the properties of resource associated with an assignment.</span></span> <span data-ttu-id="0c2cd-107">只有课堂中的教师才能更改工作分配资源对象。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-107">Only teachers in a class can change assignment resource objects.</span></span>  

## <a name="permissions"></a><span data-ttu-id="0c2cd-108">权限</span><span class="sxs-lookup"><span data-stu-id="0c2cd-108">Permissions</span></span>
<span data-ttu-id="0c2cd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c2cd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c2cd-111">Permission type</span></span>      | <span data-ttu-id="0c2cd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c2cd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-113">Delegated (work or school account)</span></span> |  <span data-ttu-id="0c2cd-114">EduAssignments、ReadWriteBasic、EduAssignments</span><span class="sxs-lookup"><span data-stu-id="0c2cd-114">EduAssignments.ReadWriteBasic, EduAssignments.ReadWrite</span></span>   |
|<span data-ttu-id="0c2cd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c2cd-115">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="0c2cd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-116">Not supported.</span></span>  |
|<span data-ttu-id="0c2cd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c2cd-117">Application</span></span> | <span data-ttu-id="0c2cd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-118">Not supported.</span></span> | 

## <a name="http-request"></a><span data-ttu-id="0c2cd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c2cd-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/classes/{id}/assignments/{id}/resources/{id}
```
## <a name="request-headers"></a><span data-ttu-id="0c2cd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c2cd-120">Request headers</span></span>
| <span data-ttu-id="0c2cd-121">标头</span><span class="sxs-lookup"><span data-stu-id="0c2cd-121">Header</span></span>       | <span data-ttu-id="0c2cd-122">值</span><span class="sxs-lookup"><span data-stu-id="0c2cd-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c2cd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c2cd-123">Authorization</span></span>  | <span data-ttu-id="0c2cd-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c2cd-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0c2cd-126">Content-Type</span></span>  | <span data-ttu-id="0c2cd-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0c2cd-127">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0c2cd-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c2cd-128">Request body</span></span>
<span data-ttu-id="0c2cd-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="0c2cd-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0c2cd-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0c2cd-132">属性</span><span class="sxs-lookup"><span data-stu-id="0c2cd-132">Property</span></span>     | <span data-ttu-id="0c2cd-133">类型</span><span class="sxs-lookup"><span data-stu-id="0c2cd-133">Type</span></span>   |<span data-ttu-id="0c2cd-134">说明</span><span class="sxs-lookup"><span data-stu-id="0c2cd-134">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0c2cd-135">distributeForStudentWork</span><span class="sxs-lookup"><span data-stu-id="0c2cd-135">distributeForStudentWork</span></span>|<span data-ttu-id="0c2cd-136">布尔</span><span class="sxs-lookup"><span data-stu-id="0c2cd-136">Boolean</span></span>| <span data-ttu-id="0c2cd-137">指示在发布工作分配时是否应将此资源复制到每个学生的资源对象。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-137">Indicates whether this resource should be copied to each student's resource object when the assignment is published.</span></span>|
|<span data-ttu-id="0c2cd-138">resource</span><span class="sxs-lookup"><span data-stu-id="0c2cd-138">resource</span></span>|<span data-ttu-id="0c2cd-139">educationResource</span><span class="sxs-lookup"><span data-stu-id="0c2cd-139">educationResource</span></span>| <span data-ttu-id="0c2cd-140">Resource 对象。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-140">Resource object.</span></span> |

## <a name="response"></a><span data-ttu-id="0c2cd-141">响应</span><span class="sxs-lookup"><span data-stu-id="0c2cd-141">Response</span></span>
<span data-ttu-id="0c2cd-142">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[educationAssignmentResource](../resources/educationassignmentresource.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-142">If successful, this method returns a `200 OK` response code and an updated [educationAssignmentResource](../resources/educationassignmentresource.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0c2cd-143">示例</span><span class="sxs-lookup"><span data-stu-id="0c2cd-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0c2cd-144">请求</span><span class="sxs-lookup"><span data-stu-id="0c2cd-144">Request</span></span>
<span data-ttu-id="0c2cd-145">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-145">The following is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="0c2cd-146">响应</span><span class="sxs-lookup"><span data-stu-id="0c2cd-146">Response</span></span>
<span data-ttu-id="0c2cd-147">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-147">The following is an example of the response.</span></span> 

><span data-ttu-id="0c2cd-148">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-148">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="0c2cd-149">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c2cd-149">All of the properties will be returned from an actual call.</span></span>


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
  "suppressions": []
}
-->
