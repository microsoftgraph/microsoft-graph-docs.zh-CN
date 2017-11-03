# <a name="contact-resource-type"></a><span data-ttu-id="2e4eb-101">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="2e4eb-101">contact resource type</span></span>

<span data-ttu-id="2e4eb-p101">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="2e4eb-104">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="2e4eb-104">This resource supports:</span></span>

- <span data-ttu-id="2e4eb-105">使用[扩展](../../../concepts/extensibility_overview.md)将自己的数据添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-105">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="2e4eb-106">通过提供 [delta](../api/contact_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-106">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="2e4eb-107">方法</span><span class="sxs-lookup"><span data-stu-id="2e4eb-107">Methods</span></span>

| <span data-ttu-id="2e4eb-108">方法</span><span class="sxs-lookup"><span data-stu-id="2e4eb-108">Method</span></span>       | <span data-ttu-id="2e4eb-109">返回类型</span><span class="sxs-lookup"><span data-stu-id="2e4eb-109">Return Type</span></span>  |<span data-ttu-id="2e4eb-110">说明</span><span class="sxs-lookup"><span data-stu-id="2e4eb-110">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e4eb-111">获取联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-111">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="2e4eb-112">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-112">contact</span></span>](contact.md) |<span data-ttu-id="2e4eb-113">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-113">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="2e4eb-114">创建</span><span class="sxs-lookup"><span data-stu-id="2e4eb-114">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="2e4eb-115">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-115">contact</span></span>](contact.md) |<span data-ttu-id="2e4eb-116">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-116">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="2e4eb-117">更新</span><span class="sxs-lookup"><span data-stu-id="2e4eb-117">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="2e4eb-118">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-118">contact</span></span>](contact.md) |<span data-ttu-id="2e4eb-119">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-119">Update contact object.</span></span> |
|[<span data-ttu-id="2e4eb-120">删除</span><span class="sxs-lookup"><span data-stu-id="2e4eb-120">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="2e4eb-121">无</span><span class="sxs-lookup"><span data-stu-id="2e4eb-121">None</span></span> |<span data-ttu-id="2e4eb-122">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-122">Delete contact object.</span></span> |
|[<span data-ttu-id="2e4eb-123">delta</span><span class="sxs-lookup"><span data-stu-id="2e4eb-123">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="2e4eb-124">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e4eb-124">[contact](contact.md) collection</span></span>| <span data-ttu-id="2e4eb-125">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-125">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="2e4eb-126">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="2e4eb-126">**Open extensions**</span></span>| | |
|[<span data-ttu-id="2e4eb-127">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="2e4eb-127">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="2e4eb-128">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="2e4eb-128">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="2e4eb-129">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-129">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="2e4eb-130">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="2e4eb-130">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="2e4eb-131">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e4eb-131">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="2e4eb-132">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-132">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="2e4eb-133">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="2e4eb-133">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="2e4eb-134">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="2e4eb-134">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="2e4eb-135">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-135">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="2e4eb-136">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="2e4eb-136">**Extended properties**</span></span>| | |
|[<span data-ttu-id="2e4eb-137">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="2e4eb-137">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="2e4eb-138">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-138">contact</span></span>](contact.md)  |<span data-ttu-id="2e4eb-139">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-139">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="2e4eb-140">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-140">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="2e4eb-141">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-141">contact</span></span>](contact.md) | <span data-ttu-id="2e4eb-142">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-142">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="2e4eb-143">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="2e4eb-143">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="2e4eb-144">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-144">contact</span></span>](contact.md) | <span data-ttu-id="2e4eb-145">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-145">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="2e4eb-146">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-146">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="2e4eb-147">联系人</span><span class="sxs-lookup"><span data-stu-id="2e4eb-147">contact</span></span>](contact.md) | <span data-ttu-id="2e4eb-148">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-148">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e4eb-149">属性</span><span class="sxs-lookup"><span data-stu-id="2e4eb-149">Properties</span></span>
| <span data-ttu-id="2e4eb-150">属性</span><span class="sxs-lookup"><span data-stu-id="2e4eb-150">Property</span></span>     | <span data-ttu-id="2e4eb-151">类型</span><span class="sxs-lookup"><span data-stu-id="2e4eb-151">Type</span></span>   |<span data-ttu-id="2e4eb-152">说明</span><span class="sxs-lookup"><span data-stu-id="2e4eb-152">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e4eb-153">assistantName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-153">assistantName</span></span>|<span data-ttu-id="2e4eb-154">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-154">String</span></span>|<span data-ttu-id="2e4eb-155">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-155">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="2e4eb-156">birthday</span><span class="sxs-lookup"><span data-stu-id="2e4eb-156">birthday</span></span>|<span data-ttu-id="2e4eb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e4eb-157">DateTimeOffset</span></span>|<span data-ttu-id="2e4eb-p102">联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2e4eb-161">businessAddress</span><span class="sxs-lookup"><span data-stu-id="2e4eb-161">businessAddress</span></span>|[<span data-ttu-id="2e4eb-162">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="2e4eb-162">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="2e4eb-163">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-163">The contact's business address.</span></span>|
|<span data-ttu-id="2e4eb-164">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="2e4eb-164">businessHomePage</span></span>|<span data-ttu-id="2e4eb-165">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-165">String</span></span>|<span data-ttu-id="2e4eb-166">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-166">The business home page of the contact.</span></span>|
|<span data-ttu-id="2e4eb-167">businessPhones</span><span class="sxs-lookup"><span data-stu-id="2e4eb-167">businessPhones</span></span>|<span data-ttu-id="2e4eb-168">String collection</span><span class="sxs-lookup"><span data-stu-id="2e4eb-168">String collection</span></span>|<span data-ttu-id="2e4eb-169">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-169">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="2e4eb-170">categories</span><span class="sxs-lookup"><span data-stu-id="2e4eb-170">categories</span></span>|<span data-ttu-id="2e4eb-171">String collection</span><span class="sxs-lookup"><span data-stu-id="2e4eb-171">String collection</span></span>|<span data-ttu-id="2e4eb-172">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-172">The categories associated with the contact.</span></span>|
|<span data-ttu-id="2e4eb-173">changeKey</span><span class="sxs-lookup"><span data-stu-id="2e4eb-173">changeKey</span></span>|<span data-ttu-id="2e4eb-174">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-174">String</span></span>|<span data-ttu-id="2e4eb-p103">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="2e4eb-178">children</span><span class="sxs-lookup"><span data-stu-id="2e4eb-178">children</span></span>|<span data-ttu-id="2e4eb-179">String collection</span><span class="sxs-lookup"><span data-stu-id="2e4eb-179">String collection</span></span>|<span data-ttu-id="2e4eb-180">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-180">The names of the contact's children.</span></span>|
|<span data-ttu-id="2e4eb-181">companyName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-181">companyName</span></span>|<span data-ttu-id="2e4eb-182">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-182">String</span></span>|<span data-ttu-id="2e4eb-183">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-183">The name of the contact's company.</span></span>|
|<span data-ttu-id="2e4eb-184">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e4eb-184">createdDateTime</span></span>|<span data-ttu-id="2e4eb-185">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e4eb-185">DateTimeOffset</span></span>|<span data-ttu-id="2e4eb-p104">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2e4eb-189">部门</span><span class="sxs-lookup"><span data-stu-id="2e4eb-189">department</span></span>|<span data-ttu-id="2e4eb-190">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-190">String</span></span>|<span data-ttu-id="2e4eb-191">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-191">The contact's department.</span></span>|
|<span data-ttu-id="2e4eb-192">displayName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-192">displayName</span></span>|<span data-ttu-id="2e4eb-193">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-193">String</span></span>|<span data-ttu-id="2e4eb-194">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-194">The contact's display name.</span></span>|
|<span data-ttu-id="2e4eb-195">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="2e4eb-195">emailAddresses</span></span>|<span data-ttu-id="2e4eb-196">[EmailAddress](emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e4eb-196">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="2e4eb-197">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-197">The contact's email addresses.</span></span>|
|<span data-ttu-id="2e4eb-198">fileAs</span><span class="sxs-lookup"><span data-stu-id="2e4eb-198">fileAs</span></span>|<span data-ttu-id="2e4eb-199">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-199">String</span></span>|<span data-ttu-id="2e4eb-200">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-200">The name the contact is filed under.</span></span>|
|<span data-ttu-id="2e4eb-201">generation</span><span class="sxs-lookup"><span data-stu-id="2e4eb-201">generation</span></span>|<span data-ttu-id="2e4eb-202">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-202">String</span></span>|<span data-ttu-id="2e4eb-203">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-203">The contact's generation.</span></span>|
|<span data-ttu-id="2e4eb-204">givenName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-204">givenName</span></span>|<span data-ttu-id="2e4eb-205">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-205">String</span></span>|<span data-ttu-id="2e4eb-206">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-206">The contact's given name.</span></span>|
|<span data-ttu-id="2e4eb-207">homeAddress</span><span class="sxs-lookup"><span data-stu-id="2e4eb-207">homeAddress</span></span>|[<span data-ttu-id="2e4eb-208">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="2e4eb-208">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="2e4eb-209">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-209">The contact's home address.</span></span>|
|<span data-ttu-id="2e4eb-210">homePhones</span><span class="sxs-lookup"><span data-stu-id="2e4eb-210">homePhones</span></span>|<span data-ttu-id="2e4eb-211">String collection</span><span class="sxs-lookup"><span data-stu-id="2e4eb-211">String collection</span></span>|<span data-ttu-id="2e4eb-212">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-212">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="2e4eb-213">id</span><span class="sxs-lookup"><span data-stu-id="2e4eb-213">id</span></span>|<span data-ttu-id="2e4eb-214">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-214">String</span></span>|<span data-ttu-id="2e4eb-p105">联系人的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p105">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="2e4eb-217">imAddresses</span><span class="sxs-lookup"><span data-stu-id="2e4eb-217">imAddresses</span></span>|<span data-ttu-id="2e4eb-218">String collection</span><span class="sxs-lookup"><span data-stu-id="2e4eb-218">String collection</span></span>|<span data-ttu-id="2e4eb-219">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-219">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="2e4eb-220">initials</span><span class="sxs-lookup"><span data-stu-id="2e4eb-220">initials</span></span>|<span data-ttu-id="2e4eb-221">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-221">String</span></span>|<span data-ttu-id="2e4eb-222">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-222">The contact's initials.</span></span>|
|<span data-ttu-id="2e4eb-223">jobTitle</span><span class="sxs-lookup"><span data-stu-id="2e4eb-223">jobTitle</span></span>|<span data-ttu-id="2e4eb-224">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-224">String</span></span>|<span data-ttu-id="2e4eb-225">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-225">The contact’s job title.</span></span>|
|<span data-ttu-id="2e4eb-226">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e4eb-226">lastModifiedDateTime</span></span>|<span data-ttu-id="2e4eb-227">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e4eb-227">DateTimeOffset</span></span>|<span data-ttu-id="2e4eb-p106">修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p106">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2e4eb-231">manager</span><span class="sxs-lookup"><span data-stu-id="2e4eb-231">manager</span></span>|<span data-ttu-id="2e4eb-232">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-232">String</span></span>|<span data-ttu-id="2e4eb-233">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-233">The name of the contact's manager.</span></span>
|<span data-ttu-id="2e4eb-234">middleName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-234">middleName</span></span>|<span data-ttu-id="2e4eb-235">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-235">String</span></span>|<span data-ttu-id="2e4eb-236">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-236">The contact's middle name.</span></span>|
|<span data-ttu-id="2e4eb-237">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="2e4eb-237">mobilePhone</span></span>|<span data-ttu-id="2e4eb-238">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-238">String</span></span>|<span data-ttu-id="2e4eb-239">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-239">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="2e4eb-240">nickName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-240">nickName</span></span>|<span data-ttu-id="2e4eb-241">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-241">String</span></span>|<span data-ttu-id="2e4eb-242">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-242">The contact's nickname.</span></span>|
|<span data-ttu-id="2e4eb-243">officeLocation</span><span class="sxs-lookup"><span data-stu-id="2e4eb-243">officeLocation</span></span>|<span data-ttu-id="2e4eb-244">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-244">String</span></span>|<span data-ttu-id="2e4eb-245">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-245">The location of the contact's office.</span></span>|
|<span data-ttu-id="2e4eb-246">otherAddress</span><span class="sxs-lookup"><span data-stu-id="2e4eb-246">otherAddress</span></span>|[<span data-ttu-id="2e4eb-247">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="2e4eb-247">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="2e4eb-248">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-248">Other addresses for the contact.</span></span>|
|<span data-ttu-id="2e4eb-249">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="2e4eb-249">parentFolderId</span></span>|<span data-ttu-id="2e4eb-250">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-250">String</span></span>|<span data-ttu-id="2e4eb-251">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-251">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="2e4eb-252">personalNotes</span><span class="sxs-lookup"><span data-stu-id="2e4eb-252">personalNotes</span></span>|<span data-ttu-id="2e4eb-253">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-253">String</span></span>|<span data-ttu-id="2e4eb-254">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-254">The user's notes about the contact.</span></span>|
|<span data-ttu-id="2e4eb-255">profession</span><span class="sxs-lookup"><span data-stu-id="2e4eb-255">profession</span></span>|<span data-ttu-id="2e4eb-256">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-256">String</span></span>|<span data-ttu-id="2e4eb-257">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-257">The contact's profession.</span></span>|
|<span data-ttu-id="2e4eb-258">spouseName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-258">spouseName</span></span>|<span data-ttu-id="2e4eb-259">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-259">String</span></span>|<span data-ttu-id="2e4eb-260">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-260">The name of the contact's spouse.</span></span>|
|<span data-ttu-id="2e4eb-261">surname</span><span class="sxs-lookup"><span data-stu-id="2e4eb-261">surname</span></span>|<span data-ttu-id="2e4eb-262">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-262">String</span></span>|<span data-ttu-id="2e4eb-263">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-263">The contact's surname.</span></span>|
|<span data-ttu-id="2e4eb-264">title</span><span class="sxs-lookup"><span data-stu-id="2e4eb-264">title</span></span>|<span data-ttu-id="2e4eb-265">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-265">String</span></span>|<span data-ttu-id="2e4eb-266">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-266">The contact's title.</span></span>|
|<span data-ttu-id="2e4eb-267">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-267">yomiCompanyName</span></span>|<span data-ttu-id="2e4eb-268">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-268">String</span></span>|<span data-ttu-id="2e4eb-269">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-269">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="2e4eb-270">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="2e4eb-270">yomiGivenName</span></span>|<span data-ttu-id="2e4eb-271">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-271">String</span></span>|<span data-ttu-id="2e4eb-272">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-272">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="2e4eb-273">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="2e4eb-273">yomiSurname</span></span>|<span data-ttu-id="2e4eb-274">String</span><span class="sxs-lookup"><span data-stu-id="2e4eb-274">String</span></span>|<span data-ttu-id="2e4eb-275">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-275">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2e4eb-276">关系</span><span class="sxs-lookup"><span data-stu-id="2e4eb-276">Relationships</span></span>
| <span data-ttu-id="2e4eb-277">关系</span><span class="sxs-lookup"><span data-stu-id="2e4eb-277">Relationship</span></span> | <span data-ttu-id="2e4eb-278">类型</span><span class="sxs-lookup"><span data-stu-id="2e4eb-278">Type</span></span>   |<span data-ttu-id="2e4eb-279">说明</span><span class="sxs-lookup"><span data-stu-id="2e4eb-279">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2e4eb-280">extensions</span><span class="sxs-lookup"><span data-stu-id="2e4eb-280">extensions</span></span>|<span data-ttu-id="2e4eb-281">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="2e4eb-281">[extension](extension.md) collection</span></span>|<span data-ttu-id="2e4eb-p107">为联系人定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p107">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="2e4eb-285">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2e4eb-285">multiValueExtendedProperties</span></span>|<span data-ttu-id="2e4eb-286">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="2e4eb-286">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2e4eb-p108">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p108">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="2e4eb-290">照片</span><span class="sxs-lookup"><span data-stu-id="2e4eb-290">photo</span></span>|[<span data-ttu-id="2e4eb-291">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="2e4eb-291">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="2e4eb-p109">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p109">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="2e4eb-294">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="2e4eb-294">singleValueExtendedProperties</span></span>|<span data-ttu-id="2e4eb-295">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="2e4eb-295">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="2e4eb-p110">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-p110">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2e4eb-299">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e4eb-299">JSON representation</span></span>

<span data-ttu-id="2e4eb-300">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e4eb-300">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "businessAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "businessHomePage": "string",
  "businessPhones": ["string"],
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.emailAddress"}],
  "fileAs": "string",
  "generation": "string",
  "givenName": "string",
  "homeAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "homePhones": ["string"],
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "mobilePhone": "string",
  "nickName": "string",
  "officeLocation": "string",
  "otherAddress": {"@odata.type": "microsoft.graph.physicalAddress"},
  "parentFolderId": "string",
  "personalNotes": "string",
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string",

  "photo": { "@odata.type": "microsoft.graph.profilePhoto" }
}

```

## <a name="see-also"></a><span data-ttu-id="2e4eb-301">另请参阅</span><span class="sxs-lookup"><span data-stu-id="2e4eb-301">See also</span></span>

- [<span data-ttu-id="2e4eb-302">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="2e4eb-302">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="2e4eb-303">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="2e4eb-303">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="2e4eb-304">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e4eb-304">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="2e4eb-305">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e4eb-305">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="2e4eb-306">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="2e4eb-306">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
