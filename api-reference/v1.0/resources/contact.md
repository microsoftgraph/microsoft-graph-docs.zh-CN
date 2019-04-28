---
title: 联系人资源类型
description: 联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 7b60333bec9bfca9d67fedc379e4a51ce768fba2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548101"
---
# <a name="contact-resource-type"></a><span data-ttu-id="99540-104">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="99540-104">contact resource type</span></span>

<span data-ttu-id="99540-p102">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="99540-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="99540-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="99540-107">This resource supports:</span></span>

- <span data-ttu-id="99540-108">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="99540-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="99540-109">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="99540-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="99540-110">通过提供 [delta](../api/contact-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="99540-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="99540-111">方法</span><span class="sxs-lookup"><span data-stu-id="99540-111">Methods</span></span>

| <span data-ttu-id="99540-112">方法</span><span class="sxs-lookup"><span data-stu-id="99540-112">Method</span></span>       | <span data-ttu-id="99540-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="99540-113">Return Type</span></span>  |<span data-ttu-id="99540-114">说明</span><span class="sxs-lookup"><span data-stu-id="99540-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="99540-115">获取联系人</span><span class="sxs-lookup"><span data-stu-id="99540-115">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="99540-116">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-116">contact</span></span>](contact.md) |<span data-ttu-id="99540-117">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99540-117">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="99540-118">创建</span><span class="sxs-lookup"><span data-stu-id="99540-118">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="99540-119">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-119">contact</span></span>](contact.md) |<span data-ttu-id="99540-120">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="99540-120">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="99540-121">更新</span><span class="sxs-lookup"><span data-stu-id="99540-121">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="99540-122">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-122">contact</span></span>](contact.md) |<span data-ttu-id="99540-123">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="99540-123">Update contact object.</span></span> |
|[<span data-ttu-id="99540-124">删除</span><span class="sxs-lookup"><span data-stu-id="99540-124">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="99540-125">无</span><span class="sxs-lookup"><span data-stu-id="99540-125">None</span></span> |<span data-ttu-id="99540-126">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="99540-126">Delete contact object.</span></span> |
|[<span data-ttu-id="99540-127">delta</span><span class="sxs-lookup"><span data-stu-id="99540-127">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="99540-128">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="99540-128">[contact](contact.md) collection</span></span>| <span data-ttu-id="99540-129">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="99540-129">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="99540-130">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="99540-130">**Open extensions**</span></span>| | |
|[<span data-ttu-id="99540-131">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="99540-131">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="99540-132">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="99540-132">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="99540-133">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="99540-133">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="99540-134">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="99540-134">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="99540-135">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99540-135">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="99540-136">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="99540-136">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="99540-137">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="99540-137">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="99540-138">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="99540-138">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="99540-139">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="99540-139">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="99540-140">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="99540-140">**Extended properties**</span></span>| | |
|[<span data-ttu-id="99540-141">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="99540-141">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="99540-142">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-142">contact</span></span>](contact.md)  |<span data-ttu-id="99540-143">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="99540-143">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="99540-144">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="99540-144">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="99540-145">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-145">contact</span></span>](contact.md) | <span data-ttu-id="99540-146">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="99540-146">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="99540-147">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="99540-147">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="99540-148">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-148">contact</span></span>](contact.md) | <span data-ttu-id="99540-149">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="99540-149">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="99540-150">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="99540-150">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="99540-151">联系人</span><span class="sxs-lookup"><span data-stu-id="99540-151">contact</span></span>](contact.md) | <span data-ttu-id="99540-152">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="99540-152">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="99540-153">属性</span><span class="sxs-lookup"><span data-stu-id="99540-153">Properties</span></span>
| <span data-ttu-id="99540-154">属性</span><span class="sxs-lookup"><span data-stu-id="99540-154">Property</span></span>     | <span data-ttu-id="99540-155">类型</span><span class="sxs-lookup"><span data-stu-id="99540-155">Type</span></span>   |<span data-ttu-id="99540-156">说明</span><span class="sxs-lookup"><span data-stu-id="99540-156">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99540-157">assistantName</span><span class="sxs-lookup"><span data-stu-id="99540-157">assistantName</span></span>|<span data-ttu-id="99540-158">String</span><span class="sxs-lookup"><span data-stu-id="99540-158">String</span></span>|<span data-ttu-id="99540-159">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="99540-159">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="99540-160">birthday</span><span class="sxs-lookup"><span data-stu-id="99540-160">birthday</span></span>|<span data-ttu-id="99540-161">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99540-161">DateTimeOffset</span></span>|<span data-ttu-id="99540-p103">联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99540-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99540-165">businessAddress</span><span class="sxs-lookup"><span data-stu-id="99540-165">businessAddress</span></span>|[<span data-ttu-id="99540-166">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="99540-166">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="99540-167">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="99540-167">The contact's business address.</span></span>|
|<span data-ttu-id="99540-168">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="99540-168">businessHomePage</span></span>|<span data-ttu-id="99540-169">String</span><span class="sxs-lookup"><span data-stu-id="99540-169">String</span></span>|<span data-ttu-id="99540-170">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="99540-170">The business home page of the contact.</span></span>|
|<span data-ttu-id="99540-171">businessPhones</span><span class="sxs-lookup"><span data-stu-id="99540-171">businessPhones</span></span>|<span data-ttu-id="99540-172">String collection</span><span class="sxs-lookup"><span data-stu-id="99540-172">String collection</span></span>|<span data-ttu-id="99540-173">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="99540-173">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="99540-174">categories</span><span class="sxs-lookup"><span data-stu-id="99540-174">categories</span></span>|<span data-ttu-id="99540-175">String collection</span><span class="sxs-lookup"><span data-stu-id="99540-175">String collection</span></span>|<span data-ttu-id="99540-176">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="99540-176">The categories associated with the contact.</span></span>|
|<span data-ttu-id="99540-177">changeKey</span><span class="sxs-lookup"><span data-stu-id="99540-177">changeKey</span></span>|<span data-ttu-id="99540-178">String</span><span class="sxs-lookup"><span data-stu-id="99540-178">String</span></span>|<span data-ttu-id="99540-p104">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="99540-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="99540-182">children</span><span class="sxs-lookup"><span data-stu-id="99540-182">children</span></span>|<span data-ttu-id="99540-183">String collection</span><span class="sxs-lookup"><span data-stu-id="99540-183">String collection</span></span>|<span data-ttu-id="99540-184">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="99540-184">The names of the contact's children.</span></span>|
|<span data-ttu-id="99540-185">companyName</span><span class="sxs-lookup"><span data-stu-id="99540-185">companyName</span></span>|<span data-ttu-id="99540-186">String</span><span class="sxs-lookup"><span data-stu-id="99540-186">String</span></span>|<span data-ttu-id="99540-187">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="99540-187">The name of the contact's company.</span></span>|
|<span data-ttu-id="99540-188">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="99540-188">createdDateTime</span></span>|<span data-ttu-id="99540-189">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99540-189">DateTimeOffset</span></span>|<span data-ttu-id="99540-p105">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99540-p105">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99540-193">部门</span><span class="sxs-lookup"><span data-stu-id="99540-193">department</span></span>|<span data-ttu-id="99540-194">String</span><span class="sxs-lookup"><span data-stu-id="99540-194">String</span></span>|<span data-ttu-id="99540-195">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="99540-195">The contact's department.</span></span>|
|<span data-ttu-id="99540-196">displayName</span><span class="sxs-lookup"><span data-stu-id="99540-196">displayName</span></span>|<span data-ttu-id="99540-197">String</span><span class="sxs-lookup"><span data-stu-id="99540-197">String</span></span>|<span data-ttu-id="99540-198">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="99540-198">The contact's display name.</span></span> <span data-ttu-id="99540-199">可以在[创建](../api/user-post-contacts.md)或[更新](../api/contact-update.md)操作中指定显示名称。</span><span class="sxs-lookup"><span data-stu-id="99540-199">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="99540-200">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="99540-200">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="99540-201">若要保留预先存在的值，请始终在[更新](../api/contact-update.md)操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="99540-201">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="99540-202">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="99540-202">emailAddresses</span></span>|<span data-ttu-id="99540-203">[EmailAddress](emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99540-203">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="99540-204">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="99540-204">The contact's email addresses.</span></span>|
|<span data-ttu-id="99540-205">fileAs</span><span class="sxs-lookup"><span data-stu-id="99540-205">fileAs</span></span>|<span data-ttu-id="99540-206">String</span><span class="sxs-lookup"><span data-stu-id="99540-206">String</span></span>|<span data-ttu-id="99540-207">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="99540-207">The name the contact is filed under.</span></span>|
|<span data-ttu-id="99540-208">generation</span><span class="sxs-lookup"><span data-stu-id="99540-208">generation</span></span>|<span data-ttu-id="99540-209">String</span><span class="sxs-lookup"><span data-stu-id="99540-209">String</span></span>|<span data-ttu-id="99540-210">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="99540-210">The contact's generation.</span></span>|
|<span data-ttu-id="99540-211">givenName</span><span class="sxs-lookup"><span data-stu-id="99540-211">givenName</span></span>|<span data-ttu-id="99540-212">String</span><span class="sxs-lookup"><span data-stu-id="99540-212">String</span></span>|<span data-ttu-id="99540-213">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="99540-213">The contact's given name.</span></span>|
|<span data-ttu-id="99540-214">homeAddress</span><span class="sxs-lookup"><span data-stu-id="99540-214">homeAddress</span></span>|[<span data-ttu-id="99540-215">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="99540-215">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="99540-216">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="99540-216">The contact's home address.</span></span>|
|<span data-ttu-id="99540-217">homePhones</span><span class="sxs-lookup"><span data-stu-id="99540-217">homePhones</span></span>|<span data-ttu-id="99540-218">String collection</span><span class="sxs-lookup"><span data-stu-id="99540-218">String collection</span></span>|<span data-ttu-id="99540-219">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="99540-219">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="99540-220">id</span><span class="sxs-lookup"><span data-stu-id="99540-220">id</span></span>|<span data-ttu-id="99540-221">String</span><span class="sxs-lookup"><span data-stu-id="99540-221">String</span></span>|<span data-ttu-id="99540-p107">联系人的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="99540-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="99540-224">imAddresses</span><span class="sxs-lookup"><span data-stu-id="99540-224">imAddresses</span></span>|<span data-ttu-id="99540-225">String collection</span><span class="sxs-lookup"><span data-stu-id="99540-225">String collection</span></span>|<span data-ttu-id="99540-226">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="99540-226">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="99540-227">initials</span><span class="sxs-lookup"><span data-stu-id="99540-227">initials</span></span>|<span data-ttu-id="99540-228">String</span><span class="sxs-lookup"><span data-stu-id="99540-228">String</span></span>|<span data-ttu-id="99540-229">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="99540-229">The contact's initials.</span></span>|
|<span data-ttu-id="99540-230">jobTitle</span><span class="sxs-lookup"><span data-stu-id="99540-230">jobTitle</span></span>|<span data-ttu-id="99540-231">String</span><span class="sxs-lookup"><span data-stu-id="99540-231">String</span></span>|<span data-ttu-id="99540-232">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="99540-232">The contact’s job title.</span></span>|
|<span data-ttu-id="99540-233">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="99540-233">lastModifiedDateTime</span></span>|<span data-ttu-id="99540-234">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99540-234">DateTimeOffset</span></span>|<span data-ttu-id="99540-p108">修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="99540-p108">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="99540-238">manager</span><span class="sxs-lookup"><span data-stu-id="99540-238">manager</span></span>|<span data-ttu-id="99540-239">String</span><span class="sxs-lookup"><span data-stu-id="99540-239">String</span></span>|<span data-ttu-id="99540-240">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="99540-240">The name of the contact's manager.</span></span>
|<span data-ttu-id="99540-241">middleName</span><span class="sxs-lookup"><span data-stu-id="99540-241">middleName</span></span>|<span data-ttu-id="99540-242">String</span><span class="sxs-lookup"><span data-stu-id="99540-242">String</span></span>|<span data-ttu-id="99540-243">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="99540-243">The contact's middle name.</span></span>|
|<span data-ttu-id="99540-244">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="99540-244">mobilePhone</span></span>|<span data-ttu-id="99540-245">String</span><span class="sxs-lookup"><span data-stu-id="99540-245">String</span></span>|<span data-ttu-id="99540-246">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="99540-246">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="99540-247">nickName</span><span class="sxs-lookup"><span data-stu-id="99540-247">nickName</span></span>|<span data-ttu-id="99540-248">String</span><span class="sxs-lookup"><span data-stu-id="99540-248">String</span></span>|<span data-ttu-id="99540-249">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="99540-249">The contact's nickname.</span></span>|
|<span data-ttu-id="99540-250">officeLocation</span><span class="sxs-lookup"><span data-stu-id="99540-250">officeLocation</span></span>|<span data-ttu-id="99540-251">String</span><span class="sxs-lookup"><span data-stu-id="99540-251">String</span></span>|<span data-ttu-id="99540-252">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="99540-252">The location of the contact's office.</span></span>|
|<span data-ttu-id="99540-253">otherAddress</span><span class="sxs-lookup"><span data-stu-id="99540-253">otherAddress</span></span>|[<span data-ttu-id="99540-254">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="99540-254">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="99540-255">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="99540-255">Other addresses for the contact.</span></span>|
|<span data-ttu-id="99540-256">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="99540-256">parentFolderId</span></span>|<span data-ttu-id="99540-257">String</span><span class="sxs-lookup"><span data-stu-id="99540-257">String</span></span>|<span data-ttu-id="99540-258">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="99540-258">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="99540-259">personalNotes</span><span class="sxs-lookup"><span data-stu-id="99540-259">personalNotes</span></span>|<span data-ttu-id="99540-260">String</span><span class="sxs-lookup"><span data-stu-id="99540-260">String</span></span>|<span data-ttu-id="99540-261">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="99540-261">The user's notes about the contact.</span></span>|
|<span data-ttu-id="99540-262">profession</span><span class="sxs-lookup"><span data-stu-id="99540-262">profession</span></span>|<span data-ttu-id="99540-263">String</span><span class="sxs-lookup"><span data-stu-id="99540-263">String</span></span>|<span data-ttu-id="99540-264">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="99540-264">The contact's profession.</span></span>|
|<span data-ttu-id="99540-265">spouseName</span><span class="sxs-lookup"><span data-stu-id="99540-265">spouseName</span></span>|<span data-ttu-id="99540-266">String</span><span class="sxs-lookup"><span data-stu-id="99540-266">String</span></span>|<span data-ttu-id="99540-267">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="99540-267">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="99540-268">surname</span><span class="sxs-lookup"><span data-stu-id="99540-268">surname</span></span>|<span data-ttu-id="99540-269">String</span><span class="sxs-lookup"><span data-stu-id="99540-269">String</span></span>|<span data-ttu-id="99540-270">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="99540-270">The contact's surname.</span></span>|
|<span data-ttu-id="99540-271">title</span><span class="sxs-lookup"><span data-stu-id="99540-271">title</span></span>|<span data-ttu-id="99540-272">String</span><span class="sxs-lookup"><span data-stu-id="99540-272">String</span></span>|<span data-ttu-id="99540-273">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="99540-273">The contact's title.</span></span>|
|<span data-ttu-id="99540-274">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="99540-274">yomiCompanyName</span></span>|<span data-ttu-id="99540-275">String</span><span class="sxs-lookup"><span data-stu-id="99540-275">String</span></span>|<span data-ttu-id="99540-276">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="99540-276">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="99540-277">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="99540-277">yomiGivenName</span></span>|<span data-ttu-id="99540-278">String</span><span class="sxs-lookup"><span data-stu-id="99540-278">String</span></span>|<span data-ttu-id="99540-279">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="99540-279">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="99540-280">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="99540-280">yomiSurname</span></span>|<span data-ttu-id="99540-281">String</span><span class="sxs-lookup"><span data-stu-id="99540-281">String</span></span>|<span data-ttu-id="99540-282">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="99540-282">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="99540-283">关系</span><span class="sxs-lookup"><span data-stu-id="99540-283">Relationships</span></span>
| <span data-ttu-id="99540-284">关系</span><span class="sxs-lookup"><span data-stu-id="99540-284">Relationship</span></span> | <span data-ttu-id="99540-285">类型</span><span class="sxs-lookup"><span data-stu-id="99540-285">Type</span></span>   |<span data-ttu-id="99540-286">说明</span><span class="sxs-lookup"><span data-stu-id="99540-286">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="99540-287">extensions</span><span class="sxs-lookup"><span data-stu-id="99540-287">extensions</span></span>|<span data-ttu-id="99540-288">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="99540-288">[extension](extension.md) collection</span></span>|<span data-ttu-id="99540-p109">为联系人定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="99540-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="99540-292">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="99540-292">multiValueExtendedProperties</span></span>|<span data-ttu-id="99540-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="99540-293">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="99540-p110">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="99540-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="99540-297">照片</span><span class="sxs-lookup"><span data-stu-id="99540-297">photo</span></span>|[<span data-ttu-id="99540-298">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="99540-298">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="99540-p111">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="99540-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="99540-301">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="99540-301">singleValueExtendedProperties</span></span>|<span data-ttu-id="99540-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="99540-302">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="99540-p112">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="99540-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="99540-306">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="99540-306">JSON representation</span></span>

<span data-ttu-id="99540-307">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99540-307">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="99540-308">另请参阅</span><span class="sxs-lookup"><span data-stu-id="99540-308">See also</span></span>

- [<span data-ttu-id="99540-309">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="99540-309">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="99540-310">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="99540-310">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="99540-311">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="99540-311">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="99540-312">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="99540-312">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="99540-313">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="99540-313">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
