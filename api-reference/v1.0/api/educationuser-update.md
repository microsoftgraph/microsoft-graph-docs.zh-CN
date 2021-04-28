---
title: 更新 educationUser 属性
description: 更新 **educationuser** 对象的属性。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 32645e98fbb2e7da1aeec8d48eddb3c5da6822bb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52054033"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="c6043-103">更新 educationUser 属性</span><span class="sxs-lookup"><span data-stu-id="c6043-103">Update educationUser properties</span></span>

<span data-ttu-id="c6043-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c6043-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c6043-105">更新 **educationuser** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c6043-105">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="c6043-106">权限</span><span class="sxs-lookup"><span data-stu-id="c6043-106">Permissions</span></span>
<span data-ttu-id="c6043-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c6043-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c6043-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c6043-109">Permission type</span></span>      | <span data-ttu-id="c6043-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c6043-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c6043-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c6043-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="c6043-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6043-112">Not supported.</span></span>  |
|<span data-ttu-id="c6043-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c6043-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="c6043-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c6043-114">Not supported.</span></span>  |
|<span data-ttu-id="c6043-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c6043-115">Application</span></span> | <span data-ttu-id="c6043-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c6043-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c6043-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c6043-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="c6043-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c6043-118">Request headers</span></span>
| <span data-ttu-id="c6043-119">标头</span><span class="sxs-lookup"><span data-stu-id="c6043-119">Header</span></span>       | <span data-ttu-id="c6043-120">值</span><span class="sxs-lookup"><span data-stu-id="c6043-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c6043-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c6043-121">Authorization</span></span>  | <span data-ttu-id="c6043-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c6043-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c6043-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c6043-124">Content-Type</span></span>  | <span data-ttu-id="c6043-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c6043-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c6043-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c6043-126">Request body</span></span>
<span data-ttu-id="c6043-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="c6043-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="c6043-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="c6043-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="c6043-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="c6043-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="c6043-130">属性</span><span class="sxs-lookup"><span data-stu-id="c6043-130">Property</span></span>     | <span data-ttu-id="c6043-131">类型</span><span class="sxs-lookup"><span data-stu-id="c6043-131">Type</span></span>   |<span data-ttu-id="c6043-132">说明</span><span class="sxs-lookup"><span data-stu-id="c6043-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c6043-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c6043-133">displayName</span></span>| <span data-ttu-id="c6043-134">String</span><span class="sxs-lookup"><span data-stu-id="c6043-134">String</span></span>| <span data-ttu-id="c6043-135">显示用户名称</span><span class="sxs-lookup"><span data-stu-id="c6043-135">Display Name of User</span></span>|
|<span data-ttu-id="c6043-136">givenName</span><span class="sxs-lookup"><span data-stu-id="c6043-136">givenName</span></span>| <span data-ttu-id="c6043-137">String</span><span class="sxs-lookup"><span data-stu-id="c6043-137">String</span></span> | <span data-ttu-id="c6043-138">名字</span><span class="sxs-lookup"><span data-stu-id="c6043-138">First Name</span></span> |
|<span data-ttu-id="c6043-139">middleName</span><span class="sxs-lookup"><span data-stu-id="c6043-139">middleName</span></span>| <span data-ttu-id="c6043-140">String</span><span class="sxs-lookup"><span data-stu-id="c6043-140">String</span></span> | <span data-ttu-id="c6043-141">用户的中间名</span><span class="sxs-lookup"><span data-stu-id="c6043-141">Middle Name of user</span></span>|
|<span data-ttu-id="c6043-142">surname</span><span class="sxs-lookup"><span data-stu-id="c6043-142">surname</span></span>| <span data-ttu-id="c6043-143">String</span><span class="sxs-lookup"><span data-stu-id="c6043-143">String</span></span> | <span data-ttu-id="c6043-144">用户的姓</span><span class="sxs-lookup"><span data-stu-id="c6043-144">Surname of user</span></span>|
|<span data-ttu-id="c6043-145">mail</span><span class="sxs-lookup"><span data-stu-id="c6043-145">mail</span></span>| <span data-ttu-id="c6043-146">String</span><span class="sxs-lookup"><span data-stu-id="c6043-146">String</span></span>| <span data-ttu-id="c6043-147">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="c6043-147">email address</span></span>|
|<span data-ttu-id="c6043-148">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="c6043-148">mobilePhone</span></span>| <span data-ttu-id="c6043-149">String</span><span class="sxs-lookup"><span data-stu-id="c6043-149">String</span></span> | <span data-ttu-id="c6043-150">用户的移动电话号码</span><span class="sxs-lookup"><span data-stu-id="c6043-150">Mobile number of user</span></span> |
|<span data-ttu-id="c6043-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="c6043-151">externalSource</span></span>|<span data-ttu-id="c6043-152">string</span><span class="sxs-lookup"><span data-stu-id="c6043-152">string</span></span>| <span data-ttu-id="c6043-153">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="c6043-153">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="c6043-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="c6043-154">externalSource</span></span>|<span data-ttu-id="c6043-155">string</span><span class="sxs-lookup"><span data-stu-id="c6043-155">string</span></span>| <span data-ttu-id="c6043-156">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="c6043-156">Where this user was created from.</span></span>  <span data-ttu-id="c6043-157">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="c6043-157">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="c6043-158">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="c6043-158">mailingAddress</span></span>|[<span data-ttu-id="c6043-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6043-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="c6043-160">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c6043-160">Mail address of user.</span></span>|
|<span data-ttu-id="c6043-161">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="c6043-161">residenceAddress</span></span>|[<span data-ttu-id="c6043-162">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="c6043-162">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="c6043-163">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="c6043-163">Address where user lives.</span></span>|
|<span data-ttu-id="c6043-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="c6043-164">primaryRole</span></span>|<span data-ttu-id="c6043-165">string</span><span class="sxs-lookup"><span data-stu-id="c6043-165">string</span></span>| <span data-ttu-id="c6043-166">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="c6043-166">Default Role for a user.</span></span>  <span data-ttu-id="c6043-167">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="c6043-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="c6043-168">可能的值包括 `student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="c6043-168">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="c6043-169">student</span><span class="sxs-lookup"><span data-stu-id="c6043-169">student</span></span>|[<span data-ttu-id="c6043-170">educationStudent</span><span class="sxs-lookup"><span data-stu-id="c6043-170">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="c6043-171">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="c6043-171">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="c6043-172">teacher</span><span class="sxs-lookup"><span data-stu-id="c6043-172">teacher</span></span>|[<span data-ttu-id="c6043-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="c6043-173">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="c6043-174">如果主要角色是教师，则此块将包含特定于教师的数据。</span><span class="sxs-lookup"><span data-stu-id="c6043-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="c6043-175">响应</span><span class="sxs-lookup"><span data-stu-id="c6043-175">Response</span></span>
<span data-ttu-id="c6043-176">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c6043-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c6043-177">示例</span><span class="sxs-lookup"><span data-stu-id="c6043-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c6043-178">请求</span><span class="sxs-lookup"><span data-stu-id="c6043-178">Request</span></span>
<span data-ttu-id="c6043-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c6043-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c6043-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="c6043-180">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/users/{user-id}
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```
# <a name="c"></a>[<span data-ttu-id="c6043-181">C#</span><span class="sxs-lookup"><span data-stu-id="c6043-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c6043-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c6043-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c6043-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c6043-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c6043-184">Java</span><span class="sxs-lookup"><span data-stu-id="c6043-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c6043-185">响应</span><span class="sxs-lookup"><span data-stu-id="c6043-185">Response</span></span>
<span data-ttu-id="c6043-186">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c6043-186">Here is an example of the response.</span></span> <span data-ttu-id="c6043-187">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c6043-187">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 508

{
  "id": "13020",
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
  "mail": "rogelioC@contoso.com",
  "mobilePhone": "+1 (253) 555-0101",
  "createdBy": {
        "user": {
          "displayName": "Susana Rocha",
          "id": "14012",
        }
  },
  "externalSource": "sis",
  "mailingAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "primaryRole": "student",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

