---
title: 更新 educationschool 属性
description: 更新 school 对象的属性。
author: mmast-msft
localization_priority: Normal
ms.openlocfilehash: 23c7c476e2447fbde43a0e7521d4b3d626f80f5b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892230"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="c21c4-103">更新 educationschool 属性</span><span class="sxs-lookup"><span data-stu-id="c21c4-103">Update educationschool properties</span></span>

> <span data-ttu-id="c21c4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c21c4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c21c4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c21c4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c21c4-106">更新 school 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c21c4-106">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c21c4-107">权限</span><span class="sxs-lookup"><span data-stu-id="c21c4-107">Permissions</span></span>
<span data-ttu-id="c21c4-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c21c4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c21c4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c21c4-110">Permission type</span></span>      | <span data-ttu-id="c21c4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c21c4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c21c4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c21c4-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="c21c4-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c21c4-113">Not supported.</span></span>  |
|<span data-ttu-id="c21c4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c21c4-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c21c4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c21c4-115">Not supported.</span></span>  |
|<span data-ttu-id="c21c4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c21c4-116">Application</span></span> | <span data-ttu-id="c21c4-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c21c4-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c21c4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c21c4-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c21c4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c21c4-119">Request headers</span></span>
| <span data-ttu-id="c21c4-120">标头</span><span class="sxs-lookup"><span data-stu-id="c21c4-120">Header</span></span>       | <span data-ttu-id="c21c4-121">值</span><span class="sxs-lookup"><span data-stu-id="c21c4-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c21c4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c21c4-122">Authorization</span></span>  | <span data-ttu-id="c21c4-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c21c4-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c21c4-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c21c4-125">Content-Type</span></span>  | <span data-ttu-id="c21c4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c21c4-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c21c4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c21c4-127">Request body</span></span>
<span data-ttu-id="c21c4-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c21c4-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c21c4-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c21c4-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c21c4-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c21c4-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c21c4-131">属性</span><span class="sxs-lookup"><span data-stu-id="c21c4-131">Property</span></span>     | <span data-ttu-id="c21c4-132">类型</span><span class="sxs-lookup"><span data-stu-id="c21c4-132">Type</span></span>   |<span data-ttu-id="c21c4-133">说明</span><span class="sxs-lookup"><span data-stu-id="c21c4-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c21c4-134">displayName</span><span class="sxs-lookup"><span data-stu-id="c21c4-134">displayName</span></span>| <span data-ttu-id="c21c4-135">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-135">String</span></span>| <span data-ttu-id="c21c4-136">学校的显示名称</span><span class="sxs-lookup"><span data-stu-id="c21c4-136">Display name of the school</span></span>| 
|<span data-ttu-id="c21c4-137">description</span><span class="sxs-lookup"><span data-stu-id="c21c4-137">description</span></span>| <span data-ttu-id="c21c4-138">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-138">String</span></span> | <span data-ttu-id="c21c4-139">学校描述</span><span class="sxs-lookup"><span data-stu-id="c21c4-139">Description of the school</span></span>| 
|<span data-ttu-id="c21c4-140">principalEmail</span><span class="sxs-lookup"><span data-stu-id="c21c4-140">principalEmail</span></span>| <span data-ttu-id="c21c4-141">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-141">String</span></span>| <span data-ttu-id="c21c4-142">主体的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="c21c4-142">Email address of the principal</span></span>|
|<span data-ttu-id="c21c4-143">principalName</span><span class="sxs-lookup"><span data-stu-id="c21c4-143">principalName</span></span>| <span data-ttu-id="c21c4-144">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-144">String</span></span> | <span data-ttu-id="c21c4-145">主体名称</span><span class="sxs-lookup"><span data-stu-id="c21c4-145">Name of the principal</span></span>|
|<span data-ttu-id="c21c4-146">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="c21c4-146">externalPrincipalId</span></span>| <span data-ttu-id="c21c4-147">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-147">String</span></span> | <span data-ttu-id="c21c4-148">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="c21c4-148">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="c21c4-149">highestGrade</span><span class="sxs-lookup"><span data-stu-id="c21c4-149">highestGrade</span></span>|<span data-ttu-id="c21c4-150">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-150">String</span></span>| <span data-ttu-id="c21c4-151">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="c21c4-151">Highest grade taught.</span></span> |
|<span data-ttu-id="c21c4-152">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="c21c4-152">lowestGrade</span></span>|<span data-ttu-id="c21c4-153">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-153">String</span></span>| <span data-ttu-id="c21c4-154">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="c21c4-154">Lowest grade taught.</span></span> |
|<span data-ttu-id="c21c4-155">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="c21c4-155">schoolNumber</span></span>|<span data-ttu-id="c21c4-156">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-156">String</span></span>| <span data-ttu-id="c21c4-157">学校编号。</span><span class="sxs-lookup"><span data-stu-id="c21c4-157">School Number.</span></span>|
|<span data-ttu-id="c21c4-158">externalId</span><span class="sxs-lookup"><span data-stu-id="c21c4-158">externalId</span></span>|<span data-ttu-id="c21c4-159">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-159">String</span></span>| <span data-ttu-id="c21c4-160">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="c21c4-160">Id of school in syncing system.</span></span> |
|<span data-ttu-id="c21c4-161">phone</span><span class="sxs-lookup"><span data-stu-id="c21c4-161">phone</span></span>|<span data-ttu-id="c21c4-162">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-162">String</span></span>| <span data-ttu-id="c21c4-163">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="c21c4-163">Phone number of school.</span></span> |
|<span data-ttu-id="c21c4-164">fax</span><span class="sxs-lookup"><span data-stu-id="c21c4-164">fax</span></span>|<span data-ttu-id="c21c4-165">String</span><span class="sxs-lookup"><span data-stu-id="c21c4-165">String</span></span>| <span data-ttu-id="c21c4-166">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="c21c4-166">Fax number of school.</span></span> |
|<span data-ttu-id="c21c4-167">address</span><span class="sxs-lookup"><span data-stu-id="c21c4-167">address</span></span>|[<span data-ttu-id="c21c4-168">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c21c4-168">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="c21c4-169">学校地址。</span><span class="sxs-lookup"><span data-stu-id="c21c4-169">Address of the School.</span></span>|
|<span data-ttu-id="c21c4-170">createdBy</span><span class="sxs-lookup"><span data-stu-id="c21c4-170">createdBy</span></span>|[<span data-ttu-id="c21c4-171">identitySet</span><span class="sxs-lookup"><span data-stu-id="c21c4-171">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="c21c4-172">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="c21c4-172">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="c21c4-173">响应</span><span class="sxs-lookup"><span data-stu-id="c21c4-173">Response</span></span>
<span data-ttu-id="c21c4-174">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c21c4-174">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c21c4-175">示例</span><span class="sxs-lookup"><span data-stu-id="c21c4-175">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c21c4-176">请求</span><span class="sxs-lookup"><span data-stu-id="c21c4-176">Request</span></span>
<span data-ttu-id="c21c4-177">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c21c4-177">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/beta/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="c21c4-178">响应</span><span class="sxs-lookup"><span data-stu-id="c21c4-178">Response</span></span>
<span data-ttu-id="c21c4-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c21c4-179">The following is an example of the response.</span></span> 

><span data-ttu-id="c21c4-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c21c4-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationSchool"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 292

{
  "id": "10002",
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "AmyR@fabrikam.com",
  "principalName": "Amy Roebuck",
  "externalPrincipalId": "14007",
  "highestGrade": "12",
  "lowestGrade": "9",
  "schoolNumber": "10002",
  "address": {
    "city": "Los Angeles",
    "countryOrRegion": "United States",
    "postalCode": "98055",
    "state": "CA",
    "street": "12345 Main St."
  },
  "externalId": "10002",
  "fax": "+1 (253) 555-0101",
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
