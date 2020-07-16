---
title: 更新 educationUser 属性
description: 更新 **educationuser** 对象的属性。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: 022b30eb68b29f4a77c34b0a8dc588d6f4bba071
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006752"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="afb7f-103">更新 educationUser 属性</span><span class="sxs-lookup"><span data-stu-id="afb7f-103">Update educationUser properties</span></span>

<span data-ttu-id="afb7f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb7f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="afb7f-105">更新 **educationuser** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="afb7f-105">Update the properties of an **educationuser** object.</span></span>

## <a name="permissions"></a><span data-ttu-id="afb7f-106">权限</span><span class="sxs-lookup"><span data-stu-id="afb7f-106">Permissions</span></span>

<span data-ttu-id="afb7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afb7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="afb7f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="afb7f-109">Permission type</span></span>                        | <span data-ttu-id="afb7f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="afb7f-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="afb7f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afb7f-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="afb7f-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="afb7f-112">Not supported.</span></span>                              |
| <span data-ttu-id="afb7f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afb7f-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="afb7f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="afb7f-114">Not supported.</span></span>                              |
| <span data-ttu-id="afb7f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="afb7f-115">Application</span></span>                            | <span data-ttu-id="afb7f-116">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb7f-116">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="afb7f-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afb7f-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH /education/me
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="afb7f-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="afb7f-118">Request headers</span></span>

| <span data-ttu-id="afb7f-119">标头</span><span class="sxs-lookup"><span data-stu-id="afb7f-119">Header</span></span>        | <span data-ttu-id="afb7f-120">值</span><span class="sxs-lookup"><span data-stu-id="afb7f-120">Value</span></span>                       |
| :------------ | :-------------------------- |
| <span data-ttu-id="afb7f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="afb7f-121">Authorization</span></span> | <span data-ttu-id="afb7f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="afb7f-p102">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="afb7f-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="afb7f-124">Content-Type</span></span>  | <span data-ttu-id="afb7f-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="afb7f-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="afb7f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="afb7f-127">Request body</span></span>

<span data-ttu-id="afb7f-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="afb7f-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="afb7f-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="afb7f-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="afb7f-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="afb7f-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="afb7f-131">属性</span><span class="sxs-lookup"><span data-stu-id="afb7f-131">Property</span></span>         | <span data-ttu-id="afb7f-132">类型</span><span class="sxs-lookup"><span data-stu-id="afb7f-132">Type</span></span>               | <span data-ttu-id="afb7f-133">说明</span><span class="sxs-lookup"><span data-stu-id="afb7f-133">Description</span></span>                                                                                                                                     |
| :--------------- | :----------------- | :---------------------------------------------------------------------------------------------------------------------------------------------- |
| <span data-ttu-id="afb7f-134">displayName</span><span class="sxs-lookup"><span data-stu-id="afb7f-134">displayName</span></span>      | <span data-ttu-id="afb7f-135">String</span><span class="sxs-lookup"><span data-stu-id="afb7f-135">String</span></span>             | <span data-ttu-id="afb7f-136">显示用户名称</span><span class="sxs-lookup"><span data-stu-id="afb7f-136">Display Name of User</span></span>                                                                                                                            |
| <span data-ttu-id="afb7f-137">givenName</span><span class="sxs-lookup"><span data-stu-id="afb7f-137">givenName</span></span>        | <span data-ttu-id="afb7f-138">String</span><span class="sxs-lookup"><span data-stu-id="afb7f-138">String</span></span>             | <span data-ttu-id="afb7f-139">名字</span><span class="sxs-lookup"><span data-stu-id="afb7f-139">First Name</span></span>                                                                                                                                      |
| <span data-ttu-id="afb7f-140">middleName</span><span class="sxs-lookup"><span data-stu-id="afb7f-140">middleName</span></span>       | <span data-ttu-id="afb7f-141">String</span><span class="sxs-lookup"><span data-stu-id="afb7f-141">String</span></span>             | <span data-ttu-id="afb7f-142">用户的中间名</span><span class="sxs-lookup"><span data-stu-id="afb7f-142">Middle Name of user</span></span>                                                                                                                             |
| <span data-ttu-id="afb7f-143">surname</span><span class="sxs-lookup"><span data-stu-id="afb7f-143">surname</span></span>          | <span data-ttu-id="afb7f-144">字符串</span><span class="sxs-lookup"><span data-stu-id="afb7f-144">String</span></span>             | <span data-ttu-id="afb7f-145">用户的姓</span><span class="sxs-lookup"><span data-stu-id="afb7f-145">Surname of user</span></span>                                                                                                                                 |
| <span data-ttu-id="afb7f-146">mail</span><span class="sxs-lookup"><span data-stu-id="afb7f-146">mail</span></span>             | <span data-ttu-id="afb7f-147">String</span><span class="sxs-lookup"><span data-stu-id="afb7f-147">String</span></span>             | <span data-ttu-id="afb7f-148">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="afb7f-148">email address</span></span>                                                                                                                                   |
| <span data-ttu-id="afb7f-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="afb7f-149">mobilePhone</span></span>      | <span data-ttu-id="afb7f-150">String</span><span class="sxs-lookup"><span data-stu-id="afb7f-150">String</span></span>             | <span data-ttu-id="afb7f-151">用户的移动电话号码</span><span class="sxs-lookup"><span data-stu-id="afb7f-151">Mobile number of user</span></span>                                                                                                                           |
| <span data-ttu-id="afb7f-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="afb7f-152">externalSource</span></span>   | <span data-ttu-id="afb7f-153">string</span><span class="sxs-lookup"><span data-stu-id="afb7f-153">string</span></span>             | <span data-ttu-id="afb7f-154">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="afb7f-154">Where this user was created from.</span></span> <span data-ttu-id="afb7f-155">可能的值包括： `sis` 、 `manual` 或 `lms` 。</span><span class="sxs-lookup"><span data-stu-id="afb7f-155">Possible values are: `sis`, `manual`, or `lms`.</span></span>                                                               |
| <span data-ttu-id="afb7f-156">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="afb7f-156">mailingAddress</span></span>   | <span data-ttu-id="afb7f-157">[physicalAddress]</span><span class="sxs-lookup"><span data-stu-id="afb7f-157">[physicalAddress]</span></span>  | <span data-ttu-id="afb7f-158">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="afb7f-158">Mail address of user.</span></span> <span data-ttu-id="afb7f-159">注意： `type` `postOfficeBox` 资源不支持和 `educationUser` 。</span><span class="sxs-lookup"><span data-stu-id="afb7f-159">Note: `type` and `postOfficeBox` are not supported for `educationUser` resources.</span></span>                                         |
| <span data-ttu-id="afb7f-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="afb7f-160">residenceAddress</span></span> | <span data-ttu-id="afb7f-161">[physicalAddress]</span><span class="sxs-lookup"><span data-stu-id="afb7f-161">[physicalAddress]</span></span>  | <span data-ttu-id="afb7f-162">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="afb7f-162">Address where user lives.</span></span> <span data-ttu-id="afb7f-163">注意： `type` `postOfficeBox` 资源不支持和 `educationUser` 。</span><span class="sxs-lookup"><span data-stu-id="afb7f-163">Note: `type` and `postOfficeBox` are not supported for `educationUser` resources.</span></span>                                     |
| <span data-ttu-id="afb7f-164">primaryRole</span><span class="sxs-lookup"><span data-stu-id="afb7f-164">primaryRole</span></span>      | <span data-ttu-id="afb7f-165">string</span><span class="sxs-lookup"><span data-stu-id="afb7f-165">string</span></span>             | <span data-ttu-id="afb7f-166">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="afb7f-166">Default Role for a user.</span></span> <span data-ttu-id="afb7f-167">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="afb7f-167">The user's role might be different in an individual class.</span></span> <span data-ttu-id="afb7f-168">可取值为：`student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="afb7f-168">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span> |
| <span data-ttu-id="afb7f-169">student</span><span class="sxs-lookup"><span data-stu-id="afb7f-169">student</span></span>          | <span data-ttu-id="afb7f-170">[educationStudent]</span><span class="sxs-lookup"><span data-stu-id="afb7f-170">[educationStudent]</span></span> | <span data-ttu-id="afb7f-171">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="afb7f-171">If the primary role is student, this block will contain student specific data.</span></span>                                                                  |
| <span data-ttu-id="afb7f-172">teacher</span><span class="sxs-lookup"><span data-stu-id="afb7f-172">teacher</span></span>          | [<span data-ttu-id="afb7f-173">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="afb7f-173">educationTeacher</span></span>](../resources/educationteacher.md) | <span data-ttu-id="afb7f-174">如果主要角色是教师，此块将包含教师特定的数据。</span><span class="sxs-lookup"><span data-stu-id="afb7f-174">If the primary role is teacher, this block will contain teacher specific data.</span></span>                                                                  |

## <a name="response"></a><span data-ttu-id="afb7f-175">响应</span><span class="sxs-lookup"><span data-stu-id="afb7f-175">Response</span></span>

<span data-ttu-id="afb7f-176">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afb7f-176">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb7f-177">示例</span><span class="sxs-lookup"><span data-stu-id="afb7f-177">Example</span></span>

##### <a name="request"></a><span data-ttu-id="afb7f-178">请求</span><span class="sxs-lookup"><span data-stu-id="afb7f-178">Request</span></span>

<span data-ttu-id="afb7f-179">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afb7f-179">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="afb7f-180">HTTP</span><span class="sxs-lookup"><span data-stu-id="afb7f-180">HTTP</span></span>](#tab/http)

<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}-->

```http
PATCH https://graph.microsoft.com/beta/education/users/13020
Content-type: application/json
Content-length: 508

{
  "displayName": "Rogelio Cazares",
  "givenName": "Rogelio",
  "middleName": "Fernando",
  "surname": "Cazares",
}
```

# <a name="c"></a>[<span data-ttu-id="afb7f-181">C#</span><span class="sxs-lookup"><span data-stu-id="afb7f-181">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="afb7f-182">JavaScript</span><span class="sxs-lookup"><span data-stu-id="afb7f-182">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="afb7f-183">Objective-C</span><span class="sxs-lookup"><span data-stu-id="afb7f-183">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="afb7f-184">响应</span><span class="sxs-lookup"><span data-stu-id="afb7f-184">Response</span></span>

<span data-ttu-id="afb7f-p109">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afb7f-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "primaryRole": "string",
  "residenceAddress": {
        "city": "Los Angeles",
        "countryOrRegion": "United States",
        "postalCode": "98055",
        "state": "CA",
        "street": "12345 Main St."
      },
  "student": {
      "primaryRole": "student",
      "externalId": "13005",
      "birthDate": "2001-01-01T00:00:00Z"
    }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->

[physicaladdress]: ../resources/physicaladdress.md
[educationstudent]: ../resources/educationstudent.md
