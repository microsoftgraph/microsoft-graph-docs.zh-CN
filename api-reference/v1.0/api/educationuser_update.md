# <a name="update-educationuser-properties"></a><span data-ttu-id="233ca-101">更新 educationUser 属性</span><span class="sxs-lookup"><span data-stu-id="233ca-101">Update educationUser properties</span></span>

<span data-ttu-id="233ca-102">更新 **educationuser** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="233ca-102">Update the properties of an **educationuser** object.</span></span>
## <a name="permissions"></a><span data-ttu-id="233ca-103">权限</span><span class="sxs-lookup"><span data-stu-id="233ca-103">Permissions</span></span>
<span data-ttu-id="233ca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="233ca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="233ca-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="233ca-106">Permission type</span></span>      | <span data-ttu-id="233ca-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="233ca-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="233ca-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="233ca-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="233ca-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="233ca-109">Not supported.</span></span>  |
|<span data-ttu-id="233ca-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="233ca-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="233ca-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="233ca-111">Not supported.</span></span>  |
|<span data-ttu-id="233ca-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="233ca-112">Application</span></span> | <span data-ttu-id="233ca-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="233ca-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="233ca-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="233ca-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/me
PATCH /education/users/{id}
```
## <a name="request-headers"></a><span data-ttu-id="233ca-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="233ca-115">Request headers</span></span>
| <span data-ttu-id="233ca-116">标头</span><span class="sxs-lookup"><span data-stu-id="233ca-116">Header</span></span>       | <span data-ttu-id="233ca-117">值</span><span class="sxs-lookup"><span data-stu-id="233ca-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="233ca-118">授权</span><span class="sxs-lookup"><span data-stu-id="233ca-118">Authorization</span></span>  | <span data-ttu-id="233ca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="233ca-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="233ca-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="233ca-121">Content-Type</span></span>  | <span data-ttu-id="233ca-122">application/json</span><span class="sxs-lookup"><span data-stu-id="233ca-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="233ca-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="233ca-123">Request body</span></span>
<span data-ttu-id="233ca-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="233ca-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="233ca-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="233ca-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="233ca-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="233ca-126">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="233ca-127">属性</span><span class="sxs-lookup"><span data-stu-id="233ca-127">Property</span></span>     | <span data-ttu-id="233ca-128">类型</span><span class="sxs-lookup"><span data-stu-id="233ca-128">Type</span></span>   |<span data-ttu-id="233ca-129">说明</span><span class="sxs-lookup"><span data-stu-id="233ca-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="233ca-130">displayName</span><span class="sxs-lookup"><span data-stu-id="233ca-130">displayName</span></span>| <span data-ttu-id="233ca-131">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-131">String</span></span>| <span data-ttu-id="233ca-132">显示用户名称</span><span class="sxs-lookup"><span data-stu-id="233ca-132">Display Name of User</span></span>|
|<span data-ttu-id="233ca-133">givenName</span><span class="sxs-lookup"><span data-stu-id="233ca-133">givenName</span></span>| <span data-ttu-id="233ca-134">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-134">String</span></span> | <span data-ttu-id="233ca-135">名字</span><span class="sxs-lookup"><span data-stu-id="233ca-135">First Name</span></span> |
|<span data-ttu-id="233ca-136">middleName</span><span class="sxs-lookup"><span data-stu-id="233ca-136">middleName</span></span>| <span data-ttu-id="233ca-137">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-137">String</span></span> | <span data-ttu-id="233ca-138">用户的中间名</span><span class="sxs-lookup"><span data-stu-id="233ca-138">Middle Name of user</span></span>|
|<span data-ttu-id="233ca-139">姓氏</span><span class="sxs-lookup"><span data-stu-id="233ca-139">surname</span></span>| <span data-ttu-id="233ca-140">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-140">String</span></span> | <span data-ttu-id="233ca-141">用户的姓</span><span class="sxs-lookup"><span data-stu-id="233ca-141">Surname of user</span></span>|
|<span data-ttu-id="233ca-142">邮件</span><span class="sxs-lookup"><span data-stu-id="233ca-142">mail</span></span>| <span data-ttu-id="233ca-143">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-143">String</span></span>| <span data-ttu-id="233ca-144">电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="233ca-144">email address</span></span>|
|<span data-ttu-id="233ca-145">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="233ca-145">mobilePhone</span></span>| <span data-ttu-id="233ca-146">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-146">String</span></span> | <span data-ttu-id="233ca-147">用户的移动电话号码</span><span class="sxs-lookup"><span data-stu-id="233ca-147">Mobile number of user</span></span> |
|<span data-ttu-id="233ca-148">externalSource</span><span class="sxs-lookup"><span data-stu-id="233ca-148">externalSource</span></span>|<span data-ttu-id="233ca-149">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-149">string</span></span>| <span data-ttu-id="233ca-150">可取值为：`sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="233ca-150">The possible values are `sis`, `manual`, `enum_sentinel`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="233ca-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="233ca-151">externalSource</span></span>|<span data-ttu-id="233ca-152">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-152">string</span></span>| <span data-ttu-id="233ca-153">创建此用户的位置。</span><span class="sxs-lookup"><span data-stu-id="233ca-153">Where this user was created from.</span></span>  <span data-ttu-id="233ca-154">可取值为：`sis`、`manual`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="233ca-154">The possible values are `sis`, `manual`, `enum_sentinel`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="233ca-155">mailingAddress</span><span class="sxs-lookup"><span data-stu-id="233ca-155">mailingAddress</span></span>|[<span data-ttu-id="233ca-156">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="233ca-156">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="233ca-157">用户的邮件地址。</span><span class="sxs-lookup"><span data-stu-id="233ca-157">Mail address of user.</span></span>|
|<span data-ttu-id="233ca-158">residenceAddress</span><span class="sxs-lookup"><span data-stu-id="233ca-158">residenceAddress</span></span>|[<span data-ttu-id="233ca-159">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="233ca-159">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="233ca-160">用户所在的地址。</span><span class="sxs-lookup"><span data-stu-id="233ca-160">Address where user lives.</span></span>|
|<span data-ttu-id="233ca-161">primaryRole</span><span class="sxs-lookup"><span data-stu-id="233ca-161">primaryRole</span></span>|<span data-ttu-id="233ca-162">字符串</span><span class="sxs-lookup"><span data-stu-id="233ca-162">string</span></span>| <span data-ttu-id="233ca-163">用户的默认角色。</span><span class="sxs-lookup"><span data-stu-id="233ca-163">Default Role for a user.</span></span>  <span data-ttu-id="233ca-164">用户的角色在各课程中可能有所不同。</span><span class="sxs-lookup"><span data-stu-id="233ca-164">The user's role might be different in an individual class.</span></span> <span data-ttu-id="233ca-165">可取值为：`student`、`teacher`、`enum_sentinel`。</span><span class="sxs-lookup"><span data-stu-id="233ca-165">The possible values are `student`, `teacher`, `enum_sentinel`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="233ca-166">学生</span><span class="sxs-lookup"><span data-stu-id="233ca-166">student</span></span>|[<span data-ttu-id="233ca-167">educationStudent</span><span class="sxs-lookup"><span data-stu-id="233ca-167">educationStudent</span></span>](../resources/educationstudent.md)| <span data-ttu-id="233ca-168">如果主要角色为学生，此部分将包含特定于学生的数据。</span><span class="sxs-lookup"><span data-stu-id="233ca-168">If the primary role is student, this block will contain student specific data.</span></span>|
|<span data-ttu-id="233ca-169">教师</span><span class="sxs-lookup"><span data-stu-id="233ca-169">teacher</span></span>|[<span data-ttu-id="233ca-170">educationTeacher</span><span class="sxs-lookup"><span data-stu-id="233ca-170">educationTeacher</span></span>](../resources/educationteacher.md)| <span data-ttu-id="233ca-171">如果主要角色为教师，此部分将包含特定于教师的数据。</span><span class="sxs-lookup"><span data-stu-id="233ca-171">If the primary role is teacher, this block will conatin teacher specific data.</span></span>|


## <a name="response"></a><span data-ttu-id="233ca-172">响应</span><span class="sxs-lookup"><span data-stu-id="233ca-172">Response</span></span>
<span data-ttu-id="233ca-173">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="233ca-173">If successful, this method returns a `200 OK` response code and updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="233ca-174">示例</span><span class="sxs-lookup"><span data-stu-id="233ca-174">Example</span></span>
##### <a name="request"></a><span data-ttu-id="233ca-175">请求</span><span class="sxs-lookup"><span data-stu-id="233ca-175">Request</span></span>
<span data-ttu-id="233ca-176">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="233ca-176">Here is an example of the request.</span></span>
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
##### <a name="response"></a><span data-ttu-id="233ca-177">响应</span><span class="sxs-lookup"><span data-stu-id="233ca-177">Response</span></span>
<span data-ttu-id="233ca-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="233ca-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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