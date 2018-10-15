# <a name="educationschool-resource-type"></a><span data-ttu-id="94fa5-101">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="94fa5-101">educationSchool resource type</span></span>

<span data-ttu-id="94fa5-102">一种表示学校的资源，用于管理所表示学校的课程、教师和学生。</span><span class="sxs-lookup"><span data-stu-id="94fa5-102">A resource representing a school and used to manage the classes, teachers, and students of the represented school.</span></span>  


## <a name="methods"></a><span data-ttu-id="94fa5-103">方法</span><span class="sxs-lookup"><span data-stu-id="94fa5-103">Methods</span></span>

| <span data-ttu-id="94fa5-104">方法</span><span class="sxs-lookup"><span data-stu-id="94fa5-104">Method</span></span>           | <span data-ttu-id="94fa5-105">返回类型</span><span class="sxs-lookup"><span data-stu-id="94fa5-105">Return Type</span></span>    |<span data-ttu-id="94fa5-106">说明</span><span class="sxs-lookup"><span data-stu-id="94fa5-106">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="94fa5-107">Get</span><span class="sxs-lookup"><span data-stu-id="94fa5-107">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="94fa5-108">educationSchool</span><span class="sxs-lookup"><span data-stu-id="94fa5-108">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="94fa5-109">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="94fa5-109">Read properties and relationships of an **educationSchool** object.</span></span>|
|[<span data-ttu-id="94fa5-110">Add class</span><span class="sxs-lookup"><span data-stu-id="94fa5-110">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="94fa5-111">educationClass</span><span class="sxs-lookup"><span data-stu-id="94fa5-111">educationClass</span></span>](educationclass.md)| <span data-ttu-id="94fa5-112">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="94fa5-112">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="94fa5-113">List classes</span><span class="sxs-lookup"><span data-stu-id="94fa5-113">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="94fa5-114">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94fa5-114">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="94fa5-115">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="94fa5-115">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="94fa5-116">Remove class</span><span class="sxs-lookup"><span data-stu-id="94fa5-116">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="94fa5-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="94fa5-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="94fa5-118">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="94fa5-118">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="94fa5-119">Add user</span><span class="sxs-lookup"><span data-stu-id="94fa5-119">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="94fa5-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="94fa5-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="94fa5-121">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="94fa5-121">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="94fa5-122">List users</span><span class="sxs-lookup"><span data-stu-id="94fa5-122">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="94fa5-123">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94fa5-123">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="94fa5-124">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="94fa5-124">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="94fa5-125">Remove user</span><span class="sxs-lookup"><span data-stu-id="94fa5-125">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="94fa5-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="94fa5-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="94fa5-127">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="94fa5-127">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="94fa5-128">Update</span><span class="sxs-lookup"><span data-stu-id="94fa5-128">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="94fa5-129">educationSchool</span><span class="sxs-lookup"><span data-stu-id="94fa5-129">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="94fa5-130">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="94fa5-130">Update an **educationSchool** object.</span></span> |
|[<span data-ttu-id="94fa5-131">Delete</span><span class="sxs-lookup"><span data-stu-id="94fa5-131">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="94fa5-132">无</span><span class="sxs-lookup"><span data-stu-id="94fa5-132">None</span></span> |<span data-ttu-id="94fa5-133">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="94fa5-133">Delete an **educationSchool** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="94fa5-134">属性</span><span class="sxs-lookup"><span data-stu-id="94fa5-134">Properties</span></span>
| <span data-ttu-id="94fa5-135">属性</span><span class="sxs-lookup"><span data-stu-id="94fa5-135">Property</span></span>     | <span data-ttu-id="94fa5-136">类型</span><span class="sxs-lookup"><span data-stu-id="94fa5-136">Type</span></span>   |<span data-ttu-id="94fa5-137">说明</span><span class="sxs-lookup"><span data-stu-id="94fa5-137">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94fa5-138">id</span><span class="sxs-lookup"><span data-stu-id="94fa5-138">id</span></span>|<span data-ttu-id="94fa5-139">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-139">String</span></span>|<span data-ttu-id="94fa5-140">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="94fa5-140">GUID of this school.</span></span>|
|<span data-ttu-id="94fa5-141">displayName</span><span class="sxs-lookup"><span data-stu-id="94fa5-141">displayName</span></span>| <span data-ttu-id="94fa5-142">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-142">String</span></span>| <span data-ttu-id="94fa5-143">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="94fa5-143">Display name of the school.</span></span>| 
|<span data-ttu-id="94fa5-144">description</span><span class="sxs-lookup"><span data-stu-id="94fa5-144">description</span></span>| <span data-ttu-id="94fa5-145">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-145">String</span></span> | <span data-ttu-id="94fa5-146">学校描述。</span><span class="sxs-lookup"><span data-stu-id="94fa5-146">Description of the school.</span></span>| 
|<span data-ttu-id="94fa5-147">status</span><span class="sxs-lookup"><span data-stu-id="94fa5-147">status</span></span>| <span data-ttu-id="94fa5-148">string</span><span class="sxs-lookup"><span data-stu-id="94fa5-148">string</span></span>| <span data-ttu-id="94fa5-149">只读。</span><span class="sxs-lookup"><span data-stu-id="94fa5-149">Read-Only.</span></span> <span data-ttu-id="94fa5-150">可取值为：`inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="94fa5-150">The possible values are `inactive`, `active`, `expired`, `deleteable`, , , , , , , , or .</span></span>|
|<span data-ttu-id="94fa5-151">externalSource</span><span class="sxs-lookup"><span data-stu-id="94fa5-151">externalSource</span></span>| <span data-ttu-id="94fa5-152">educationExternalSource</span><span class="sxs-lookup"><span data-stu-id="94fa5-152">educationExternalSource</span></span>| <span data-ttu-id="94fa5-153">只读。</span><span class="sxs-lookup"><span data-stu-id="94fa5-153">Read-Only.</span></span>  <span data-ttu-id="94fa5-154">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="94fa5-154">The possible values are `sis`, `manual`, `unknownFutureValue`, , , , , , , , , or .</span></span>|
|<span data-ttu-id="94fa5-155">principalEmail</span><span class="sxs-lookup"><span data-stu-id="94fa5-155">principalEmail</span></span>| <span data-ttu-id="94fa5-156">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-156">String</span></span>| <span data-ttu-id="94fa5-157">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="94fa5-157">Email address of the principal.</span></span>|
|<span data-ttu-id="94fa5-158">principalName</span><span class="sxs-lookup"><span data-stu-id="94fa5-158">principalName</span></span>| <span data-ttu-id="94fa5-159">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-159">String</span></span> | <span data-ttu-id="94fa5-160">主体名称。</span><span class="sxs-lookup"><span data-stu-id="94fa5-160">Name of the principal.</span></span>|
|<span data-ttu-id="94fa5-161">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="94fa5-161">externalPrincipalId</span></span>| <span data-ttu-id="94fa5-162">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-162">String</span></span> | <span data-ttu-id="94fa5-163">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="94fa5-163">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="94fa5-164">highestGrade</span><span class="sxs-lookup"><span data-stu-id="94fa5-164">highestGrade</span></span>|<span data-ttu-id="94fa5-165">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-165">String</span></span>| <span data-ttu-id="94fa5-166">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="94fa5-166">Highest grade taught.</span></span> |
|<span data-ttu-id="94fa5-167">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="94fa5-167">lowestGrade</span></span>|<span data-ttu-id="94fa5-168">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-168">String</span></span>| <span data-ttu-id="94fa5-169">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="94fa5-169">Lowest grade taught.</span></span> |
|<span data-ttu-id="94fa5-170">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="94fa5-170">schoolNumber</span></span>|<span data-ttu-id="94fa5-171">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-171">String</span></span>| <span data-ttu-id="94fa5-172">学校编号。</span><span class="sxs-lookup"><span data-stu-id="94fa5-172">School Number.</span></span>|
|<span data-ttu-id="94fa5-173">externalId</span><span class="sxs-lookup"><span data-stu-id="94fa5-173">externalId</span></span>|<span data-ttu-id="94fa5-174">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-174">String</span></span>| <span data-ttu-id="94fa5-175">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="94fa5-175">ID of school in syncing system.</span></span> |
|<span data-ttu-id="94fa5-176">phone</span><span class="sxs-lookup"><span data-stu-id="94fa5-176">phone</span></span>|<span data-ttu-id="94fa5-177">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-177">String</span></span>| <span data-ttu-id="94fa5-178">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="94fa5-178">Phone number of school.</span></span> |
|<span data-ttu-id="94fa5-179">fax</span><span class="sxs-lookup"><span data-stu-id="94fa5-179">fax</span></span>|<span data-ttu-id="94fa5-180">字符串</span><span class="sxs-lookup"><span data-stu-id="94fa5-180">String</span></span>| <span data-ttu-id="94fa5-181">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="94fa5-181">Fax number of school.</span></span> |
|<span data-ttu-id="94fa5-182">address</span><span class="sxs-lookup"><span data-stu-id="94fa5-182">address</span></span>|[<span data-ttu-id="94fa5-183">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="94fa5-183">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="94fa5-184">学校地址。</span><span class="sxs-lookup"><span data-stu-id="94fa5-184">Address of the school.</span></span>|
|<span data-ttu-id="94fa5-185">createdBy</span><span class="sxs-lookup"><span data-stu-id="94fa5-185">createdBy</span></span>|[<span data-ttu-id="94fa5-186">identitySet</span><span class="sxs-lookup"><span data-stu-id="94fa5-186">identitySet</span></span>](identityset.md)|<span data-ttu-id="94fa5-187">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="94fa5-187">Entity who created the school.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94fa5-188">关系</span><span class="sxs-lookup"><span data-stu-id="94fa5-188">Relationships</span></span>
| <span data-ttu-id="94fa5-189">关系</span><span class="sxs-lookup"><span data-stu-id="94fa5-189">Relationship</span></span> | <span data-ttu-id="94fa5-190">类型</span><span class="sxs-lookup"><span data-stu-id="94fa5-190">Type</span></span>   |<span data-ttu-id="94fa5-191">说明</span><span class="sxs-lookup"><span data-stu-id="94fa5-191">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="94fa5-192">classes</span><span class="sxs-lookup"><span data-stu-id="94fa5-192">classes</span></span>|<span data-ttu-id="94fa5-193">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94fa5-193">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="94fa5-194">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="94fa5-194">Classes taught at the school.</span></span> <span data-ttu-id="94fa5-195">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="94fa5-195">Nullable.</span></span>|
|<span data-ttu-id="94fa5-196">users</span><span class="sxs-lookup"><span data-stu-id="94fa5-196">users</span></span>|<span data-ttu-id="94fa5-197">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="94fa5-197">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="94fa5-198">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="94fa5-198">Users in the school.</span></span> <span data-ttu-id="94fa5-199">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="94fa5-199">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94fa5-200">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="94fa5-200">JSON representation</span></span>

<span data-ttu-id="94fa5-201">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="94fa5-201">The following is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.educationOrganization",
  "@odata.type": "microsoft.graph.educationSchool"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "description": "String",
  "status": "String",
  "externalSource": "String",
  "principalEmail": "String",
  "principalName": "String",
  "externalPrincipalId": "String",
  "highestGrade": "String",
  "lowestGrade": "String",
  "schoolNumber": "String",
  "address": {"@odata.type": "microsoft.graph.physicalAddress"},
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "externalId": "String",
  "fax": "String",
  "phone": "String",
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationSchool resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
