---
title: 更新 educationSchool 属性
description: 更新 school 对象的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: c4fb5d13264a653c8eda5856103334e348e66512
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47991325"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="91988-103">更新 educationschool 属性</span><span class="sxs-lookup"><span data-stu-id="91988-103">Update educationschool properties</span></span>

<span data-ttu-id="91988-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91988-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91988-105">更新 school 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="91988-105">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="91988-106">权限</span><span class="sxs-lookup"><span data-stu-id="91988-106">Permissions</span></span>

<span data-ttu-id="91988-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91988-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="91988-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="91988-109">Permission type</span></span>                        | <span data-ttu-id="91988-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91988-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="91988-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91988-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="91988-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="91988-112">Not supported.</span></span>                              |
| <span data-ttu-id="91988-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91988-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91988-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="91988-114">Not supported.</span></span>                              |
| <span data-ttu-id="91988-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="91988-115">Application</span></span>                            | <span data-ttu-id="91988-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91988-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="91988-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91988-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="91988-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="91988-118">Request headers</span></span>

| <span data-ttu-id="91988-119">标头</span><span class="sxs-lookup"><span data-stu-id="91988-119">Header</span></span>        | <span data-ttu-id="91988-120">值</span><span class="sxs-lookup"><span data-stu-id="91988-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="91988-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="91988-121">Authorization</span></span> | <span data-ttu-id="91988-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="91988-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="91988-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="91988-124">Content-Type</span></span>  | <span data-ttu-id="91988-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91988-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="91988-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="91988-126">Request body</span></span>

<span data-ttu-id="91988-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="91988-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="91988-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="91988-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="91988-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="91988-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="91988-130">属性</span><span class="sxs-lookup"><span data-stu-id="91988-130">Property</span></span>            | <span data-ttu-id="91988-131">类型</span><span class="sxs-lookup"><span data-stu-id="91988-131">Type</span></span>                                               | <span data-ttu-id="91988-132">说明</span><span class="sxs-lookup"><span data-stu-id="91988-132">Description</span></span>                        |
| :------------------ | :------------------------------------------------- | :--------------------------------- |
| <span data-ttu-id="91988-133">displayName</span><span class="sxs-lookup"><span data-stu-id="91988-133">displayName</span></span>         | <span data-ttu-id="91988-134">String</span><span class="sxs-lookup"><span data-stu-id="91988-134">String</span></span>                                             | <span data-ttu-id="91988-135">学校的显示名称</span><span class="sxs-lookup"><span data-stu-id="91988-135">Display name of the school</span></span>         |
| <span data-ttu-id="91988-136">description</span><span class="sxs-lookup"><span data-stu-id="91988-136">description</span></span>         | <span data-ttu-id="91988-137">String</span><span class="sxs-lookup"><span data-stu-id="91988-137">String</span></span>                                             | <span data-ttu-id="91988-138">学校描述</span><span class="sxs-lookup"><span data-stu-id="91988-138">Description of the school</span></span>          |
| <span data-ttu-id="91988-139">principalEmail</span><span class="sxs-lookup"><span data-stu-id="91988-139">principalEmail</span></span>      | <span data-ttu-id="91988-140">String</span><span class="sxs-lookup"><span data-stu-id="91988-140">String</span></span>                                             | <span data-ttu-id="91988-141">主体的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="91988-141">Email address of the principal</span></span>     |
| <span data-ttu-id="91988-142">principalName</span><span class="sxs-lookup"><span data-stu-id="91988-142">principalName</span></span>       | <span data-ttu-id="91988-143">String</span><span class="sxs-lookup"><span data-stu-id="91988-143">String</span></span>                                             | <span data-ttu-id="91988-144">主体名称</span><span class="sxs-lookup"><span data-stu-id="91988-144">Name of the principal</span></span>              |
| <span data-ttu-id="91988-145">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="91988-145">externalPrincipalId</span></span> | <span data-ttu-id="91988-146">String</span><span class="sxs-lookup"><span data-stu-id="91988-146">String</span></span>                                             | <span data-ttu-id="91988-147">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="91988-147">Id of principal in syncing system.</span></span> |
| <span data-ttu-id="91988-148">highestGrade</span><span class="sxs-lookup"><span data-stu-id="91988-148">highestGrade</span></span>        | <span data-ttu-id="91988-149">String</span><span class="sxs-lookup"><span data-stu-id="91988-149">String</span></span>                                             | <span data-ttu-id="91988-150">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="91988-150">Highest grade taught.</span></span>              |
| <span data-ttu-id="91988-151">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="91988-151">lowestGrade</span></span>         | <span data-ttu-id="91988-152">String</span><span class="sxs-lookup"><span data-stu-id="91988-152">String</span></span>                                             | <span data-ttu-id="91988-153">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="91988-153">Lowest grade taught.</span></span>               |
| <span data-ttu-id="91988-154">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="91988-154">schoolNumber</span></span>        | <span data-ttu-id="91988-155">String</span><span class="sxs-lookup"><span data-stu-id="91988-155">String</span></span>                                             | <span data-ttu-id="91988-156">学校编号。</span><span class="sxs-lookup"><span data-stu-id="91988-156">School Number.</span></span>                     |
| <span data-ttu-id="91988-157">externalId</span><span class="sxs-lookup"><span data-stu-id="91988-157">externalId</span></span>          | <span data-ttu-id="91988-158">String</span><span class="sxs-lookup"><span data-stu-id="91988-158">String</span></span>                                             | <span data-ttu-id="91988-159">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="91988-159">Id of school in syncing system.</span></span>    |
| <span data-ttu-id="91988-160">phone</span><span class="sxs-lookup"><span data-stu-id="91988-160">phone</span></span>               | <span data-ttu-id="91988-161">String</span><span class="sxs-lookup"><span data-stu-id="91988-161">String</span></span>                                             | <span data-ttu-id="91988-162">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="91988-162">Phone number of school.</span></span>            |
| <span data-ttu-id="91988-163">address</span><span class="sxs-lookup"><span data-stu-id="91988-163">address</span></span>             | [<span data-ttu-id="91988-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="91988-164">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="91988-165">学校地址。</span><span class="sxs-lookup"><span data-stu-id="91988-165">Address of the School.</span></span>             |
| <span data-ttu-id="91988-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="91988-166">createdBy</span></span>           | [<span data-ttu-id="91988-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="91988-167">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="91988-168">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="91988-168">Entity who created the school.</span></span>     |

## <a name="response"></a><span data-ttu-id="91988-169">响应</span><span class="sxs-lookup"><span data-stu-id="91988-169">Response</span></span>
<span data-ttu-id="91988-170">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="91988-170">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91988-171">示例</span><span class="sxs-lookup"><span data-stu-id="91988-171">Example</span></span>

##### <a name="request"></a><span data-ttu-id="91988-172">请求</span><span class="sxs-lookup"><span data-stu-id="91988-172">Request</span></span>

<span data-ttu-id="91988-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="91988-173">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="91988-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="91988-174">HTTP</span></span>](#tab/http)

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
# <a name="c"></a>[<span data-ttu-id="91988-175">C#</span><span class="sxs-lookup"><span data-stu-id="91988-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
# <a name="javascript"></a>[<span data-ttu-id="91988-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="91988-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]
# <a name="objective-c"></a>[<span data-ttu-id="91988-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="91988-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="91988-178">响应</span><span class="sxs-lookup"><span data-stu-id="91988-178">Response</span></span>

<span data-ttu-id="91988-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="91988-179">The following is an example of the response.</span></span>

><span data-ttu-id="91988-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="91988-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "phone": "+1 (253) 555-0102"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


