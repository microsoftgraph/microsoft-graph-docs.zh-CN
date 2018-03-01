# <a name="educationschool-resource-type"></a><span data-ttu-id="9dd4c-101">educationSchool 资源类型</span><span class="sxs-lookup"><span data-stu-id="9dd4c-101">educationSchool resource type</span></span>

<span data-ttu-id="9dd4c-102">学校。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-102">A school.</span></span> <span data-ttu-id="9dd4c-103">**educationSchool** 资源当前对应于 [administrativeUnit](../../beta/resources/administrativeunit.md) 资源并共享同一 ID。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-103">The **educationSchool** resource currently corresponds to an [administrativeUnit](../../beta/resources/administrativeunit.md) resource and shares the same ID.</span></span>  

><span data-ttu-id="9dd4c-104">**注意：****administrativeUnit** 和 **educationOrganization** 资源目前为 beta 版。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-104">**Note:**  The **administrativeUnit** and **educationOrganization** resources are currently in beta.</span></span> <span data-ttu-id="9dd4c-105">如果你正在使用这些资源，请务必定期查看[更改日志](../../../concepts/changelog.md)。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-105">If you're using these resources, be sure to review the [Changelog](../../../concepts/changelog.md) periodically.</span></span> <span data-ttu-id="9dd4c-106">当 Microsoft Graph API 资源发布到 v1.0 终结点时，将在更改日志中对此进行说明。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-106">When Microsoft Graph API resources are released to the v1.0  endpoint, we'll note this in the Changelog.</span></span> <span data-ttu-id="9dd4c-107">如果应用使用 **administrativeUnit** 或 **educationOrganization** 资源，将需要声明基本请求 URL，如下面的代码块所示。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-107">If your app consumes the **administrativeUnit** or **educationOrganization** resources, you will need to declare base request URLs as shown in the the following code block.</span></span>  
  ```JavaScript
  var v1BaseUrl = “https://graph.microsoft.com/v1.0/education”;
  var betaBaseUrl = “https://graph.microsoft.com/beta/education”;  // for administrativeUnit and educationOrganization
  ```

<span data-ttu-id="9dd4c-108">此资源是 [educationOrganization](../../beta/resources/educationorganization.md) 的子类型。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-108">This resource is a subtype of [educationOrganization](../../beta/resources/educationorganization.md).</span></span>


## <a name="methods"></a><span data-ttu-id="9dd4c-109">方法</span><span class="sxs-lookup"><span data-stu-id="9dd4c-109">Methods</span></span>

| <span data-ttu-id="9dd4c-110">方法</span><span class="sxs-lookup"><span data-stu-id="9dd4c-110">Method</span></span>           | <span data-ttu-id="9dd4c-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9dd4c-111">Return Type</span></span>    |<span data-ttu-id="9dd4c-112">说明</span><span class="sxs-lookup"><span data-stu-id="9dd4c-112">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9dd4c-113">Get</span><span class="sxs-lookup"><span data-stu-id="9dd4c-113">Get</span></span>](../api/educationschool_get.md) | [<span data-ttu-id="9dd4c-114">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9dd4c-114">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="9dd4c-115">读取 **educationSchool** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-115">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="9dd4c-116">Add class</span><span class="sxs-lookup"><span data-stu-id="9dd4c-116">Add class</span></span>](../api/educationschool_post_classes.md) |[<span data-ttu-id="9dd4c-117">educationClass</span><span class="sxs-lookup"><span data-stu-id="9dd4c-117">educationClass</span></span>](educationclass.md)| <span data-ttu-id="9dd4c-118">通过发布到课程导航属性，为学校添加一个新的 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-118">Add a new **educationClass** for the school by posting to the classes navigation property.</span></span>|
|[<span data-ttu-id="9dd4c-119">List classes</span><span class="sxs-lookup"><span data-stu-id="9dd4c-119">List classes</span></span>](../api/educationschool_list_classes.md) |<span data-ttu-id="9dd4c-120">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd4c-120">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="9dd4c-121">获取 **educationClass** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-121">Get the **educationClass** object collection.</span></span>|
|[<span data-ttu-id="9dd4c-122">Remove class</span><span class="sxs-lookup"><span data-stu-id="9dd4c-122">Remove class</span></span>](../api/educationschool_delete_classes.md) |[<span data-ttu-id="9dd4c-123">educationClass</span><span class="sxs-lookup"><span data-stu-id="9dd4c-123">educationClass</span></span>](educationclass.md)| <span data-ttu-id="9dd4c-124">通过课程导航属性从学校删除 **educationClass**。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-124">Remove an **educationClass** from the school through the classes navigation property.</span></span>|
|[<span data-ttu-id="9dd4c-125">Add user</span><span class="sxs-lookup"><span data-stu-id="9dd4c-125">Add user</span></span>](../api/educationschool_post_users.md) |[<span data-ttu-id="9dd4c-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="9dd4c-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="9dd4c-127">通过发布到 **users** 导航属性，为学校添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-127">Add a new **educationUser** for the school by posting to the **users** navigation property.</span></span>|
|[<span data-ttu-id="9dd4c-128">List users</span><span class="sxs-lookup"><span data-stu-id="9dd4c-128">List users</span></span>](../api/educationschool_list_users.md) |<span data-ttu-id="9dd4c-129">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd4c-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="9dd4c-130">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-130">Get the **educationUser** object collection.</span></span>|
|[<span data-ttu-id="9dd4c-131">Remove user</span><span class="sxs-lookup"><span data-stu-id="9dd4c-131">Remove user</span></span>](../api/educationschool_delete_users.md) |[<span data-ttu-id="9dd4c-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="9dd4c-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="9dd4c-133">通过 **users** 导航属性从学校删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-133">Remove an **educationUser** from the school through the **users** navigation property.</span></span>|
|[<span data-ttu-id="9dd4c-134">Get administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9dd4c-134">Get administrativeUnit</span></span>](../api/educationschool_get_administrativeunit.md) |[<span data-ttu-id="9dd4c-135">administrativeUnit</span><span class="sxs-lookup"><span data-stu-id="9dd4c-135">administrativeUnit</span></span>](../../beta/resources/administrativeunit.md)| <span data-ttu-id="9dd4c-136">获取与此 **educationSchool** 对应的 **administrativeUnit**。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-136">Get the **administrativeUnit** that corresponds to this **educationSchool**.</span></span>|
|[<span data-ttu-id="9dd4c-137">Update</span><span class="sxs-lookup"><span data-stu-id="9dd4c-137">Update</span></span>](../api/educationschool_update.md) | [<span data-ttu-id="9dd4c-138">educationSchool</span><span class="sxs-lookup"><span data-stu-id="9dd4c-138">educationSchool</span></span>](educationschool.md) |<span data-ttu-id="9dd4c-139">更新 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-139">Update an **event** object.</span></span> |
|[<span data-ttu-id="9dd4c-140">Delete</span><span class="sxs-lookup"><span data-stu-id="9dd4c-140">Delete</span></span>](../api/educationschool_delete.md) | <span data-ttu-id="9dd4c-141">无</span><span class="sxs-lookup"><span data-stu-id="9dd4c-141">None</span></span> |<span data-ttu-id="9dd4c-142">删除 **educationSchool** 对象。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-142">Delete an **event** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="9dd4c-143">属性</span><span class="sxs-lookup"><span data-stu-id="9dd4c-143">Properties</span></span>
| <span data-ttu-id="9dd4c-144">属性</span><span class="sxs-lookup"><span data-stu-id="9dd4c-144">Property</span></span>     | <span data-ttu-id="9dd4c-145">类型</span><span class="sxs-lookup"><span data-stu-id="9dd4c-145">Type</span></span>   |<span data-ttu-id="9dd4c-146">说明</span><span class="sxs-lookup"><span data-stu-id="9dd4c-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dd4c-147">id</span><span class="sxs-lookup"><span data-stu-id="9dd4c-147">id</span></span>|<span data-ttu-id="9dd4c-148">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-148">String</span></span>|<span data-ttu-id="9dd4c-149">该学校的 GUID。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-149">GUID of this school.</span></span>|
|<span data-ttu-id="9dd4c-150">displayName</span><span class="sxs-lookup"><span data-stu-id="9dd4c-150">displayName</span></span>| <span data-ttu-id="9dd4c-151">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-151">String</span></span>| <span data-ttu-id="9dd4c-152">学校的显示名称。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-152">Display name of the template.</span></span>| 
|<span data-ttu-id="9dd4c-153">description</span><span class="sxs-lookup"><span data-stu-id="9dd4c-153">description</span></span>| <span data-ttu-id="9dd4c-154">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-154">String</span></span> | <span data-ttu-id="9dd4c-155">学校描述。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-155">Description of the template.</span></span>| 
|<span data-ttu-id="9dd4c-156">status</span><span class="sxs-lookup"><span data-stu-id="9dd4c-156">status</span></span>| <span data-ttu-id="9dd4c-157">string</span><span class="sxs-lookup"><span data-stu-id="9dd4c-157">string</span></span>| <span data-ttu-id="9dd4c-158">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-158">Read-only.</span></span> <span data-ttu-id="9dd4c-159">可取值为：`inactive`、`active`、`expired`、`deleteable`。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-159">Possible values are: `inactive`, `active`, `expired`, `deleteable`.</span></span>|
|<span data-ttu-id="9dd4c-160">externalSource</span><span class="sxs-lookup"><span data-stu-id="9dd4c-160">externalSource</span></span>| <span data-ttu-id="9dd4c-161">string</span><span class="sxs-lookup"><span data-stu-id="9dd4c-161">string</span></span>| <span data-ttu-id="9dd4c-162">只读。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-162">Read-only.</span></span>  <span data-ttu-id="9dd4c-163">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-163">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="9dd4c-164">principalEmail</span><span class="sxs-lookup"><span data-stu-id="9dd4c-164">principalEmail</span></span>| <span data-ttu-id="9dd4c-165">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-165">String</span></span>| <span data-ttu-id="9dd4c-166">主体的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-166">Email address of the principal.</span></span>|
|<span data-ttu-id="9dd4c-167">principalName</span><span class="sxs-lookup"><span data-stu-id="9dd4c-167">PrincipalName</span></span>| <span data-ttu-id="9dd4c-168">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-168">String</span></span> | <span data-ttu-id="9dd4c-169">主体名称。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-169">Name of the principal.</span></span>|
|<span data-ttu-id="9dd4c-170">externalPrincipalId</span><span class="sxs-lookup"><span data-stu-id="9dd4c-170">externalPrincipalId</span></span>| <span data-ttu-id="9dd4c-171">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-171">String</span></span> | <span data-ttu-id="9dd4c-172">同步系统中主体的 ID。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-172">ID of principal in syncing system.</span></span> |
|<span data-ttu-id="9dd4c-173">highestGrade</span><span class="sxs-lookup"><span data-stu-id="9dd4c-173">highestGrade</span></span>|<span data-ttu-id="9dd4c-174">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-174">String</span></span>| <span data-ttu-id="9dd4c-175">教授的最高年级。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-175">Highest grade taught.</span></span> |
|<span data-ttu-id="9dd4c-176">lowestGrade</span><span class="sxs-lookup"><span data-stu-id="9dd4c-176">lowestGrade</span></span>|<span data-ttu-id="9dd4c-177">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-177">String</span></span>| <span data-ttu-id="9dd4c-178">教授的最低年级。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-178">Lowest grade taught.</span></span> |
|<span data-ttu-id="9dd4c-179">schoolNumber</span><span class="sxs-lookup"><span data-stu-id="9dd4c-179">schoolNumber</span></span>|<span data-ttu-id="9dd4c-180">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-180">String</span></span>| <span data-ttu-id="9dd4c-181">学校编号。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-181">School Number.</span></span>|
|<span data-ttu-id="9dd4c-182">externalId</span><span class="sxs-lookup"><span data-stu-id="9dd4c-182">externalId</span></span>|<span data-ttu-id="9dd4c-183">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-183">String</span></span>| <span data-ttu-id="9dd4c-184">同步系统中学校的 ID。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-184">ID of school in syncing system.</span></span> |
|<span data-ttu-id="9dd4c-185">phone</span><span class="sxs-lookup"><span data-stu-id="9dd4c-185">Phone</span></span>|<span data-ttu-id="9dd4c-186">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-186">String</span></span>| <span data-ttu-id="9dd4c-187">学校电话号码。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-187">Phone number of school.</span></span> |
|<span data-ttu-id="9dd4c-188">fax</span><span class="sxs-lookup"><span data-stu-id="9dd4c-188">fax</span></span>|<span data-ttu-id="9dd4c-189">String</span><span class="sxs-lookup"><span data-stu-id="9dd4c-189">String</span></span>| <span data-ttu-id="9dd4c-190">学校传真号码。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-190">Fax number of school.</span></span> |
|<span data-ttu-id="9dd4c-191">address</span><span class="sxs-lookup"><span data-stu-id="9dd4c-191">address</span></span>|[<span data-ttu-id="9dd4c-192">physicalAddress</span><span class="sxs-lookup"><span data-stu-id="9dd4c-192">physicalAddress</span></span>](physicaladdress.md)| <span data-ttu-id="9dd4c-193">学校地址。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-193">Address of the school.</span></span>|
|<span data-ttu-id="9dd4c-194">createdBy</span><span class="sxs-lookup"><span data-stu-id="9dd4c-194">createdBy</span></span>|[<span data-ttu-id="9dd4c-195">identitySet</span><span class="sxs-lookup"><span data-stu-id="9dd4c-195">identitySet</span></span>](identityset.md)|<span data-ttu-id="9dd4c-196">创建了学校的实体。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-196">Entity who created the school.</span></span>|


## <a name="relationships"></a><span data-ttu-id="9dd4c-197">关系</span><span class="sxs-lookup"><span data-stu-id="9dd4c-197">Relationships</span></span>
| <span data-ttu-id="9dd4c-198">关系</span><span class="sxs-lookup"><span data-stu-id="9dd4c-198">Relationship</span></span> | <span data-ttu-id="9dd4c-199">类型</span><span class="sxs-lookup"><span data-stu-id="9dd4c-199">Type</span></span>   |<span data-ttu-id="9dd4c-200">说明</span><span class="sxs-lookup"><span data-stu-id="9dd4c-200">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9dd4c-201">classes</span><span class="sxs-lookup"><span data-stu-id="9dd4c-201">Classes</span></span>|<span data-ttu-id="9dd4c-202">[educationClass](educationclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd4c-202">[educationClass](educationclass.md) collection</span></span>| <span data-ttu-id="9dd4c-203">在学校教授的课程。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-203">Classes taught at the school.</span></span> <span data-ttu-id="9dd4c-204">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-204">Nullable.</span></span>|
|<span data-ttu-id="9dd4c-205">users</span><span class="sxs-lookup"><span data-stu-id="9dd4c-205">users</span></span>|<span data-ttu-id="9dd4c-206">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9dd4c-206">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="9dd4c-207">学校中的用户。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-207">Users in the school.</span></span> <span data-ttu-id="9dd4c-208">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-208">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9dd4c-209">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9dd4c-209">JSON representation</span></span>

<span data-ttu-id="9dd4c-210">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9dd4c-210">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
