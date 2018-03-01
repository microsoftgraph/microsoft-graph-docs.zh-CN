# <a name="update-educationschool-properties"></a><span data-ttu-id="00090-101">更新 educationschool 属性</span><span class="sxs-lookup"><span data-stu-id="00090-101">Update educationschool properties</span></span>

<span data-ttu-id="00090-102">更新 school 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="00090-102">Update the properties of a contact object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00090-103">权限</span><span class="sxs-lookup"><span data-stu-id="00090-103">Permissions</span></span>
<span data-ttu-id="00090-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](../../../concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="00090-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="00090-106">权限类型</span><span class="sxs-lookup"><span data-stu-id="00090-106">Permission type</span></span>      | <span data-ttu-id="00090-107">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00090-107">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="00090-108">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00090-108">Delegated (work or school account)</span></span> |  <span data-ttu-id="00090-109">不支持。</span><span class="sxs-lookup"><span data-stu-id="00090-109">Not supported.</span></span>  |
|<span data-ttu-id="00090-110">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00090-110">Delegated (personal Microsoft account)</span></span> |  <span data-ttu-id="00090-111">不支持。</span><span class="sxs-lookup"><span data-stu-id="00090-111">Not supported.</span></span>  |
|<span data-ttu-id="00090-112">应用程序</span><span class="sxs-lookup"><span data-stu-id="00090-112">Application</span></span> | <span data-ttu-id="00090-113">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00090-113">EduRoster.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="00090-114">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00090-114">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /education/schools/{id}
```
## <a name="request-headers"></a><span data-ttu-id="00090-115">请求标头</span><span class="sxs-lookup"><span data-stu-id="00090-115">Request headers</span></span>
| <span data-ttu-id="00090-116">标头</span><span class="sxs-lookup"><span data-stu-id="00090-116">Header</span></span>       | <span data-ttu-id="00090-117">值</span><span class="sxs-lookup"><span data-stu-id="00090-117">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="00090-118">Authorization</span><span class="sxs-lookup"><span data-stu-id="00090-118">Authorization</span></span>  | <span data-ttu-id="00090-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00090-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="00090-121">Content-Type</span><span class="sxs-lookup"><span data-stu-id="00090-121">Content-Type</span></span>  | <span data-ttu-id="00090-122">application/json</span><span class="sxs-lookup"><span data-stu-id="00090-122">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="00090-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="00090-123">Request body</span></span>
<span data-ttu-id="00090-124">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="00090-124">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="00090-125">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="00090-125">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="00090-126">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="00090-126">For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="00090-127">属性</span><span class="sxs-lookup"><span data-stu-id="00090-127">Property</span></span>     | <span data-ttu-id="00090-128">类型</span><span class="sxs-lookup"><span data-stu-id="00090-128">Type</span></span>   |<span data-ttu-id="00090-129">说明</span><span class="sxs-lookup"><span data-stu-id="00090-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="00090-130">displayName</span><span class="sxs-lookup"><span data-stu-id="00090-130">displayName</span></span>| <span data-ttu-id="00090-131">String</span><span class="sxs-lookup"><span data-stu-id="00090-131">String</span></span>| <span data-ttu-id="00090-132">学校的显示名称</span><span class="sxs-lookup"><span data-stu-id="00090-132">Display name of the template.</span></span>| 
|<span data-ttu-id="00090-133">description</span><span class="sxs-lookup"><span data-stu-id="00090-133">description</span></span>| <span data-ttu-id="00090-134">String</span><span class="sxs-lookup"><span data-stu-id="00090-134">String</span></span> | <span data-ttu-id="00090-135">学校描述</span><span class="sxs-lookup"><span data-stu-id="00090-135">Description of the template.</span></span>| 
|<span data-ttu-id="00090-136">principalEmail</span><span class="sxs-lookup"><span data-stu-id="00090-136">principalEmail</span></span>| <span data-ttu-id="00090-137">String</span><span class="sxs-lookup"><span data-stu-id="00090-137">String</span></span>| <span data-ttu-id="00090-138">主体的电子邮件地址</span><span class="sxs-lookup"><span data-stu-id="00090-138">Email address of the principal</span></span>|
|<span data-ttu-id="00090-139">principalName</span><span class="sxs-lookup"><span data-stu-id="00090-139">PrincipalName</span></span>| <span data-ttu-id="00090-140">String</span><span class="sxs-lookup"><span data-stu-id="00090-140">String</span></span> | <span data-ttu-id="00090-141">主体名称</span><span class="sxs-lookup"><span data-stu-id="00090-141">Name of the principal</span></span>|
|<span data-ttu-id="00090-142">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="00090-142">externalPrincipalId</span></span>| <span data-ttu-id="00090-143">String</span><span class="sxs-lookup"><span data-stu-id="00090-143">String</span></span> | <span data-ttu-id="00090-144">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="00090-144">Id of principal in syncing system.</span></span> |
|<span data-ttu-id="00090-145">highestGrade</span><span class="sxs-lookup"><span data-stu-id="00090-145">highestGrade</span></span>|<span data-ttu-id="00090-146">String</span><span class="sxs-lookup"><span data-stu-id="00090-146">String</span></span>| <span data-ttu-id="00090-147">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="00090-147">Highest grade taught.</span></span> |
|<span data-ttu-id="00090-148">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="00090-148">lowestGrade</span></span>|<span data-ttu-id="00090-149">String</span><span class="sxs-lookup"><span data-stu-id="00090-149">String</span></span>| <span data-ttu-id="00090-150">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="00090-150">Lowest grade taught.</span></span> |
|<span data-ttu-id="00090-151">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="00090-151">schoolNumber</span></span>|<span data-ttu-id="00090-152">String</span><span class="sxs-lookup"><span data-stu-id="00090-152">String</span></span>| <span data-ttu-id="00090-153">学校编号。</span><span class="sxs-lookup"><span data-stu-id="00090-153">School Number.</span></span>|
|<span data-ttu-id="00090-154">externalId</span><span class="sxs-lookup"><span data-stu-id="00090-154">externalId</span></span>|<span data-ttu-id="00090-155">String</span><span class="sxs-lookup"><span data-stu-id="00090-155">String</span></span>| <span data-ttu-id="00090-156">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="00090-156">Id of school in syncing system.</span></span> |
|<span data-ttu-id="00090-157">phone</span><span class="sxs-lookup"><span data-stu-id="00090-157">Phone</span></span>|<span data-ttu-id="00090-158">String</span><span class="sxs-lookup"><span data-stu-id="00090-158">String</span></span>| <span data-ttu-id="00090-159">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="00090-159">Phone number of school.</span></span> |
|<span data-ttu-id="00090-160">fax</span><span class="sxs-lookup"><span data-stu-id="00090-160">fax</span></span>|<span data-ttu-id="00090-161">String</span><span class="sxs-lookup"><span data-stu-id="00090-161">String</span></span>| <span data-ttu-id="00090-162">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="00090-162">Fax number of school.</span></span> |
|<span data-ttu-id="00090-163">address</span><span class="sxs-lookup"><span data-stu-id="00090-163">address</span></span>|[<span data-ttu-id="00090-164">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="00090-164">physicalAddress</span></span>](../resources/physicaladdress.md)| <span data-ttu-id="00090-165">学校地址。</span><span class="sxs-lookup"><span data-stu-id="00090-165">Address of the School.</span></span>|
|<span data-ttu-id="00090-166">createdBy</span><span class="sxs-lookup"><span data-stu-id="00090-166">createdBy</span></span>|[<span data-ttu-id="00090-167">identitySet</span><span class="sxs-lookup"><span data-stu-id="00090-167">identitySet</span></span>](../resources/identityset.md)|<span data-ttu-id="00090-168">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="00090-168">Entity who created the school.</span></span>|

## <a name="response"></a><span data-ttu-id="00090-169">响应</span><span class="sxs-lookup"><span data-stu-id="00090-169">Response</span></span>
<span data-ttu-id="00090-170">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和更新的 [educationSchool](../resources/educationschool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00090-170">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/educationschool.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="00090-171">示例</span><span class="sxs-lookup"><span data-stu-id="00090-171">Example</span></span>
##### <a name="request"></a><span data-ttu-id="00090-172">请求</span><span class="sxs-lookup"><span data-stu-id="00090-172">Request</span></span>
<span data-ttu-id="00090-173">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="00090-173">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_educationschool"
}-->
```http
PATCH https://graph.microsoft.com/v1.0/education/schools/10002
Content-type: application/json
Content-length: 292

{
  "displayName": "Fabrikam Arts High School",
  "description": "Magnate school for the arts. Los Angeles School District"
}
```
##### <a name="response"></a><span data-ttu-id="00090-174">响应</span><span class="sxs-lookup"><span data-stu-id="00090-174">Response</span></span>
<span data-ttu-id="00090-175">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="00090-175">The following is an example of the response.</span></span> 

><span data-ttu-id="00090-p104">**注意：**为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="00090-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
