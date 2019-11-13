---
title: 更新 educationSchool 属性
description: 更新 school 对象的属性。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 2bd875c4824296c1b5ccfc6bd3969010a00b4f3b
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38303102"
---
# <a name="update-educationschool-properties"></a><span data-ttu-id="bdb59-103">更新 educationSchool 属性</span><span class="sxs-lookup"><span data-stu-id="bdb59-103">Update educationSchool properties</span></span>

<span data-ttu-id="bdb59-104">更新 school 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="bdb59-104">Update the properties of a school object.</span></span>

## <a name="permissions"></a><span data-ttu-id="bdb59-105">权限</span><span class="sxs-lookup"><span data-stu-id="bdb59-105">Permissions</span></span>

<span data-ttu-id="bdb59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bdb59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="bdb59-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="bdb59-108">Permission type</span></span>                        | <span data-ttu-id="bdb59-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bdb59-109">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="bdb59-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bdb59-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="bdb59-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdb59-111">Not supported.</span></span>                              |
| <span data-ttu-id="bdb59-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bdb59-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bdb59-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="bdb59-113">Not supported.</span></span>                              |
| <span data-ttu-id="bdb59-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="bdb59-114">Application</span></span>                            | <span data-ttu-id="bdb59-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bdb59-115">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="bdb59-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bdb59-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="bdb59-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="bdb59-117">Request headers</span></span>

| <span data-ttu-id="bdb59-118">标头</span><span class="sxs-lookup"><span data-stu-id="bdb59-118">Header</span></span>        | <span data-ttu-id="bdb59-119">值</span><span class="sxs-lookup"><span data-stu-id="bdb59-119">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="bdb59-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="bdb59-120">Authorization</span></span> | <span data-ttu-id="bdb59-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bdb59-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="bdb59-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="bdb59-123">Content-Type</span></span>  | <span data-ttu-id="bdb59-124">application/json</span><span class="sxs-lookup"><span data-stu-id="bdb59-124">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="bdb59-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="bdb59-125">Request body</span></span>

<span data-ttu-id="bdb59-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="bdb59-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="bdb59-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="bdb59-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="bdb59-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="bdb59-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="bdb59-129">属性</span><span class="sxs-lookup"><span data-stu-id="bdb59-129">Property</span></span>            | <span data-ttu-id="bdb59-130">类型</span><span class="sxs-lookup"><span data-stu-id="bdb59-130">Type</span></span>                                               | <span data-ttu-id="bdb59-131">说明</span><span class="sxs-lookup"><span data-stu-id="bdb59-131">Description</span></span>                        |
| :------------------ | :------------------------------------------------- | :--------------------------------- |
| <span data-ttu-id="bdb59-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bdb59-132">displayName</span></span>         | <span data-ttu-id="bdb59-133">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-133">String</span></span>                                             | <span data-ttu-id="bdb59-134">学校的显示名称</span><span class="sxs-lookup"><span data-stu-id="bdb59-134">Display name of the school</span></span>         |
| <span data-ttu-id="bdb59-135">说明</span><span class="sxs-lookup"><span data-stu-id="bdb59-135">description</span></span>         | <span data-ttu-id="bdb59-136">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-136">String</span></span>                                             | <span data-ttu-id="bdb59-137">学校描述</span><span class="sxs-lookup"><span data-stu-id="bdb59-137">Description of the school</span></span>          |
| <span data-ttu-id="bdb59-138">principalEmail</span><span class="sxs-lookup"><span data-stu-id="bdb59-138">principalEmail</span></span>      | <span data-ttu-id="bdb59-139">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-139">String</span></span>                                             | <span data-ttu-id="bdb59-140">主体的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="bdb59-140">Email address of the principal</span></span>     |
| <span data-ttu-id="bdb59-141">principalName</span><span class="sxs-lookup"><span data-stu-id="bdb59-141">principalName</span></span>       | <span data-ttu-id="bdb59-142">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-142">String</span></span>                                             | <span data-ttu-id="bdb59-143">主体名称</span><span class="sxs-lookup"><span data-stu-id="bdb59-143">Name of the principal</span></span>              |
| <span data-ttu-id="bdb59-144">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="bdb59-144">externalPrincipalId</span></span> | <span data-ttu-id="bdb59-145">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-145">String</span></span>                                             | <span data-ttu-id="bdb59-146">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="bdb59-146">Id of principal in syncing system.</span></span> |
| <span data-ttu-id="bdb59-147">highestGrade</span><span class="sxs-lookup"><span data-stu-id="bdb59-147">highestGrade</span></span>        | <span data-ttu-id="bdb59-148">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-148">String</span></span>                                             | <span data-ttu-id="bdb59-149">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="bdb59-149">Highest grade taught.</span></span>              |
| <span data-ttu-id="bdb59-150">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="bdb59-150">lowestGrade</span></span>         | <span data-ttu-id="bdb59-151">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-151">String</span></span>                                             | <span data-ttu-id="bdb59-152">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="bdb59-152">Lowest grade taught.</span></span>               |
| <span data-ttu-id="bdb59-153">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="bdb59-153">schoolNumber</span></span>        | <span data-ttu-id="bdb59-154">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-154">String</span></span>                                             | <span data-ttu-id="bdb59-155">学校编号。</span><span class="sxs-lookup"><span data-stu-id="bdb59-155">School Number.</span></span>                     |
| <span data-ttu-id="bdb59-156">externalId</span><span class="sxs-lookup"><span data-stu-id="bdb59-156">externalId</span></span>          | <span data-ttu-id="bdb59-157">字符串</span><span class="sxs-lookup"><span data-stu-id="bdb59-157">String</span></span>                                             | <span data-ttu-id="bdb59-158">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="bdb59-158">Id of school in syncing system.</span></span>    |
| <span data-ttu-id="bdb59-159">phone</span><span class="sxs-lookup"><span data-stu-id="bdb59-159">phone</span></span>               | <span data-ttu-id="bdb59-160">String</span><span class="sxs-lookup"><span data-stu-id="bdb59-160">String</span></span>                                             | <span data-ttu-id="bdb59-161">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="bdb59-161">Phone number of school.</span></span>            |
| <span data-ttu-id="bdb59-162">address</span><span class="sxs-lookup"><span data-stu-id="bdb59-162">address</span></span>             | [<span data-ttu-id="bdb59-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="bdb59-163">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="bdb59-164">学校地址。</span><span class="sxs-lookup"><span data-stu-id="bdb59-164">Address of the School.</span></span>             |
| <span data-ttu-id="bdb59-165">createdBy</span><span class="sxs-lookup"><span data-stu-id="bdb59-165">createdBy</span></span>           | [<span data-ttu-id="bdb59-166">identitySet</span><span class="sxs-lookup"><span data-stu-id="bdb59-166">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="bdb59-167">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="bdb59-167">Entity who created the school.</span></span>     |

## <a name="response"></a><span data-ttu-id="bdb59-168">响应</span><span class="sxs-lookup"><span data-stu-id="bdb59-168">Response</span></span>

<span data-ttu-id="bdb59-169">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bdb59-169">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bdb59-170">示例</span><span class="sxs-lookup"><span data-stu-id="bdb59-170">Example</span></span>

##### <a name="request"></a><span data-ttu-id="bdb59-171">请求</span><span class="sxs-lookup"><span data-stu-id="bdb59-171">Request</span></span>

<span data-ttu-id="bdb59-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="bdb59-172">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="bdb59-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="bdb59-173">HTTP</span></span>](#tab/http)

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

# <a name="ctabcsharp"></a>[<span data-ttu-id="bdb59-174">C#</span><span class="sxs-lookup"><span data-stu-id="bdb59-174">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="bdb59-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="bdb59-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="bdb59-176">Objective-C</span><span class="sxs-lookup"><span data-stu-id="bdb59-176">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="bdb59-177">Java</span><span class="sxs-lookup"><span data-stu-id="bdb59-177">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="bdb59-178">响应</span><span class="sxs-lookup"><span data-stu-id="bdb59-178">Response</span></span>

<span data-ttu-id="bdb59-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="bdb59-179">The following is an example of the response.</span></span>

><span data-ttu-id="bdb59-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="bdb59-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationschool",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
