---
title: 更新 educationUser 属性
description: 更新 **educationuser** 对象的属性。
localization_priority: Normal
ms.openlocfilehash: a6479095abbb1884acf98377e8fef9d115d4a6c2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843510"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="6aad6-103">更新 educationUser 属性</span><span class="sxs-lookup"><span data-stu-id="6aad6-103">Update educationUser properties</span></span>

> <span data-ttu-id="6aad6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6aad6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6aad6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6aad6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6aad6-106">更新 **educationuser** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6aad6-106">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="6aad6-107">权限</span><span class="sxs-lookup"><span data-stu-id="6aad6-107">Permissions</span></span>
<span data-ttu-id="6aad6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6aad6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6aad6-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="6aad6-110">Permission type</span></span>      | <span data-ttu-id="6aad6-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6aad6-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6aad6-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6aad6-112">Delegated (work or school account)</span></span> |  <span data-ttu-id="6aad6-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aad6-113">Not supported.</span></span>  |
|<span data-ttu-id="6aad6-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6aad6-114">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="6aad6-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="6aad6-115">Not supported.</span></span>  |
|<span data-ttu-id="6aad6-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="6aad6-116">Application</span></span> | <span data-ttu-id="6aad6-117">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6aad6-117">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6aad6-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6aad6-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="6aad6-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="6aad6-119">Request headers</span></span>
| <span data-ttu-id="6aad6-120">标头</span><span class="sxs-lookup"><span data-stu-id="6aad6-120">Header</span></span>       | <span data-ttu-id="6aad6-121">值</span><span class="sxs-lookup"><span data-stu-id="6aad6-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="6aad6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6aad6-122">Authorization</span></span>  | <span data-ttu-id="6aad6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6aad6-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="6aad6-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="6aad6-125">Content-Type</span></span>  | <span data-ttu-id="6aad6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6aad6-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="6aad6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6aad6-127">Request body</span></span>
<span data-ttu-id="6aad6-128">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="6aad6-128">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="6aad6-129">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="6aad6-129">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="6aad6-130">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="6aad6-130">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="6aad6-131">属性</span><span class="sxs-lookup"><span data-stu-id="6aad6-131">Property</span></span>     | <span data-ttu-id="6aad6-132">类型</span><span class="sxs-lookup"><span data-stu-id="6aad6-132">Type</span></span>   |<span data-ttu-id="6aad6-133">说明</span><span class="sxs-lookup"><span data-stu-id="6aad6-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6aad6-134">displayName</span><span class="sxs-lookup"><span data-stu-id="6aad6-134">displayName</span></span>| <span data-ttu-id="6aad6-135">String</span><span class="sxs-lookup"><span data-stu-id="6aad6-135">String</span></span>| <span data-ttu-id="6aad6-136">显示用户名称</span><span class="sxs-lookup"><span data-stu-id="6aad6-136">Display Name of User</span></span>|
|<span data-ttu-id="6aad6-137">givenName</span><span class="sxs-lookup"><span data-stu-id="6aad6-137">givenName</span></span>| <span data-ttu-id="6aad6-138">String</span><span class="sxs-lookup"><span data-stu-id="6aad6-138">String</span></span> | <span data-ttu-id="6aad6-139">名字</span><span class="sxs-lookup"><span data-stu-id="6aad6-139">First Name</span></span> |
|<span data-ttu-id="6aad6-140">middleName</span><span class="sxs-lookup"><span data-stu-id="6aad6-140">middleName</span></span>| <span data-ttu-id="6aad6-141">String</span><span class="sxs-lookup"><span data-stu-id="6aad6-141">String</span></span> | <span data-ttu-id="6aad6-142">用户的中间名</span><span class="sxs-lookup"><span data-stu-id="6aad6-142">Middle Name of user</span></span>|
|<span data-ttu-id="6aad6-143">surname</span><span class="sxs-lookup"><span data-stu-id="6aad6-143">surname</span></span>| <span data-ttu-id="6aad6-144">String</span><span class="sxs-lookup"><span data-stu-id="6aad6-144">String</span></span> | <span data-ttu-id="6aad6-145">用户的姓</span><span class="sxs-lookup"><span data-stu-id="6aad6-145">Surname of user</span></span>|
|<span data-ttu-id="6aad6-146">mail</span><span class="sxs-lookup"><span data-stu-id="6aad6-146">mail</span></span>| <span data-ttu-id="6aad6-147">String</span><span class="sxs-lookup"><span data-stu-id="6aad6-147">String</span></span>| <span data-ttu-id="6aad6-148">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="6aad6-148">email address</span></span>|
|<span data-ttu-id="6aad6-149">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="6aad6-149">mobilePhone</span></span>| <span data-ttu-id="6aad6-150">String</span><span class="sxs-lookup"><span data-stu-id="6aad6-150">String</span></span> | <span data-ttu-id="6aad6-151">用户的移动电话号码</span><span class="sxs-lookup"><span data-stu-id="6aad6-151">Mobile number of user</span></span> |
|<span data-ttu-id="6aad6-152">externalSource</span><span class="sxs-lookup"><span data-stu-id="6aad6-152">externalSource</span></span>|<span data-ttu-id="6aad6-153">string</span><span class="sxs-lookup"><span data-stu-id="6aad6-153">string</span></span>| <span data-ttu-id="6aad6-154">可取值为：`sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="6aad6-154">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="6aad6-155">externalSource</span><span class="sxs-lookup"><span data-stu-id="6aad6-155">externalSource</span></span>|<span data-ttu-id="6aad6-156">string</span><span class="sxs-lookup"><span data-stu-id="6aad6-156">string</span></span>| <span data-ttu-id="6aad6-157">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="6aad6-157">Where this user was created from.</span></span>  <span data-ttu-id="6aad6-158">可取值为：`sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="6aad6-158">Possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="6aad6-159">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="6aad6-159">mailingAddress</span></span>|[<span data-ttu-id="6aad6-160">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6aad6-160">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="6aad6-161">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="6aad6-161">Mail address of user.</span></span>|
|<span data-ttu-id="6aad6-162">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="6aad6-162">residenceAddress</span></span>|[<span data-ttu-id="6aad6-163">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="6aad6-163">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="6aad6-164">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="6aad6-164">Address where user lives.</span></span>|
|<span data-ttu-id="6aad6-165">primaryRole</span><span class="sxs-lookup"><span data-stu-id="6aad6-165">primaryRole</span></span>|<span data-ttu-id="6aad6-166">string</span><span class="sxs-lookup"><span data-stu-id="6aad6-166">string</span></span>| <span data-ttu-id="6aad6-167">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="6aad6-167">Default Role for a user.</span></span>  <span data-ttu-id="6aad6-168">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="6aad6-168">The user's role might be different in an individual class.</span></span> <span data-ttu-id="6aad6-169">可取值为：`student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="6aad6-169">Possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="6aad6-170">student</span><span class="sxs-lookup"><span data-stu-id="6aad6-170">student</span></span>|[<span data-ttu-id="6aad6-171">educationStudent</span><span class="sxs-lookup"><span data-stu-id="6aad6-171">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="6aad6-172">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="6aad6-172">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="6aad6-173">teacher</span><span class="sxs-lookup"><span data-stu-id="6aad6-173">teacher</span></span>|[<span data-ttu-id="6aad6-174">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="6aad6-174">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="6aad6-175">如果主要角色为教师，此部分将包含特定于教师的数据。</span><span class="sxs-lookup"><span data-stu-id="6aad6-175">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="6aad6-176">响应</span><span class="sxs-lookup"><span data-stu-id="6aad6-176">Response</span></span>
<span data-ttu-id="6aad6-177">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6aad6-177">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="6aad6-178">示例</span><span class="sxs-lookup"><span data-stu-id="6aad6-178">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6aad6-179">请求</span><span class="sxs-lookup"><span data-stu-id="6aad6-179">Request</span></span>
<span data-ttu-id="6aad6-180">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6aad6-180">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="6aad6-181">响应</span><span class="sxs-lookup"><span data-stu-id="6aad6-181">Response</span></span>
<span data-ttu-id="6aad6-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6aad6-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "Update educationuser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
