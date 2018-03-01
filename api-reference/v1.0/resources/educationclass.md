# <a name="educationclass-resource-type"></a><span data-ttu-id="8ed03-101">educationClass 资源类型</span><span class="sxs-lookup"><span data-stu-id="8ed03-101">educationClass resource type</span></span>

<span data-ttu-id="8ed03-102">表示学校的课程。</span><span class="sxs-lookup"><span data-stu-id="8ed03-102">Represents a class within a school.</span></span> <span data-ttu-id="8ed03-103">**educationClass** 资源对应于 Office 365 组并共享同一个 ID。</span><span class="sxs-lookup"><span data-stu-id="8ed03-103">The **educationClass** resource corresponds to the Office 365 group and shares the same ID.</span></span> <span data-ttu-id="8ed03-104">学生是课程的正式成员，教师为所有者，且具有相应权限。</span><span class="sxs-lookup"><span data-stu-id="8ed03-104">Students are regular members of the class, and teachers are owners and have appropriate rights.</span></span> <span data-ttu-id="8ed03-105">若要使 Office 体验正常进行，教师必须同时为教师和成员集合的成员。</span><span class="sxs-lookup"><span data-stu-id="8ed03-105">For Office experiences to work correctly, teachers must be members of both the teachers and members collections.</span></span>  


## <a name="methods"></a><span data-ttu-id="8ed03-106">方法</span><span class="sxs-lookup"><span data-stu-id="8ed03-106">Methods</span></span>

| <span data-ttu-id="8ed03-107">方法</span><span class="sxs-lookup"><span data-stu-id="8ed03-107">Method</span></span>           | <span data-ttu-id="8ed03-108">返回类型</span><span class="sxs-lookup"><span data-stu-id="8ed03-108">Return Type</span></span>    |<span data-ttu-id="8ed03-109">说明</span><span class="sxs-lookup"><span data-stu-id="8ed03-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8ed03-110">Get educationClass</span><span class="sxs-lookup"><span data-stu-id="8ed03-110">Get educationClass</span></span>](../api/educationclass_get.md) | [<span data-ttu-id="8ed03-111">educationClass</span><span class="sxs-lookup"><span data-stu-id="8ed03-111">educationClass</span></span>](educationclass.md) |<span data-ttu-id="8ed03-112">读取 **educationClass** 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="8ed03-112">Read properties and relationships of **plannerTaskDetails** object.</span></span>|
|[<span data-ttu-id="8ed03-113">Add member</span><span class="sxs-lookup"><span data-stu-id="8ed03-113">Add member</span></span>](../api/educationclass_post_members.md) |[<span data-ttu-id="8ed03-114">educationUser</span><span class="sxs-lookup"><span data-stu-id="8ed03-114">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8ed03-115">通过发布到 members 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="8ed03-115">Add a new **educationUser** for the class by posting to the members navigation property.</span></span>|
|[<span data-ttu-id="8ed03-116">List members</span><span class="sxs-lookup"><span data-stu-id="8ed03-116">List members</span></span>](../api/educationclass_list_members.md) |<span data-ttu-id="8ed03-117">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed03-117">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8ed03-118">获取 **educationUser** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8ed03-118">Get an **educationUser** object collection.</span></span>|
|[<span data-ttu-id="8ed03-119">Remove student</span><span class="sxs-lookup"><span data-stu-id="8ed03-119">Remove student</span></span>](../api/educationclass_delete_members.md) |[<span data-ttu-id="8ed03-120">educationUser</span><span class="sxs-lookup"><span data-stu-id="8ed03-120">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8ed03-121">通过成员导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="8ed03-121">Remove an **educationUser** from the class through the members navigation property.</span></span>|
|[<span data-ttu-id="8ed03-122">List schools</span><span class="sxs-lookup"><span data-stu-id="8ed03-122">List schools</span></span>](../api/educationclass_list_schools.md) |<span data-ttu-id="8ed03-123">[educationSchool](educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed03-123">[educationSchool](educationschool.md) collection</span></span>| <span data-ttu-id="8ed03-124">获取 **educationSchool** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8ed03-124">Get an **educationSchool** object collection.</span></span>|
|[<span data-ttu-id="8ed03-125">Add teacher</span><span class="sxs-lookup"><span data-stu-id="8ed03-125">Add teacher</span></span>](../api/educationclass_post_teachers.md) |[<span data-ttu-id="8ed03-126">educationUser</span><span class="sxs-lookup"><span data-stu-id="8ed03-126">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8ed03-127">通过发布到 teachers 导航属性，为课程添加一个新的 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="8ed03-127">Add a new **educationUser** for the class by posting to the teachers navigation property.</span></span>|
|[<span data-ttu-id="8ed03-128">List teachers</span><span class="sxs-lookup"><span data-stu-id="8ed03-128">List teachers</span></span>](../api/educationclass_list_teachers.md) |<span data-ttu-id="8ed03-129">[educationUser](educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed03-129">[educationUser](educationuser.md) collection</span></span>| <span data-ttu-id="8ed03-130">获取课程的教师列表。</span><span class="sxs-lookup"><span data-stu-id="8ed03-130">Get a list of teachers for the class.</span></span>|
|[<span data-ttu-id="8ed03-131">Remove teacher</span><span class="sxs-lookup"><span data-stu-id="8ed03-131">Remove teacher</span></span>](../api/educationclass_delete_teachers.md) |[<span data-ttu-id="8ed03-132">educationUser</span><span class="sxs-lookup"><span data-stu-id="8ed03-132">educationUser</span></span>](educationuser.md)| <span data-ttu-id="8ed03-133">通过教师导航属性从课程删除 **educationUser**。</span><span class="sxs-lookup"><span data-stu-id="8ed03-133">Remove an **educationUser** from the class through the teachers navigation property.</span></span>|
|[<span data-ttu-id="8ed03-134">Get group</span><span class="sxs-lookup"><span data-stu-id="8ed03-134">Get group</span></span>](../api/educationclass_get_group.md) |[<span data-ttu-id="8ed03-135">group</span><span class="sxs-lookup"><span data-stu-id="8ed03-135">group</span></span>](group.md)| <span data-ttu-id="8ed03-136">获得与此 **educationClass** 对应的 Office 365 **group**。</span><span class="sxs-lookup"><span data-stu-id="8ed03-136">Get the Office 365 **group** that corresponds to this **educationClass**.</span></span>|
|[<span data-ttu-id="8ed03-137">Update</span><span class="sxs-lookup"><span data-stu-id="8ed03-137">Update</span></span>](../api/educationclass_update.md) | [<span data-ttu-id="8ed03-138">educationClass</span><span class="sxs-lookup"><span data-stu-id="8ed03-138">educationClass</span></span>](educationclass.md)    |<span data-ttu-id="8ed03-139">更新 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="8ed03-139">Update **educationClass** object.</span></span> |
|[<span data-ttu-id="8ed03-140">Delete</span><span class="sxs-lookup"><span data-stu-id="8ed03-140">Delete</span></span>](../api/educationclass_delete.md) | <span data-ttu-id="8ed03-141">无</span><span class="sxs-lookup"><span data-stu-id="8ed03-141">None</span></span> |<span data-ttu-id="8ed03-142">删除 **educationClass** 对象。</span><span class="sxs-lookup"><span data-stu-id="8ed03-142">Delete **educationClass** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="8ed03-143">属性</span><span class="sxs-lookup"><span data-stu-id="8ed03-143">Properties</span></span>
| <span data-ttu-id="8ed03-144">属性</span><span class="sxs-lookup"><span data-stu-id="8ed03-144">Property</span></span>     | <span data-ttu-id="8ed03-145">类型</span><span class="sxs-lookup"><span data-stu-id="8ed03-145">Type</span></span>   |<span data-ttu-id="8ed03-146">说明</span><span class="sxs-lookup"><span data-stu-id="8ed03-146">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ed03-147">id</span><span class="sxs-lookup"><span data-stu-id="8ed03-147">id</span></span>| <span data-ttu-id="8ed03-148">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-148">String</span></span>| <span data-ttu-id="8ed03-149">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="8ed03-149">Unique identifier for the identity.</span></span>|
|<span data-ttu-id="8ed03-150">description</span><span class="sxs-lookup"><span data-stu-id="8ed03-150">description</span></span>|<span data-ttu-id="8ed03-151">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-151">String</span></span>| <span data-ttu-id="8ed03-152">课程说明。</span><span class="sxs-lookup"><span data-stu-id="8ed03-152">Description of the template.</span></span>|
|<span data-ttu-id="8ed03-153">displayName</span><span class="sxs-lookup"><span data-stu-id="8ed03-153">displayName</span></span>|<span data-ttu-id="8ed03-154">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-154">String</span></span>| <span data-ttu-id="8ed03-155">课程名称。</span><span class="sxs-lookup"><span data-stu-id="8ed03-155">Name of the class.</span></span>|
|<span data-ttu-id="8ed03-156">mailNickname</span><span class="sxs-lookup"><span data-stu-id="8ed03-156">mailNickname</span></span>|<span data-ttu-id="8ed03-157">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-157">String</span></span>| <span data-ttu-id="8ed03-158">向所有成员发送电子邮件的邮件名称（如果已启用）。</span><span class="sxs-lookup"><span data-stu-id="8ed03-158">Mail name for sending email to all members, if this is enabled.</span></span> |
|<span data-ttu-id="8ed03-159">createdBy</span><span class="sxs-lookup"><span data-stu-id="8ed03-159">createdBy</span></span>|[<span data-ttu-id="8ed03-160">identitySet</span><span class="sxs-lookup"><span data-stu-id="8ed03-160">identitySet</span></span>](identityset.md)| <span data-ttu-id="8ed03-161">创建了课程的实体</span><span class="sxs-lookup"><span data-stu-id="8ed03-161">Entity who created the class</span></span> |
|<span data-ttu-id="8ed03-162">classCode</span><span class="sxs-lookup"><span data-stu-id="8ed03-162">classCode</span></span>|<span data-ttu-id="8ed03-163">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-163">String</span></span>| <span data-ttu-id="8ed03-164">学校用于标识课程的课程代码。</span><span class="sxs-lookup"><span data-stu-id="8ed03-164">Class code used by the school to identify the class.</span></span>|
|<span data-ttu-id="8ed03-165">externalId</span><span class="sxs-lookup"><span data-stu-id="8ed03-165">externalId</span></span>|<span data-ttu-id="8ed03-166">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-166">String</span></span>| <span data-ttu-id="8ed03-167">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="8ed03-167">ID of the class from the syncing system.</span></span> |
|<span data-ttu-id="8ed03-168">externalName</span><span class="sxs-lookup"><span data-stu-id="8ed03-168">externalName</span></span>|<span data-ttu-id="8ed03-169">String</span><span class="sxs-lookup"><span data-stu-id="8ed03-169">String</span></span>|<span data-ttu-id="8ed03-170">同步系统中的课程名称。</span><span class="sxs-lookup"><span data-stu-id="8ed03-170">Name of the class in the syncing system.</span></span>|
|<span data-ttu-id="8ed03-171">externalSource</span><span class="sxs-lookup"><span data-stu-id="8ed03-171">externalSource</span></span>|<span data-ttu-id="8ed03-172">string</span><span class="sxs-lookup"><span data-stu-id="8ed03-172">string</span></span>| <span data-ttu-id="8ed03-173">此课程的创建方式。</span><span class="sxs-lookup"><span data-stu-id="8ed03-173">How this class was created.</span></span> <span data-ttu-id="8ed03-174">可取值为：`sis`、`manual`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="8ed03-174">Possible values are: `sis`, `manual`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="8ed03-175">term</span><span class="sxs-lookup"><span data-stu-id="8ed03-175">Term</span></span>|[<span data-ttu-id="8ed03-176">educationTerm</span><span class="sxs-lookup"><span data-stu-id="8ed03-176">educationTerm</span></span>](educationterm.md)|<span data-ttu-id="8ed03-177">此课程的学期。</span><span class="sxs-lookup"><span data-stu-id="8ed03-177">Term for this class.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8ed03-178">关系</span><span class="sxs-lookup"><span data-stu-id="8ed03-178">Relationships</span></span>
| <span data-ttu-id="8ed03-179">关系</span><span class="sxs-lookup"><span data-stu-id="8ed03-179">Relationship</span></span> | <span data-ttu-id="8ed03-180">类型</span><span class="sxs-lookup"><span data-stu-id="8ed03-180">Type</span></span>   |<span data-ttu-id="8ed03-181">说明</span><span class="sxs-lookup"><span data-stu-id="8ed03-181">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8ed03-182">members</span><span class="sxs-lookup"><span data-stu-id="8ed03-182">members</span></span>|<span data-ttu-id="8ed03-183">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed03-183">[educationUser](../resources/educationuser.md) collection</span></span>| <span data-ttu-id="8ed03-184">课程中的所有用户。</span><span class="sxs-lookup"><span data-stu-id="8ed03-184">All users in the class.</span></span> <span data-ttu-id="8ed03-185">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8ed03-185">Nullable.</span></span>|
|<span data-ttu-id="8ed03-186">schools</span><span class="sxs-lookup"><span data-stu-id="8ed03-186">schools</span></span>|<span data-ttu-id="8ed03-187">[educationSchool](../resources/educationschool.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed03-187">[educationSchool](../resources/educationschool.md) collection</span></span>| <span data-ttu-id="8ed03-188">与此课程相关的所有学校。</span><span class="sxs-lookup"><span data-stu-id="8ed03-188">All schools that this class is associated with.</span></span> <span data-ttu-id="8ed03-189">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8ed03-189">Nullable.</span></span>|
|<span data-ttu-id="8ed03-190">teachers</span><span class="sxs-lookup"><span data-stu-id="8ed03-190">teachers</span></span>|<span data-ttu-id="8ed03-191">[educationUser](../resources/educationuser.md) 集合</span><span class="sxs-lookup"><span data-stu-id="8ed03-191">[educationUser](../resources/educationuser.md) collection</span></span>|  <span data-ttu-id="8ed03-192">课程中的所有教师。</span><span class="sxs-lookup"><span data-stu-id="8ed03-192">All teachers in the class.</span></span> <span data-ttu-id="8ed03-193">可为 NULL。</span><span class="sxs-lookup"><span data-stu-id="8ed03-193">Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="8ed03-194">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8ed03-194">JSON representation</span></span>

<span data-ttu-id="8ed03-195">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8ed03-195">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationClass"
}-->

```json
{
  "id": "String",
  "description": "String",
  "classCode": "String",
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "displayName": "String",
  "externalId": "String",
  "externalName": "String",
  "externalSource": "string",
  "mailNickname": "String",
  "term": {"@odata.type": "microsoft.graph.education.term"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationClass resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
