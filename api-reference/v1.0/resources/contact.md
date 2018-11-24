# <a name="contact-resource-type"></a><span data-ttu-id="dd7ab-101">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="dd7ab-101">contact resource type</span></span>

<span data-ttu-id="dd7ab-p101">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p101">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="dd7ab-104">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="dd7ab-104">This resource supports:</span></span>

- <span data-ttu-id="dd7ab-105">将您自己的数据添加到自定义属性，作为[扩展](../../../concepts/extensibility_overview.md)。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-105">Adding your own data to custom properties as [extensions](../../../concepts/extensibility_overview.md).</span></span>
- <span data-ttu-id="dd7ab-106">订阅[更改通知](../../../concepts/webhooks.md)。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-106">Subscribing to [change notifications](../../../concepts/webhooks.md).</span></span>
- <span data-ttu-id="dd7ab-107">通过提供 [delta](../api/contact_delta.md) 函数使用[增量查询](../../../concepts/delta_query_overview.md)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-107">Using [delta query](../../../concepts/delta_query_overview.md) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact_delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="dd7ab-108">方法</span><span class="sxs-lookup"><span data-stu-id="dd7ab-108">Methods</span></span>

| <span data-ttu-id="dd7ab-109">方法</span><span class="sxs-lookup"><span data-stu-id="dd7ab-109">Method</span></span>       | <span data-ttu-id="dd7ab-110">返回类型</span><span class="sxs-lookup"><span data-stu-id="dd7ab-110">Return Type</span></span>  |<span data-ttu-id="dd7ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="dd7ab-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="dd7ab-112">获取联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-112">Get contact</span></span>](../api/contact_get.md) | [<span data-ttu-id="dd7ab-113">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-113">contact</span></span>](contact.md) |<span data-ttu-id="dd7ab-114">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-114">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="dd7ab-115">创建</span><span class="sxs-lookup"><span data-stu-id="dd7ab-115">Create</span></span>](../api/user_post_contacts.md) | [<span data-ttu-id="dd7ab-116">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-116">contact</span></span>](contact.md) |<span data-ttu-id="dd7ab-117">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-117">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="dd7ab-118">更新</span><span class="sxs-lookup"><span data-stu-id="dd7ab-118">Update</span></span>](../api/contact_update.md) | [<span data-ttu-id="dd7ab-119">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-119">contact</span></span>](contact.md) |<span data-ttu-id="dd7ab-120">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-120">Update contact object.</span></span> |
|[<span data-ttu-id="dd7ab-121">删除</span><span class="sxs-lookup"><span data-stu-id="dd7ab-121">Delete</span></span>](../api/contact_delete.md) | <span data-ttu-id="dd7ab-122">无</span><span class="sxs-lookup"><span data-stu-id="dd7ab-122">None</span></span> |<span data-ttu-id="dd7ab-123">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-123">Delete contact object.</span></span> |
|[<span data-ttu-id="dd7ab-124">delta</span><span class="sxs-lookup"><span data-stu-id="dd7ab-124">delta</span></span>](../api/contact_delta.md)|<span data-ttu-id="dd7ab-125">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="dd7ab-125">[contact](contact.md) collection</span></span>| <span data-ttu-id="dd7ab-126">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-126">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="dd7ab-127">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="dd7ab-127">**Open extensions**</span></span>| | |
|[<span data-ttu-id="dd7ab-128">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="dd7ab-128">Create open extension</span></span>](../api/opentypeextension_post_opentypeextension.md) |[<span data-ttu-id="dd7ab-129">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="dd7ab-129">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="dd7ab-130">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-130">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="dd7ab-131">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="dd7ab-131">Get open extension</span></span>](../api/opentypeextension_get.md) |<span data-ttu-id="dd7ab-132">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd7ab-132">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="dd7ab-133">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-133">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="dd7ab-134">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="dd7ab-134">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="dd7ab-135">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="dd7ab-135">Add schema extension values</span></span>](../../../concepts/extensibility_schema_groups.md) || <span data-ttu-id="dd7ab-136">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-136">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="dd7ab-137">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="dd7ab-137">**Extended properties**</span></span>| | |
|[<span data-ttu-id="dd7ab-138">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="dd7ab-138">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_post_singlevalueextendedproperties.md) |[<span data-ttu-id="dd7ab-139">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-139">contact</span></span>](contact.md)  |<span data-ttu-id="dd7ab-140">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-140">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="dd7ab-141">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-141">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="dd7ab-142">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-142">contact</span></span>](contact.md) | <span data-ttu-id="dd7ab-143">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-143">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="dd7ab-144">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="dd7ab-144">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_post_multivalueextendedproperties.md) | [<span data-ttu-id="dd7ab-145">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-145">contact</span></span>](contact.md) | <span data-ttu-id="dd7ab-146">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-146">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="dd7ab-147">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-147">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty_get.md)  | [<span data-ttu-id="dd7ab-148">联系人</span><span class="sxs-lookup"><span data-stu-id="dd7ab-148">contact</span></span>](contact.md) | <span data-ttu-id="dd7ab-149">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-149">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="dd7ab-150">属性</span><span class="sxs-lookup"><span data-stu-id="dd7ab-150">Properties</span></span>
| <span data-ttu-id="dd7ab-151">属性</span><span class="sxs-lookup"><span data-stu-id="dd7ab-151">Property</span></span>     | <span data-ttu-id="dd7ab-152">类型</span><span class="sxs-lookup"><span data-stu-id="dd7ab-152">Type</span></span>   |<span data-ttu-id="dd7ab-153">说明</span><span class="sxs-lookup"><span data-stu-id="dd7ab-153">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd7ab-154">assistantName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-154">assistantName</span></span>|<span data-ttu-id="dd7ab-155">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-155">String</span></span>|<span data-ttu-id="dd7ab-156">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-156">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="dd7ab-157">birthday</span><span class="sxs-lookup"><span data-stu-id="dd7ab-157">birthday</span></span>|<span data-ttu-id="dd7ab-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7ab-158">DateTimeOffset</span></span>|<span data-ttu-id="dd7ab-p102">联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p102">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dd7ab-162">businessAddress</span><span class="sxs-lookup"><span data-stu-id="dd7ab-162">businessAddress</span></span>|[<span data-ttu-id="dd7ab-163">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="dd7ab-163">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="dd7ab-164">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-164">The contact's business address.</span></span>|
|<span data-ttu-id="dd7ab-165">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="dd7ab-165">businessHomePage</span></span>|<span data-ttu-id="dd7ab-166">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-166">String</span></span>|<span data-ttu-id="dd7ab-167">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-167">The business home page of the contact.</span></span>|
|<span data-ttu-id="dd7ab-168">businessPhones</span><span class="sxs-lookup"><span data-stu-id="dd7ab-168">businessPhones</span></span>|<span data-ttu-id="dd7ab-169">String collection</span><span class="sxs-lookup"><span data-stu-id="dd7ab-169">String collection</span></span>|<span data-ttu-id="dd7ab-170">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-170">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="dd7ab-171">categories</span><span class="sxs-lookup"><span data-stu-id="dd7ab-171">categories</span></span>|<span data-ttu-id="dd7ab-172">String collection</span><span class="sxs-lookup"><span data-stu-id="dd7ab-172">String collection</span></span>|<span data-ttu-id="dd7ab-173">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-173">The categories associated with the contact.</span></span>|
|<span data-ttu-id="dd7ab-174">changeKey</span><span class="sxs-lookup"><span data-stu-id="dd7ab-174">changeKey</span></span>|<span data-ttu-id="dd7ab-175">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-175">String</span></span>|<span data-ttu-id="dd7ab-p103">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p103">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="dd7ab-179">children</span><span class="sxs-lookup"><span data-stu-id="dd7ab-179">children</span></span>|<span data-ttu-id="dd7ab-180">String collection</span><span class="sxs-lookup"><span data-stu-id="dd7ab-180">String collection</span></span>|<span data-ttu-id="dd7ab-181">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-181">The names of the contact's children.</span></span>|
|<span data-ttu-id="dd7ab-182">companyName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-182">companyName</span></span>|<span data-ttu-id="dd7ab-183">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-183">String</span></span>|<span data-ttu-id="dd7ab-184">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-184">The name of the contact's company.</span></span>|
|<span data-ttu-id="dd7ab-185">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7ab-185">createdDateTime</span></span>|<span data-ttu-id="dd7ab-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7ab-186">DateTimeOffset</span></span>|<span data-ttu-id="dd7ab-p104">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p104">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dd7ab-190">部门</span><span class="sxs-lookup"><span data-stu-id="dd7ab-190">department</span></span>|<span data-ttu-id="dd7ab-191">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-191">String</span></span>|<span data-ttu-id="dd7ab-192">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-192">The contact's department.</span></span>|
|<span data-ttu-id="dd7ab-193">displayName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-193">displayName</span></span>|<span data-ttu-id="dd7ab-194">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-194">String</span></span>|<span data-ttu-id="dd7ab-195">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-195">The contact's display name.</span></span> <span data-ttu-id="dd7ab-196">您可以[创建](../api/user_post_contacts.md)或[更新](../api/contact_update.md)操作中指定的显示名称。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-196">You can specify the display name in a [create](../api/user_post_contacts.md) or [update](../api/contact_update.md) operation.</span></span> <span data-ttu-id="dd7ab-197">请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-197">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="dd7ab-198">若要保留现有的值，请始终作为[更新](../api/contact_update.md)操作中的 displayName 包括它。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-198">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact_update.md) operation.</span></span>|
|<span data-ttu-id="dd7ab-199">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="dd7ab-199">emailAddresses</span></span>|<span data-ttu-id="dd7ab-200">[EmailAddress](emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd7ab-200">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="dd7ab-201">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-201">The contact's email addresses.</span></span>|
|<span data-ttu-id="dd7ab-202">fileAs</span><span class="sxs-lookup"><span data-stu-id="dd7ab-202">fileAs</span></span>|<span data-ttu-id="dd7ab-203">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-203">String</span></span>|<span data-ttu-id="dd7ab-204">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-204">The name the contact is filed under.</span></span>|
|<span data-ttu-id="dd7ab-205">generation</span><span class="sxs-lookup"><span data-stu-id="dd7ab-205">generation</span></span>|<span data-ttu-id="dd7ab-206">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-206">String</span></span>|<span data-ttu-id="dd7ab-207">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-207">The contact's generation.</span></span>|
|<span data-ttu-id="dd7ab-208">givenName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-208">givenName</span></span>|<span data-ttu-id="dd7ab-209">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-209">String</span></span>|<span data-ttu-id="dd7ab-210">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-210">The contact's given name.</span></span>|
|<span data-ttu-id="dd7ab-211">homeAddress</span><span class="sxs-lookup"><span data-stu-id="dd7ab-211">homeAddress</span></span>|[<span data-ttu-id="dd7ab-212">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="dd7ab-212">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="dd7ab-213">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-213">The contact's home address.</span></span>|
|<span data-ttu-id="dd7ab-214">homePhones</span><span class="sxs-lookup"><span data-stu-id="dd7ab-214">homePhones</span></span>|<span data-ttu-id="dd7ab-215">String collection</span><span class="sxs-lookup"><span data-stu-id="dd7ab-215">String collection</span></span>|<span data-ttu-id="dd7ab-216">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-216">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="dd7ab-217">id</span><span class="sxs-lookup"><span data-stu-id="dd7ab-217">id</span></span>|<span data-ttu-id="dd7ab-218">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-218">String</span></span>|<span data-ttu-id="dd7ab-p106">联系人的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p106">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="dd7ab-221">imAddresses</span><span class="sxs-lookup"><span data-stu-id="dd7ab-221">imAddresses</span></span>|<span data-ttu-id="dd7ab-222">String collection</span><span class="sxs-lookup"><span data-stu-id="dd7ab-222">String collection</span></span>|<span data-ttu-id="dd7ab-223">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-223">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="dd7ab-224">initials</span><span class="sxs-lookup"><span data-stu-id="dd7ab-224">initials</span></span>|<span data-ttu-id="dd7ab-225">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-225">String</span></span>|<span data-ttu-id="dd7ab-226">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-226">The contact's initials.</span></span>|
|<span data-ttu-id="dd7ab-227">jobTitle</span><span class="sxs-lookup"><span data-stu-id="dd7ab-227">jobTitle</span></span>|<span data-ttu-id="dd7ab-228">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-228">String</span></span>|<span data-ttu-id="dd7ab-229">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-229">The contact’s job title.</span></span>|
|<span data-ttu-id="dd7ab-230">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd7ab-230">lastModifiedDateTime</span></span>|<span data-ttu-id="dd7ab-231">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd7ab-231">DateTimeOffset</span></span>|<span data-ttu-id="dd7ab-p107">修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p107">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="dd7ab-235">manager</span><span class="sxs-lookup"><span data-stu-id="dd7ab-235">manager</span></span>|<span data-ttu-id="dd7ab-236">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-236">String</span></span>|<span data-ttu-id="dd7ab-237">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-237">The name of the contact's manager.</span></span>
|<span data-ttu-id="dd7ab-238">middleName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-238">middleName</span></span>|<span data-ttu-id="dd7ab-239">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-239">String</span></span>|<span data-ttu-id="dd7ab-240">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-240">The contact's middle name.</span></span>|
|<span data-ttu-id="dd7ab-241">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="dd7ab-241">mobilePhone</span></span>|<span data-ttu-id="dd7ab-242">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-242">String</span></span>|<span data-ttu-id="dd7ab-243">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-243">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="dd7ab-244">nickName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-244">nickName</span></span>|<span data-ttu-id="dd7ab-245">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-245">String</span></span>|<span data-ttu-id="dd7ab-246">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-246">The contact's nickname.</span></span>|
|<span data-ttu-id="dd7ab-247">officeLocation</span><span class="sxs-lookup"><span data-stu-id="dd7ab-247">officeLocation</span></span>|<span data-ttu-id="dd7ab-248">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-248">String</span></span>|<span data-ttu-id="dd7ab-249">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-249">The location of the contact's office.</span></span>|
|<span data-ttu-id="dd7ab-250">otherAddress</span><span class="sxs-lookup"><span data-stu-id="dd7ab-250">otherAddress</span></span>|[<span data-ttu-id="dd7ab-251">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="dd7ab-251">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="dd7ab-252">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-252">Other addresses for the contact.</span></span>|
|<span data-ttu-id="dd7ab-253">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="dd7ab-253">parentFolderId</span></span>|<span data-ttu-id="dd7ab-254">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-254">String</span></span>|<span data-ttu-id="dd7ab-255">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-255">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="dd7ab-256">personalNotes</span><span class="sxs-lookup"><span data-stu-id="dd7ab-256">personalNotes</span></span>|<span data-ttu-id="dd7ab-257">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-257">String</span></span>|<span data-ttu-id="dd7ab-258">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-258">The user's notes about the contact.</span></span>|
|<span data-ttu-id="dd7ab-259">profession</span><span class="sxs-lookup"><span data-stu-id="dd7ab-259">profession</span></span>|<span data-ttu-id="dd7ab-260">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-260">String</span></span>|<span data-ttu-id="dd7ab-261">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-261">The contact's profession.</span></span>|
|<span data-ttu-id="dd7ab-262">spouseName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-262">spouseName</span></span>|<span data-ttu-id="dd7ab-263">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-263">String</span></span>|<span data-ttu-id="dd7ab-264">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-264">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="dd7ab-265">surname</span><span class="sxs-lookup"><span data-stu-id="dd7ab-265">surname</span></span>|<span data-ttu-id="dd7ab-266">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-266">String</span></span>|<span data-ttu-id="dd7ab-267">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-267">The contact's surname.</span></span>|
|<span data-ttu-id="dd7ab-268">title</span><span class="sxs-lookup"><span data-stu-id="dd7ab-268">title</span></span>|<span data-ttu-id="dd7ab-269">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-269">String</span></span>|<span data-ttu-id="dd7ab-270">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-270">The contact's title.</span></span>|
|<span data-ttu-id="dd7ab-271">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-271">yomiCompanyName</span></span>|<span data-ttu-id="dd7ab-272">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-272">String</span></span>|<span data-ttu-id="dd7ab-273">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-273">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="dd7ab-274">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="dd7ab-274">yomiGivenName</span></span>|<span data-ttu-id="dd7ab-275">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-275">String</span></span>|<span data-ttu-id="dd7ab-276">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-276">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="dd7ab-277">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="dd7ab-277">yomiSurname</span></span>|<span data-ttu-id="dd7ab-278">String</span><span class="sxs-lookup"><span data-stu-id="dd7ab-278">String</span></span>|<span data-ttu-id="dd7ab-279">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-279">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd7ab-280">Relationships</span><span class="sxs-lookup"><span data-stu-id="dd7ab-280">Relationships</span></span>
| <span data-ttu-id="dd7ab-281">关系</span><span class="sxs-lookup"><span data-stu-id="dd7ab-281">Relationship</span></span> | <span data-ttu-id="dd7ab-282">类型</span><span class="sxs-lookup"><span data-stu-id="dd7ab-282">Type</span></span>   |<span data-ttu-id="dd7ab-283">说明</span><span class="sxs-lookup"><span data-stu-id="dd7ab-283">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dd7ab-284">extensions</span><span class="sxs-lookup"><span data-stu-id="dd7ab-284">extensions</span></span>|<span data-ttu-id="dd7ab-285">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="dd7ab-285">[extension](extension.md) collection</span></span>|<span data-ttu-id="dd7ab-p108">为联系人定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p108">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="dd7ab-289">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="dd7ab-289">multiValueExtendedProperties</span></span>|<span data-ttu-id="dd7ab-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="dd7ab-290">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="dd7ab-p109">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p109">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="dd7ab-294">photo</span><span class="sxs-lookup"><span data-stu-id="dd7ab-294">photo</span></span>|[<span data-ttu-id="dd7ab-295">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="dd7ab-295">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="dd7ab-p110">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p110">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="dd7ab-298">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="dd7ab-298">singleValueExtendedProperties</span></span>|<span data-ttu-id="dd7ab-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="dd7ab-299">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="dd7ab-p111">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-p111">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="dd7ab-303">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd7ab-303">JSON representation</span></span>

<span data-ttu-id="dd7ab-304">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd7ab-304">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="dd7ab-305">另请参阅</span><span class="sxs-lookup"><span data-stu-id="dd7ab-305">See also</span></span>

- [<span data-ttu-id="dd7ab-306">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="dd7ab-306">Use delta query to track changes in Microsoft Graph data</span></span>](../../../concepts/delta_query_overview.md)
- [<span data-ttu-id="dd7ab-307">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="dd7ab-307">Get incremental changes to messages in a folder</span></span>](../../../concepts/delta_query_messages.md)
- [<span data-ttu-id="dd7ab-308">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="dd7ab-308">Add custom data to resources using extensions</span></span>](../../../concepts/extensibility_overview.md)
- [<span data-ttu-id="dd7ab-309">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="dd7ab-309">Add custom data to users using open extensions</span></span>](../../../concepts/extensibility_open_users.md)
- [<span data-ttu-id="dd7ab-310">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="dd7ab-310">Add custom data to groups using schema extensions</span></span>](../../../concepts/extensibility_schema_groups.md)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
