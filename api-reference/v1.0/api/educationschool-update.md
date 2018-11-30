---
title: 更新 educationschool 属性
description: 更新 school 对象的属性。
ms.openlocfilehash: aa413360305b32f3e2c5288192929ae48279bd60
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27007815"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="a3ca7-103">更新 educationschool 属性</span><span class="sxs-lookup"><span data-stu-id="a3ca7-103">Update educationschool properties</span></span>

<span data-ttu-id="a3ca7-104">更新 school 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a3ca7-105">权限</span><span class="sxs-lookup"><span data-stu-id="a3ca7-105">Permissions</span></span>
<span data-ttu-id="a3ca7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3ca7-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3ca7-108">Permission type</span></span>      | <span data-ttu-id="a3ca7-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3ca7-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a3ca7-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ca7-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="a3ca7-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-111">Not supported.</span></span>  |
|<span data-ttu-id="a3ca7-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3ca7-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="a3ca7-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-113">Not supported.</span></span>  |
|<span data-ttu-id="a3ca7-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3ca7-114">Application</span></span> | <span data-ttu-id="a3ca7-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3ca7-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a3ca7-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3ca7-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="a3ca7-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3ca7-117">Request headers</span></span>
| <span data-ttu-id="a3ca7-118">标头</span><span class="sxs-lookup"><span data-stu-id="a3ca7-118">Header</span></span>       | <span data-ttu-id="a3ca7-119">值</span><span class="sxs-lookup"><span data-stu-id="a3ca7-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="a3ca7-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3ca7-120">Authorization</span></span>  | <span data-ttu-id="a3ca7-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="a3ca7-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="a3ca7-123">Content-Type</span></span>  | <span data-ttu-id="a3ca7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3ca7-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="a3ca7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3ca7-125">Request body</span></span>
<span data-ttu-id="a3ca7-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="a3ca7-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a3ca7-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="a3ca7-129">属性</span><span class="sxs-lookup"><span data-stu-id="a3ca7-129">Property</span></span>     | <span data-ttu-id="a3ca7-130">类型</span><span class="sxs-lookup"><span data-stu-id="a3ca7-130">Type</span></span>   |<span data-ttu-id="a3ca7-131">说明</span><span class="sxs-lookup"><span data-stu-id="a3ca7-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3ca7-132">displayName</span><span class="sxs-lookup"><span data-stu-id="a3ca7-132">displayName</span></span>| <span data-ttu-id="a3ca7-133">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-133">String</span></span>| <span data-ttu-id="a3ca7-134">学校的显示名称</span><span class="sxs-lookup"><span data-stu-id="a3ca7-134">Display name of the school</span></span>| 
|<span data-ttu-id="a3ca7-135">description</span><span class="sxs-lookup"><span data-stu-id="a3ca7-135">description</span></span>| <span data-ttu-id="a3ca7-136">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-136">String</span></span> | <span data-ttu-id="a3ca7-137">学校描述</span><span class="sxs-lookup"><span data-stu-id="a3ca7-137">Description of the school</span></span>| 
|<span data-ttu-id="a3ca7-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="a3ca7-138">principalEmail</span></span>| <span data-ttu-id="a3ca7-139">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-139">String</span></span>| <span data-ttu-id="a3ca7-140">主体的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="a3ca7-140">Email address of the principal</span></span>|
|<span data-ttu-id="a3ca7-141">principalName</span><span class="sxs-lookup"><span data-stu-id="a3ca7-141">principalName</span></span>| <span data-ttu-id="a3ca7-142">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-142">String</span></span> | <span data-ttu-id="a3ca7-143">主体名称</span><span class="sxs-lookup"><span data-stu-id="a3ca7-143">Name of the principal</span></span>|
|<span data-ttu-id="a3ca7-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="a3ca7-144">externalPrincipalId</span></span>| <span data-ttu-id="a3ca7-145">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-145">String</span></span> | <span data-ttu-id="a3ca7-146">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-146">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="a3ca7-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="a3ca7-147">highestGrade</span></span>|<span data-ttu-id="a3ca7-148">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-148">String</span></span>| <span data-ttu-id="a3ca7-149">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-149">Highest grade taught.</span></span> |
|<span data-ttu-id="a3ca7-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="a3ca7-150">lowestGrade</span></span>|<span data-ttu-id="a3ca7-151">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-151">String</span></span>| <span data-ttu-id="a3ca7-152">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-152">Lowest grade taught.</span></span> |
|<span data-ttu-id="a3ca7-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="a3ca7-153">schoolNumber</span></span>|<span data-ttu-id="a3ca7-154">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-154">String</span></span>| <span data-ttu-id="a3ca7-155">学校编号。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-155">School Number.</span></span>|
|<span data-ttu-id="a3ca7-156">externalId</span><span class="sxs-lookup"><span data-stu-id="a3ca7-156">externalId</span></span>|<span data-ttu-id="a3ca7-157">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-157">String</span></span>| <span data-ttu-id="a3ca7-158">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-158">Id of school in syncing system.</span></span> |
|<span data-ttu-id="a3ca7-159">phone</span><span class="sxs-lookup"><span data-stu-id="a3ca7-159">phone</span></span>|<span data-ttu-id="a3ca7-160">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-160">String</span></span>| <span data-ttu-id="a3ca7-161">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-161">Phone number of school.</span></span> |
|<span data-ttu-id="a3ca7-162">fax</span><span class="sxs-lookup"><span data-stu-id="a3ca7-162">fax</span></span>|<span data-ttu-id="a3ca7-163">String</span><span class="sxs-lookup"><span data-stu-id="a3ca7-163">String</span></span>| <span data-ttu-id="a3ca7-164">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-164">Fax number of school.</span></span> |
|<span data-ttu-id="a3ca7-165">address</span><span class="sxs-lookup"><span data-stu-id="a3ca7-165">address</span></span>|[<span data-ttu-id="a3ca7-166">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="a3ca7-166">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="a3ca7-167">学校地址。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-167">Address of the School.</span></span>|
|<span data-ttu-id="a3ca7-168">createdBy</span><span class="sxs-lookup"><span data-stu-id="a3ca7-168">createdBy</span></span>|[<span data-ttu-id="a3ca7-169">identitySet</span><span class="sxs-lookup"><span data-stu-id="a3ca7-169">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="a3ca7-170">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-170">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="a3ca7-171">响应</span><span class="sxs-lookup"><span data-stu-id="a3ca7-171">Response</span></span>
<span data-ttu-id="a3ca7-172">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-172">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a3ca7-173">示例</span><span class="sxs-lookup"><span data-stu-id="a3ca7-173">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a3ca7-174">请求</span><span class="sxs-lookup"><span data-stu-id="a3ca7-174">Request</span></span>
<span data-ttu-id="a3ca7-175">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-175">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/{school-id}
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="a3ca7-176">响应</span><span class="sxs-lookup"><span data-stu-id="a3ca7-176">Response</span></span>
<span data-ttu-id="a3ca7-177">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-177">The following is an example of the response.</span></span> 

><span data-ttu-id="a3ca7-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a3ca7-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
