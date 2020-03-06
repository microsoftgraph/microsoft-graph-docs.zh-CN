---
title: 更新 educationUser 属性
description: 更新 **educationuser** 对象的属性。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 61c6293840c544e397f6761149c9131c94d9f930
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42517402"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="4c86d-103">更新 educationUser 属性</span><span class="sxs-lookup"><span data-stu-id="4c86d-103">Update educationUser properties</span></span>

<span data-ttu-id="4c86d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c86d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4c86d-105">更新 **educationuser** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4c86d-105">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="4c86d-106">权限</span><span class="sxs-lookup"><span data-stu-id="4c86d-106">Permissions</span></span>
<span data-ttu-id="4c86d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c86d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c86d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c86d-109">Permission type</span></span>      | <span data-ttu-id="4c86d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4c86d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4c86d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c86d-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="4c86d-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c86d-112">Not supported.</span></span>  |
|<span data-ttu-id="4c86d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c86d-113">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="4c86d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c86d-114">Not supported.</span></span>  |
|<span data-ttu-id="4c86d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c86d-115">Application</span></span> | <span data-ttu-id="4c86d-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c86d-116">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="4c86d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c86d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="4c86d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c86d-118">Request headers</span></span>
| <span data-ttu-id="4c86d-119">标头</span><span class="sxs-lookup"><span data-stu-id="4c86d-119">Header</span></span>       | <span data-ttu-id="4c86d-120">值</span><span class="sxs-lookup"><span data-stu-id="4c86d-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="4c86d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c86d-121">Authorization</span></span>  | <span data-ttu-id="4c86d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4c86d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="4c86d-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="4c86d-124">Content-Type</span></span>  | <span data-ttu-id="4c86d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c86d-125">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="4c86d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c86d-126">Request body</span></span>
<span data-ttu-id="4c86d-127">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="4c86d-127">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="4c86d-128">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="4c86d-128">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="4c86d-129">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="4c86d-129">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="4c86d-130">属性</span><span class="sxs-lookup"><span data-stu-id="4c86d-130">Property</span></span>     | <span data-ttu-id="4c86d-131">类型</span><span class="sxs-lookup"><span data-stu-id="4c86d-131">Type</span></span>   |<span data-ttu-id="4c86d-132">说明</span><span class="sxs-lookup"><span data-stu-id="4c86d-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4c86d-133">displayName</span><span class="sxs-lookup"><span data-stu-id="4c86d-133">displayName</span></span>| <span data-ttu-id="4c86d-134">字符串</span><span class="sxs-lookup"><span data-stu-id="4c86d-134">String</span></span>| <span data-ttu-id="4c86d-135">显示用户名称</span><span class="sxs-lookup"><span data-stu-id="4c86d-135">Display Name of User</span></span>|
|<span data-ttu-id="4c86d-136">givenName</span><span class="sxs-lookup"><span data-stu-id="4c86d-136">givenName</span></span>| <span data-ttu-id="4c86d-137">字符串</span><span class="sxs-lookup"><span data-stu-id="4c86d-137">String</span></span> | <span data-ttu-id="4c86d-138">名字</span><span class="sxs-lookup"><span data-stu-id="4c86d-138">First Name</span></span> |
|<span data-ttu-id="4c86d-139">middleName</span><span class="sxs-lookup"><span data-stu-id="4c86d-139">middleName</span></span>| <span data-ttu-id="4c86d-140">String</span><span class="sxs-lookup"><span data-stu-id="4c86d-140">String</span></span> | <span data-ttu-id="4c86d-141">用户的中间名</span><span class="sxs-lookup"><span data-stu-id="4c86d-141">Middle Name of user</span></span>|
|<span data-ttu-id="4c86d-142">surname</span><span class="sxs-lookup"><span data-stu-id="4c86d-142">surname</span></span>| <span data-ttu-id="4c86d-143">字符串</span><span class="sxs-lookup"><span data-stu-id="4c86d-143">String</span></span> | <span data-ttu-id="4c86d-144">用户的姓</span><span class="sxs-lookup"><span data-stu-id="4c86d-144">Surname of user</span></span>|
|<span data-ttu-id="4c86d-145">mail</span><span class="sxs-lookup"><span data-stu-id="4c86d-145">mail</span></span>| <span data-ttu-id="4c86d-146">String</span><span class="sxs-lookup"><span data-stu-id="4c86d-146">String</span></span>| <span data-ttu-id="4c86d-147">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="4c86d-147">email address</span></span>|
|<span data-ttu-id="4c86d-148">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="4c86d-148">mobilePhone</span></span>| <span data-ttu-id="4c86d-149">String</span><span class="sxs-lookup"><span data-stu-id="4c86d-149">String</span></span> | <span data-ttu-id="4c86d-150">用户的移动电话号码</span><span class="sxs-lookup"><span data-stu-id="4c86d-150">Mobile number of user</span></span> |
|<span data-ttu-id="4c86d-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="4c86d-151">externalSource</span></span>|<span data-ttu-id="4c86d-152">字符串</span><span class="sxs-lookup"><span data-stu-id="4c86d-152">string</span></span>| <span data-ttu-id="4c86d-153">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="4c86d-153">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="4c86d-154">externalSource</span><span class="sxs-lookup"><span data-stu-id="4c86d-154">externalSource</span></span>|<span data-ttu-id="4c86d-155">字符串</span><span class="sxs-lookup"><span data-stu-id="4c86d-155">string</span></span>| <span data-ttu-id="4c86d-156">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="4c86d-156">Where this user was created from.</span></span>  <span data-ttu-id="4c86d-157">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="4c86d-157">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="4c86d-158">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="4c86d-158">mailingAddress</span></span>|[<span data-ttu-id="4c86d-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4c86d-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="4c86d-160">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="4c86d-160">Mail address of user.</span></span>|
|<span data-ttu-id="4c86d-161">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="4c86d-161">residenceAddress</span></span>|[<span data-ttu-id="4c86d-162">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="4c86d-162">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="4c86d-163">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="4c86d-163">Address where user lives.</span></span>|
|<span data-ttu-id="4c86d-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="4c86d-164">primaryRole</span></span>|<span data-ttu-id="4c86d-165">string</span><span class="sxs-lookup"><span data-stu-id="4c86d-165">string</span></span>| <span data-ttu-id="4c86d-166">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="4c86d-166">Default Role for a user.</span></span>  <span data-ttu-id="4c86d-167">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="4c86d-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="4c86d-168">可能的值包括 `student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="4c86d-168">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="4c86d-169">student</span><span class="sxs-lookup"><span data-stu-id="4c86d-169">student</span></span>|[<span data-ttu-id="4c86d-170">educationStudent</span><span class="sxs-lookup"><span data-stu-id="4c86d-170">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="4c86d-171">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="4c86d-171">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="4c86d-172">teacher</span><span class="sxs-lookup"><span data-stu-id="4c86d-172">teacher</span></span>|[<span data-ttu-id="4c86d-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="4c86d-173">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="4c86d-174">如果主要角色是教师，此块将包含教师特定的数据。</span><span class="sxs-lookup"><span data-stu-id="4c86d-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="4c86d-175">响应</span><span class="sxs-lookup"><span data-stu-id="4c86d-175">Response</span></span>
<span data-ttu-id="4c86d-176">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c86d-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="4c86d-177">示例</span><span class="sxs-lookup"><span data-stu-id="4c86d-177">Example</span></span>
##### <a name="request"></a><span data-ttu-id="4c86d-178">请求</span><span class="sxs-lookup"><span data-stu-id="4c86d-178">Request</span></span>
<span data-ttu-id="4c86d-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c86d-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="4c86d-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="4c86d-180">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="4c86d-181">C#</span><span class="sxs-lookup"><span data-stu-id="4c86d-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4c86d-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4c86d-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4c86d-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4c86d-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4c86d-184">Java</span><span class="sxs-lookup"><span data-stu-id="4c86d-184">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="4c86d-185">响应</span><span class="sxs-lookup"><span data-stu-id="4c86d-185">Response</span></span>
<span data-ttu-id="4c86d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c86d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
