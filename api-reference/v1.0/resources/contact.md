# <a name="contact-resource-type"></a><span data-ttu-id="89617-101">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="89617-101">contact resource type</span></span>

<span data-ttu-id="89617-p101">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="89617-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="89617-104">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="89617-104">This resource supports:</span></span>

- <span data-ttu-id="89617-105">在[扩展](../../../concepts/extensibility_overview.md)中添加您自己的数据作为自定义属性。</span><span class="sxs-lookup"><span data-stu-id="89617-105">Adding your own data to custom properties using [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="89617-106">订阅 [更改通知](../../../concepts/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="89617-106">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="89617-107">通过提供 [delta](../api/contact_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="89617-107">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="89617-108">方法</span><span class="sxs-lookup"><span data-stu-id="89617-108">Methods</span></span>

| <span data-ttu-id="89617-109">方法</span><span class="sxs-lookup"><span data-stu-id="89617-109">Method</span></span>       | <span data-ttu-id="89617-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="89617-110">Return Type</span></span>  |<span data-ttu-id="89617-111">说明</span><span class="sxs-lookup"><span data-stu-id="89617-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="89617-112">获取联系人</span><span class="sxs-lookup"><span data-stu-id="89617-112">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="89617-113">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-113">contact</span></span>](contact.md) |<span data-ttu-id="89617-114">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="89617-114">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="89617-115">创建</span><span class="sxs-lookup"><span data-stu-id="89617-115">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="89617-116">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-116">contact</span></span>](contact.md) |<span data-ttu-id="89617-117">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="89617-117">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="89617-118">更新</span><span class="sxs-lookup"><span data-stu-id="89617-118">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="89617-119">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-119">contact</span></span>](contact.md) |<span data-ttu-id="89617-120">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="89617-120">Update contact object.</span></span> |
|[<span data-ttu-id="89617-121">删除</span><span class="sxs-lookup"><span data-stu-id="89617-121">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="89617-122">无</span><span class="sxs-lookup"><span data-stu-id="89617-122">None</span></span> |<span data-ttu-id="89617-123">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="89617-123">Delete contact object.</span></span> |
|[<span data-ttu-id="89617-124">delta</span><span class="sxs-lookup"><span data-stu-id="89617-124">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="89617-125">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="89617-125">[contact](contact.md) collection</span></span>| <span data-ttu-id="89617-126">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="89617-126">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="89617-127">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="89617-127">**Open extensions**</span></span>| | |
|[<span data-ttu-id="89617-128">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="89617-128">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="89617-129">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="89617-129">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="89617-130">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="89617-130">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="89617-131">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="89617-131">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="89617-132">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89617-132">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="89617-133">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="89617-133">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="89617-134">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="89617-134">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="89617-135">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="89617-135">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="89617-136">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="89617-136">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="89617-137">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="89617-137">**Extended properties**</span></span>| | |
|[<span data-ttu-id="89617-138">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="89617-138">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="89617-139">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-139">contact</span></span>](contact.md)  |<span data-ttu-id="89617-140">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="89617-140">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="89617-141">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="89617-141">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="89617-142">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-142">contact</span></span>](contact.md) | <span data-ttu-id="89617-143">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="89617-143">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="89617-144">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="89617-144">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="89617-145">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-145">contact</span></span>](contact.md) | <span data-ttu-id="89617-146">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="89617-146">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="89617-147">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="89617-147">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="89617-148">联系人</span><span class="sxs-lookup"><span data-stu-id="89617-148">contact</span></span>](contact.md) | <span data-ttu-id="89617-149">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="89617-149">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="89617-150">属性</span><span class="sxs-lookup"><span data-stu-id="89617-150">Properties</span></span>
| <span data-ttu-id="89617-151">属性</span><span class="sxs-lookup"><span data-stu-id="89617-151">Property</span></span>     | <span data-ttu-id="89617-152">类型</span><span class="sxs-lookup"><span data-stu-id="89617-152">Type</span></span>   |<span data-ttu-id="89617-153">说明</span><span class="sxs-lookup"><span data-stu-id="89617-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89617-154">assistantName</span><span class="sxs-lookup"><span data-stu-id="89617-154">assistantName</span></span>|<span data-ttu-id="89617-155">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-155">String</span></span>|<span data-ttu-id="89617-156">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="89617-156">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="89617-157">birthday</span><span class="sxs-lookup"><span data-stu-id="89617-157">birthday</span></span>|<span data-ttu-id="89617-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89617-158">DateTimeOffset</span></span>|<span data-ttu-id="89617-p102">联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="89617-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="89617-162">businessAddress</span><span class="sxs-lookup"><span data-stu-id="89617-162">businessAddress</span></span>|[<span data-ttu-id="89617-163">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="89617-163">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="89617-164">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="89617-164">The contact's business address.</span></span>|
|<span data-ttu-id="89617-165">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="89617-165">businessHomePage</span></span>|<span data-ttu-id="89617-166">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-166">String</span></span>|<span data-ttu-id="89617-167">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="89617-167">The business home page of the contact.</span></span>|
|<span data-ttu-id="89617-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="89617-168">businessPhones</span></span>|<span data-ttu-id="89617-169">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89617-169">String collection</span></span>|<span data-ttu-id="89617-170">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="89617-170">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="89617-171">categories</span><span class="sxs-lookup"><span data-stu-id="89617-171">categories</span></span>|<span data-ttu-id="89617-172">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89617-172">String collection</span></span>|<span data-ttu-id="89617-173">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="89617-173">The categories associated with the contact.</span></span>|
|<span data-ttu-id="89617-174">changeKey</span><span class="sxs-lookup"><span data-stu-id="89617-174">changeKey</span></span>|<span data-ttu-id="89617-175">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-175">String</span></span>|<span data-ttu-id="89617-p103">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="89617-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="89617-179">children</span><span class="sxs-lookup"><span data-stu-id="89617-179">children</span></span>|<span data-ttu-id="89617-180">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89617-180">String collection</span></span>|<span data-ttu-id="89617-181">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="89617-181">The names of the contact's children.</span></span>|
|<span data-ttu-id="89617-182">companyName</span><span class="sxs-lookup"><span data-stu-id="89617-182">companyName</span></span>|<span data-ttu-id="89617-183">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-183">String</span></span>|<span data-ttu-id="89617-184">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="89617-184">The name of the contact's company.</span></span>|
|<span data-ttu-id="89617-185">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="89617-185">createdDateTime</span></span>|<span data-ttu-id="89617-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89617-186">DateTimeOffset</span></span>|<span data-ttu-id="89617-p104">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="89617-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="89617-190">department</span><span class="sxs-lookup"><span data-stu-id="89617-190">department</span></span>|<span data-ttu-id="89617-191">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-191">String</span></span>|<span data-ttu-id="89617-192">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="89617-192">The contact's department.</span></span>|
|<span data-ttu-id="89617-193">displayName</span><span class="sxs-lookup"><span data-stu-id="89617-193">displayName</span></span>|<span data-ttu-id="89617-194">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-194">String</span></span>|<span data-ttu-id="89617-195">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="89617-195">The contact's display name.</span></span>|
|<span data-ttu-id="89617-196">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="89617-196">emailAddresses</span></span>|<span data-ttu-id="89617-197">[EmailAddress](emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89617-197">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="89617-198">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="89617-198">The contact's email addresses.</span></span>|
|<span data-ttu-id="89617-199">flag</span><span class="sxs-lookup"><span data-stu-id="89617-199">flag</span></span>|[<span data-ttu-id="89617-200">followupFlag</span><span class="sxs-lookup"><span data-stu-id="89617-200">followUpFlag</span></span>](followupflag.md)|<span data-ttu-id="89617-201">指示邮件的状态、开始日期、截止日期或完成日期的标记值。</span><span class="sxs-lookup"><span data-stu-id="89617-201">The flag value that indicates the status, start date, due date, or completion date for the message.</span></span>|
|<span data-ttu-id="89617-202">fileAs</span><span class="sxs-lookup"><span data-stu-id="89617-202">fileAs</span></span>|<span data-ttu-id="89617-203">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-203">String</span></span>|<span data-ttu-id="89617-204">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="89617-204">The name the contact is filed under.</span></span>|
|<span data-ttu-id="89617-205">generation</span><span class="sxs-lookup"><span data-stu-id="89617-205">generation</span></span>|<span data-ttu-id="89617-206">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-206">String</span></span>|<span data-ttu-id="89617-207">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="89617-207">The contact's generation.</span></span>|
|<span data-ttu-id="89617-208">givenName</span><span class="sxs-lookup"><span data-stu-id="89617-208">givenName</span></span>|<span data-ttu-id="89617-209">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-209">String</span></span>|<span data-ttu-id="89617-210">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="89617-210">The contact's given name.</span></span>|
|<span data-ttu-id="89617-211">homeAddress</span><span class="sxs-lookup"><span data-stu-id="89617-211">homeAddress</span></span>|[<span data-ttu-id="89617-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="89617-212">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="89617-213">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="89617-213">The contact's home address.</span></span>|
|<span data-ttu-id="89617-214">homePhones</span><span class="sxs-lookup"><span data-stu-id="89617-214">homePhones</span></span>|<span data-ttu-id="89617-215">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89617-215">String collection</span></span>|<span data-ttu-id="89617-216">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="89617-216">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="89617-217">id</span><span class="sxs-lookup"><span data-stu-id="89617-217">id</span></span>|<span data-ttu-id="89617-218">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-218">String</span></span>|<span data-ttu-id="89617-p105">联系人的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="89617-p105">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="89617-221">imAddresses</span><span class="sxs-lookup"><span data-stu-id="89617-221">imAddresses</span></span>|<span data-ttu-id="89617-222">字符串集合</span><span class="sxs-lookup"><span data-stu-id="89617-222">String collection</span></span>|<span data-ttu-id="89617-223">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="89617-223">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="89617-224">initials</span><span class="sxs-lookup"><span data-stu-id="89617-224">initials</span></span>|<span data-ttu-id="89617-225">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-225">String</span></span>|<span data-ttu-id="89617-226">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="89617-226">The contact's initials.</span></span>|
|<span data-ttu-id="89617-227">jobTitle</span><span class="sxs-lookup"><span data-stu-id="89617-227">jobTitle</span></span>|<span data-ttu-id="89617-228">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-228">String</span></span>|<span data-ttu-id="89617-229">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="89617-229">The contact’s job title.</span></span>|
|<span data-ttu-id="89617-230">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="89617-230">lastModifiedDateTime</span></span>|<span data-ttu-id="89617-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="89617-231">DateTimeOffset</span></span>|<span data-ttu-id="89617-p106">修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式： `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="89617-p106">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="89617-235">manager</span><span class="sxs-lookup"><span data-stu-id="89617-235">manager</span></span>|<span data-ttu-id="89617-236">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-236">String</span></span>|<span data-ttu-id="89617-237">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="89617-237">The name of the contact's manager.</span></span>
|<span data-ttu-id="89617-238">middleName</span><span class="sxs-lookup"><span data-stu-id="89617-238">middleName</span></span>|<span data-ttu-id="89617-239">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-239">String</span></span>|<span data-ttu-id="89617-240">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="89617-240">The contact's middle name.</span></span>|
|<span data-ttu-id="89617-241">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="89617-241">mobilePhone</span></span>|<span data-ttu-id="89617-242">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-242">String</span></span>|<span data-ttu-id="89617-243">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="89617-243">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="89617-244">nickName</span><span class="sxs-lookup"><span data-stu-id="89617-244">nickName</span></span>|<span data-ttu-id="89617-245">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-245">String</span></span>|<span data-ttu-id="89617-246">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="89617-246">The contact's nickname.</span></span>|
|<span data-ttu-id="89617-247">officeLocation</span><span class="sxs-lookup"><span data-stu-id="89617-247">officeLocation</span></span>|<span data-ttu-id="89617-248">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-248">String</span></span>|<span data-ttu-id="89617-249">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="89617-249">The location of the contact's office.</span></span>|
|<span data-ttu-id="89617-250">otherAddress</span><span class="sxs-lookup"><span data-stu-id="89617-250">otherAddress</span></span>|[<span data-ttu-id="89617-251">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="89617-251">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="89617-252">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="89617-252">Other addresses for the contact.</span></span>|
|<span data-ttu-id="89617-253">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="89617-253">parentFolderId</span></span>|<span data-ttu-id="89617-254">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-254">String</span></span>|<span data-ttu-id="89617-255">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="89617-255">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="89617-256">personalNotes</span><span class="sxs-lookup"><span data-stu-id="89617-256">personalNotes</span></span>|<span data-ttu-id="89617-257">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-257">String</span></span>|<span data-ttu-id="89617-258">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="89617-258">The user's notes about the contact.</span></span>|
|<span data-ttu-id="89617-259">profession</span><span class="sxs-lookup"><span data-stu-id="89617-259">profession</span></span>|<span data-ttu-id="89617-260">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-260">String</span></span>|<span data-ttu-id="89617-261">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="89617-261">The contact's profession.</span></span>|
|<span data-ttu-id="89617-262">spouseName</span><span class="sxs-lookup"><span data-stu-id="89617-262">spouseName</span></span>|<span data-ttu-id="89617-263">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-263">String</span></span>|<span data-ttu-id="89617-264">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="89617-264">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="89617-265">surname</span><span class="sxs-lookup"><span data-stu-id="89617-265">surname</span></span>|<span data-ttu-id="89617-266">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-266">String</span></span>|<span data-ttu-id="89617-267">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="89617-267">The contact's surname.</span></span>|
|<span data-ttu-id="89617-268">title</span><span class="sxs-lookup"><span data-stu-id="89617-268">title</span></span>|<span data-ttu-id="89617-269">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-269">String</span></span>|<span data-ttu-id="89617-270">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="89617-270">The contact's title.</span></span>|
|<span data-ttu-id="89617-271">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="89617-271">yomiCompanyName</span></span>|<span data-ttu-id="89617-272">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-272">String</span></span>|<span data-ttu-id="89617-273">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="89617-273">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="89617-274">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="89617-274">yomiGivenName</span></span>|<span data-ttu-id="89617-275">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-275">String</span></span>|<span data-ttu-id="89617-276">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="89617-276">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="89617-277">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="89617-277">yomiSurname</span></span>|<span data-ttu-id="89617-278">字符串</span><span class="sxs-lookup"><span data-stu-id="89617-278">String</span></span>|<span data-ttu-id="89617-279">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="89617-279">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="89617-280">关系</span><span class="sxs-lookup"><span data-stu-id="89617-280">Relationships</span></span>
| <span data-ttu-id="89617-281">关系</span><span class="sxs-lookup"><span data-stu-id="89617-281">Relationship</span></span> | <span data-ttu-id="89617-282">类型</span><span class="sxs-lookup"><span data-stu-id="89617-282">Type</span></span>   |<span data-ttu-id="89617-283">说明</span><span class="sxs-lookup"><span data-stu-id="89617-283">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89617-284">extensions</span><span class="sxs-lookup"><span data-stu-id="89617-284">extensions</span></span>|<span data-ttu-id="89617-285">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="89617-285">[extension](extension.md) collection</span></span>|<span data-ttu-id="89617-p107">为联系人定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="89617-p107">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="89617-289">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="89617-289">multiValueExtendedProperties</span></span>|<span data-ttu-id="89617-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89617-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="89617-p108">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="89617-p108">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="89617-294">photo</span><span class="sxs-lookup"><span data-stu-id="89617-294">photo</span></span>|[<span data-ttu-id="89617-295">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="89617-295">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="89617-p109">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="89617-p109">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="89617-298">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="89617-298">singleValueExtendedProperties</span></span>|<span data-ttu-id="89617-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89617-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="89617-p110">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="89617-p110">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89617-303">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89617-303">JSON representation</span></span>

<span data-ttu-id="89617-304">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89617-304">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.outlookItem",
  "openType": true,
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.contact",
  "@odata.annotations": [
    {
      "property": "extensions",
      "capabilities": {
        "changeTracking": false,
        "searchable": false
      }
    },
    {
      "property": "photo",
      "capabilities": {
        "changeTracking": false,
        "deletable": false,
        "expandable": false,
        "insertable": false,
        "searchable": false
      }
    }
  ]
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
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
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

## <a name="see-also"></a><span data-ttu-id="89617-305">另请参阅</span><span class="sxs-lookup"><span data-stu-id="89617-305">See also</span></span>

- [<span data-ttu-id="89617-306">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="89617-306">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="89617-307">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="89617-307">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="89617-308">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="89617-308">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="89617-309">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="89617-309">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="89617-310">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="89617-310">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
