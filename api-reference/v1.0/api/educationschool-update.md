---
title: 更新 educationSchool
description: 更新 educationSchool 对象的属性。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: e6c53b2b9b5934559a352378ee5316618ae69abe
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231869"
---
# <a name="update-educationschool"></a><span data-ttu-id="5e366-103">更新 educationSchool</span><span class="sxs-lookup"><span data-stu-id="5e366-103">Update educationSchool</span></span>

<span data-ttu-id="5e366-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5e366-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5e366-105">更新 [educationSchool 对象](../resources/educationschool.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="5e366-105">Update the properties of an [educationSchool](../resources/educationschool.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5e366-106">权限</span><span class="sxs-lookup"><span data-stu-id="5e366-106">Permissions</span></span>

<span data-ttu-id="5e366-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5e366-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5e366-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5e366-109">Permission type</span></span>                        | <span data-ttu-id="5e366-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5e366-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5e366-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5e366-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5e366-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e366-112">Not supported.</span></span>                              |
| <span data-ttu-id="5e366-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5e366-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5e366-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5e366-114">Not supported.</span></span>                              |
| <span data-ttu-id="5e366-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5e366-115">Application</span></span>                            | <span data-ttu-id="5e366-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e366-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="5e366-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5e366-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5e366-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5e366-118">Request headers</span></span>

| <span data-ttu-id="5e366-119">标头</span><span class="sxs-lookup"><span data-stu-id="5e366-119">Header</span></span>        | <span data-ttu-id="5e366-120">值</span><span class="sxs-lookup"><span data-stu-id="5e366-120">Value</span></span>                     |
| :------------ | :------------------------ |
| <span data-ttu-id="5e366-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e366-121">Authorization</span></span> | <span data-ttu-id="5e366-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5e366-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5e366-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5e366-124">Content-Type</span></span>  | <span data-ttu-id="5e366-125">application/json</span><span class="sxs-lookup"><span data-stu-id="5e366-125">application/json</span></span>          |

## <a name="request-body"></a><span data-ttu-id="5e366-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5e366-126">Request body</span></span>

<span data-ttu-id="5e366-127">在请求正文中，提供 [educationSchool](../resources/educationschool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5e366-127">In the request body, supply a JSON representation of the [educationSchool](../resources/educationschool.md) object.</span></span>

<span data-ttu-id="5e366-128">下表显示更新 [educationSchool 时所需的属性](../resources/educationschool.md)。</span><span class="sxs-lookup"><span data-stu-id="5e366-128">The following table shows the properties that are required when you update the [educationSchool](../resources/educationschool.md).</span></span>

| <span data-ttu-id="5e366-129">属性</span><span class="sxs-lookup"><span data-stu-id="5e366-129">Property</span></span>             | <span data-ttu-id="5e366-130">类型</span><span class="sxs-lookup"><span data-stu-id="5e366-130">Type</span></span>                                               | <span data-ttu-id="5e366-131">说明</span><span class="sxs-lookup"><span data-stu-id="5e366-131">Description</span></span>                                                                                                                                                           |
| :------------------- | :------------------------------------------------- | :-------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="5e366-132">displayName</span><span class="sxs-lookup"><span data-stu-id="5e366-132">displayName</span></span>          | <span data-ttu-id="5e366-133">String</span><span class="sxs-lookup"><span data-stu-id="5e366-133">String</span></span>                                             | <span data-ttu-id="5e366-134">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="5e366-134">Display name of the school.</span></span> <span data-ttu-id="5e366-135">继承自 [educationOrganization](../resources/educationorganization.md)。</span><span class="sxs-lookup"><span data-stu-id="5e366-135">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                            |
| <span data-ttu-id="5e366-136">说明</span><span class="sxs-lookup"><span data-stu-id="5e366-136">description</span></span>          | <span data-ttu-id="5e366-137">String</span><span class="sxs-lookup"><span data-stu-id="5e366-137">String</span></span>                                             | <span data-ttu-id="5e366-138">学校描述。</span><span class="sxs-lookup"><span data-stu-id="5e366-138">Description of the school.</span></span> <span data-ttu-id="5e366-139">继承自 [educationOrganization](../resources/educationorganization.md)。</span><span class="sxs-lookup"><span data-stu-id="5e366-139">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span>                                                             |
| <span data-ttu-id="5e366-140">externalSource</span><span class="sxs-lookup"><span data-stu-id="5e366-140">externalSource</span></span>       | <span data-ttu-id="5e366-141">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="5e366-141">educationExternalSource</span></span>                            | <span data-ttu-id="5e366-142">创建组织的来源。</span><span class="sxs-lookup"><span data-stu-id="5e366-142">Source where this organization was created from.</span></span> <span data-ttu-id="5e366-143">继承自 [educationOrganization](../resources/educationorganization.md)。</span><span class="sxs-lookup"><span data-stu-id="5e366-143">Inherited from [educationOrganization](../resources/educationorganization.md).</span></span> <span data-ttu-id="5e366-144">可取值为：`sis`、`manual`。</span><span class="sxs-lookup"><span data-stu-id="5e366-144">Possible values are: `sis`, `manual`.</span></span> |
| <span data-ttu-id="5e366-145">externalSourceDetail</span><span class="sxs-lookup"><span data-stu-id="5e366-145">externalSourceDetail</span></span> | <span data-ttu-id="5e366-146">String</span><span class="sxs-lookup"><span data-stu-id="5e366-146">String</span></span>                                             | <span data-ttu-id="5e366-147">生成此资源的外部源的名称。</span><span class="sxs-lookup"><span data-stu-id="5e366-147">The name of the external source this resources was generated from.</span></span>                                                                                                    |
| <span data-ttu-id="5e366-148">principalEmail</span><span class="sxs-lookup"><span data-stu-id="5e366-148">principalEmail</span></span>       | <span data-ttu-id="5e366-149">String</span><span class="sxs-lookup"><span data-stu-id="5e366-149">String</span></span>                                             | <span data-ttu-id="5e366-150">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="5e366-150">Email address of the principal.</span></span>                                                                                                                                       |
| <span data-ttu-id="5e366-151">principalName</span><span class="sxs-lookup"><span data-stu-id="5e366-151">principalName</span></span>        | <span data-ttu-id="5e366-152">String</span><span class="sxs-lookup"><span data-stu-id="5e366-152">String</span></span>                                             | <span data-ttu-id="5e366-153">主体名称。</span><span class="sxs-lookup"><span data-stu-id="5e366-153">Name of the principal.</span></span>                                                                                                                                                |
| <span data-ttu-id="5e366-154">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="5e366-154">externalPrincipalId</span></span>  | <span data-ttu-id="5e366-155">String</span><span class="sxs-lookup"><span data-stu-id="5e366-155">String</span></span>                                             | <span data-ttu-id="5e366-156">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="5e366-156">ID of principal in syncing system.</span></span>                                                                                                                                    |
| <span data-ttu-id="5e366-157">highestGrade</span><span class="sxs-lookup"><span data-stu-id="5e366-157">highestGrade</span></span>         | <span data-ttu-id="5e366-158">String</span><span class="sxs-lookup"><span data-stu-id="5e366-158">String</span></span>                                             | <span data-ttu-id="5e366-159">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="5e366-159">Highest grade taught.</span></span>                                                                                                                                                 |
| <span data-ttu-id="5e366-160">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="5e366-160">lowestGrade</span></span>          | <span data-ttu-id="5e366-161">String</span><span class="sxs-lookup"><span data-stu-id="5e366-161">String</span></span>                                             | <span data-ttu-id="5e366-162">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="5e366-162">Lowest grade taught.</span></span>                                                                                                                                                  |
| <span data-ttu-id="5e366-163">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="5e366-163">schoolNumber</span></span>         | <span data-ttu-id="5e366-164">String</span><span class="sxs-lookup"><span data-stu-id="5e366-164">String</span></span>                                             | <span data-ttu-id="5e366-165">学校编号。</span><span class="sxs-lookup"><span data-stu-id="5e366-165">School Number.</span></span>                                                                                                                                                        |
| <span data-ttu-id="5e366-166">externalId</span><span class="sxs-lookup"><span data-stu-id="5e366-166">externalId</span></span>           | <span data-ttu-id="5e366-167">String</span><span class="sxs-lookup"><span data-stu-id="5e366-167">String</span></span>                                             | <span data-ttu-id="5e366-168">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="5e366-168">ID of school in syncing system.</span></span>                                                                                                                                       |
| <span data-ttu-id="5e366-169">phone</span><span class="sxs-lookup"><span data-stu-id="5e366-169">phone</span></span>                | <span data-ttu-id="5e366-170">String</span><span class="sxs-lookup"><span data-stu-id="5e366-170">String</span></span>                                             | <span data-ttu-id="5e366-171">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="5e366-171">Phone number of school.</span></span>                                                                                                                                               |
| <span data-ttu-id="5e366-172">fax</span><span class="sxs-lookup"><span data-stu-id="5e366-172">fax</span></span>                  | <span data-ttu-id="5e366-173">String</span><span class="sxs-lookup"><span data-stu-id="5e366-173">String</span></span>                                             | <span data-ttu-id="5e366-174">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="5e366-174">Fax number of school.</span></span>                                                                                                                                                 |
| <span data-ttu-id="5e366-175">createdBy</span><span class="sxs-lookup"><span data-stu-id="5e366-175">createdBy</span></span>            | [<span data-ttu-id="5e366-176">identitySet</span><span class="sxs-lookup"><span data-stu-id="5e366-176">identitySet</span></span>](../resources/identityset.md)         | <span data-ttu-id="5e366-177">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="5e366-177">Entity who created the school.</span></span>                                                                                                                                        |
| <span data-ttu-id="5e366-178">address</span><span class="sxs-lookup"><span data-stu-id="5e366-178">address</span></span>              | [<span data-ttu-id="5e366-179">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="5e366-179">physicalAddress</span></span>](../resources/physicaladdress.md) | <span data-ttu-id="5e366-180">学校地址。</span><span class="sxs-lookup"><span data-stu-id="5e366-180">Address of the school.</span></span>                                                                                                                                                |

## <a name="response"></a><span data-ttu-id="5e366-181">响应</span><span class="sxs-lookup"><span data-stu-id="5e366-181">Response</span></span>

<span data-ttu-id="5e366-182">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5e366-182">If successful, this method returns a `200 OK` response code and an updated [educationSchool](../resources/educationschool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e366-183">示例</span><span class="sxs-lookup"><span data-stu-id="5e366-183">Example</span></span>

##### <a name="request"></a><span data-ttu-id="5e366-184">请求</span><span class="sxs-lookup"><span data-stu-id="5e366-184">Request</span></span>

<span data-ttu-id="5e366-185">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5e366-185">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="5e366-186">HTTP</span><span class="sxs-lookup"><span data-stu-id="5e366-186">HTTP</span></span>](#tab/http)

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

# <a name="c"></a>[<span data-ttu-id="5e366-187">C#</span><span class="sxs-lookup"><span data-stu-id="5e366-187">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationschool-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5e366-188">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5e366-188">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationschool-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5e366-189">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5e366-189">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationschool-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5e366-190">Java</span><span class="sxs-lookup"><span data-stu-id="5e366-190">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationschool-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="5e366-191">响应</span><span class="sxs-lookup"><span data-stu-id="5e366-191">Response</span></span>

<span data-ttu-id="5e366-192">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5e366-192">The following is an example of the response.</span></span>

><span data-ttu-id="5e366-193">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5e366-193">**Note:** The response object shown here might be shortened for readability.</span></span>

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
