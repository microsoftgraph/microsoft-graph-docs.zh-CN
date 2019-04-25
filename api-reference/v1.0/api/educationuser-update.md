---
title: 更新 educationUser 属性
description: 更新 **educationuser** 对象的属性。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 0c93ecd601e941cd68f0b6f8d668775e7de3feef
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32550040"
---
# <a name="update-educationuser-properties"></a><span data-ttu-id="00256-103">更新 educationUser 属性</span><span class="sxs-lookup"><span data-stu-id="00256-103">Update educationUser properties</span></span>

<span data-ttu-id="00256-104">更新 **educationuser** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00256-104">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="00256-105">权限</span><span class="sxs-lookup"><span data-stu-id="00256-105">Permissions</span></span>
<span data-ttu-id="00256-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00256-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00256-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="00256-108">Permission type</span></span>      | <span data-ttu-id="00256-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00256-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00256-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00256-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="00256-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="00256-111">Not supported.</span></span>  |
|<span data-ttu-id="00256-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00256-112">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="00256-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="00256-113">Not supported.</span></span>  |
|<span data-ttu-id="00256-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="00256-114">Application</span></span> | <span data-ttu-id="00256-115">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00256-115">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00256-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00256-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00256-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="00256-117">Request headers</span></span>
| <span data-ttu-id="00256-118">标头</span><span class="sxs-lookup"><span data-stu-id="00256-118">Header</span></span>       | <span data-ttu-id="00256-119">值</span><span class="sxs-lookup"><span data-stu-id="00256-119">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00256-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="00256-120">Authorization</span></span>  | <span data-ttu-id="00256-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00256-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00256-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00256-123">Content-Type</span></span>  | <span data-ttu-id="00256-124">application/json</span><span class="sxs-lookup"><span data-stu-id="00256-124">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00256-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="00256-125">Request body</span></span>
<span data-ttu-id="00256-126">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="00256-126">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="00256-127">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="00256-127">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="00256-128">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="00256-128">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="00256-129">属性</span><span class="sxs-lookup"><span data-stu-id="00256-129">Property</span></span>     | <span data-ttu-id="00256-130">类型</span><span class="sxs-lookup"><span data-stu-id="00256-130">Type</span></span>   |<span data-ttu-id="00256-131">说明</span><span class="sxs-lookup"><span data-stu-id="00256-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00256-132">displayName</span><span class="sxs-lookup"><span data-stu-id="00256-132">displayName</span></span>| <span data-ttu-id="00256-133">String</span><span class="sxs-lookup"><span data-stu-id="00256-133">String</span></span>| <span data-ttu-id="00256-134">显示用户名称</span><span class="sxs-lookup"><span data-stu-id="00256-134">Display Name of User</span></span>|
|<span data-ttu-id="00256-135">givenName</span><span class="sxs-lookup"><span data-stu-id="00256-135">givenName</span></span>| <span data-ttu-id="00256-136">String</span><span class="sxs-lookup"><span data-stu-id="00256-136">String</span></span> | <span data-ttu-id="00256-137">名字</span><span class="sxs-lookup"><span data-stu-id="00256-137">First Name</span></span> |
|<span data-ttu-id="00256-138">middleName</span><span class="sxs-lookup"><span data-stu-id="00256-138">middleName</span></span>| <span data-ttu-id="00256-139">String</span><span class="sxs-lookup"><span data-stu-id="00256-139">String</span></span> | <span data-ttu-id="00256-140">用户的中间名</span><span class="sxs-lookup"><span data-stu-id="00256-140">Middle Name of user</span></span>|
|<span data-ttu-id="00256-141">surname</span><span class="sxs-lookup"><span data-stu-id="00256-141">surname</span></span>| <span data-ttu-id="00256-142">String</span><span class="sxs-lookup"><span data-stu-id="00256-142">String</span></span> | <span data-ttu-id="00256-143">用户的姓</span><span class="sxs-lookup"><span data-stu-id="00256-143">Surname of user</span></span>|
|<span data-ttu-id="00256-144">mail</span><span class="sxs-lookup"><span data-stu-id="00256-144">mail</span></span>| <span data-ttu-id="00256-145">String</span><span class="sxs-lookup"><span data-stu-id="00256-145">String</span></span>| <span data-ttu-id="00256-146">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="00256-146">email address</span></span>|
|<span data-ttu-id="00256-147">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="00256-147">mobilePhone</span></span>| <span data-ttu-id="00256-148">String</span><span class="sxs-lookup"><span data-stu-id="00256-148">String</span></span> | <span data-ttu-id="00256-149">用户的移动电话号码</span><span class="sxs-lookup"><span data-stu-id="00256-149">Mobile number of user</span></span> |
|<span data-ttu-id="00256-150">externalSource</span><span class="sxs-lookup"><span data-stu-id="00256-150">externalSource</span></span>|<span data-ttu-id="00256-151">string</span><span class="sxs-lookup"><span data-stu-id="00256-151">string</span></span>| <span data-ttu-id="00256-152">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="00256-152">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="00256-153">externalSource</span><span class="sxs-lookup"><span data-stu-id="00256-153">externalSource</span></span>|<span data-ttu-id="00256-154">string</span><span class="sxs-lookup"><span data-stu-id="00256-154">string</span></span>| <span data-ttu-id="00256-155">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="00256-155">Where this user was created from.</span></span>  <span data-ttu-id="00256-156">可能的值包括 `sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="00256-156">The possible values are: `sis`, `manual`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="00256-157">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="00256-157">mailingAddress</span></span>|[<span data-ttu-id="00256-158">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="00256-158">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="00256-159">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="00256-159">Mail address of user.</span></span>|
|<span data-ttu-id="00256-160">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="00256-160">residenceAddress</span></span>|[<span data-ttu-id="00256-161">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="00256-161">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="00256-162">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="00256-162">Address where user lives.</span></span>|
|<span data-ttu-id="00256-163">primaryRole</span><span class="sxs-lookup"><span data-stu-id="00256-163">primaryRole</span></span>|<span data-ttu-id="00256-164">string</span><span class="sxs-lookup"><span data-stu-id="00256-164">string</span></span>| <span data-ttu-id="00256-165">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="00256-165">Default Role for a user.</span></span>  <span data-ttu-id="00256-166">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="00256-166">The user's role might be different in an individual class.</span></span> <span data-ttu-id="00256-167">可能的值包括 `student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="00256-167">The possible values are: `student`, `teacher`, `enum_sentinel`.</span></span>|
|<span data-ttu-id="00256-168">student</span><span class="sxs-lookup"><span data-stu-id="00256-168">student</span></span>|[<span data-ttu-id="00256-169">educationStudent</span><span class="sxs-lookup"><span data-stu-id="00256-169">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="00256-170">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="00256-170">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="00256-171">teacher</span><span class="sxs-lookup"><span data-stu-id="00256-171">teacher</span></span>|[<span data-ttu-id="00256-172">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="00256-172">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="00256-173">如果主要角色为教师，此部分将包含特定于教师的数据。</span><span class="sxs-lookup"><span data-stu-id="00256-173">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="00256-174">响应</span><span class="sxs-lookup"><span data-stu-id="00256-174">Response</span></span>
<span data-ttu-id="00256-175">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00256-175">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00256-176">示例</span><span class="sxs-lookup"><span data-stu-id="00256-176">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00256-177">请求</span><span class="sxs-lookup"><span data-stu-id="00256-177">Request</span></span>
<span data-ttu-id="00256-178">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="00256-178">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="00256-179">响应</span><span class="sxs-lookup"><span data-stu-id="00256-179">Response</span></span>
<span data-ttu-id="00256-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="00256-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "tocPath": ""
}-->
