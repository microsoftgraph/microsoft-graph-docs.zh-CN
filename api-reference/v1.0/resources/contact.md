---
title: 联系人资源类型
description: 联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。
author: kevinbellinger
localization_priority: Priority
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 91ce5d0c21d0b9dc700e2669efe881488d79257d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721997"
---
# <a name="contact-resource-type"></a><span data-ttu-id="fe6b1-104">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="fe6b1-104">contact resource type</span></span>

<span data-ttu-id="fe6b1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fe6b1-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fe6b1-p102">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="fe6b1-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="fe6b1-108">This resource supports:</span></span>

- <span data-ttu-id="fe6b1-109">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="fe6b1-110">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="fe6b1-111">通过提供 [delta](../api/contact-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>


## <a name="methods"></a><span data-ttu-id="fe6b1-112">方法</span><span class="sxs-lookup"><span data-stu-id="fe6b1-112">Methods</span></span>

| <span data-ttu-id="fe6b1-113">方法</span><span class="sxs-lookup"><span data-stu-id="fe6b1-113">Method</span></span>       | <span data-ttu-id="fe6b1-114">返回类型</span><span class="sxs-lookup"><span data-stu-id="fe6b1-114">Return Type</span></span>  |<span data-ttu-id="fe6b1-115">说明</span><span class="sxs-lookup"><span data-stu-id="fe6b1-115">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe6b1-116">获取联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-116">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="fe6b1-117">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-117">contact</span></span>](contact.md) |<span data-ttu-id="fe6b1-118">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-118">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="fe6b1-119">创建</span><span class="sxs-lookup"><span data-stu-id="fe6b1-119">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="fe6b1-120">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-120">contact</span></span>](contact.md) |<span data-ttu-id="fe6b1-121">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-121">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="fe6b1-122">更新</span><span class="sxs-lookup"><span data-stu-id="fe6b1-122">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="fe6b1-123">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-123">contact</span></span>](contact.md) |<span data-ttu-id="fe6b1-124">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-124">Update contact object.</span></span> |
|[<span data-ttu-id="fe6b1-125">删除</span><span class="sxs-lookup"><span data-stu-id="fe6b1-125">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="fe6b1-126">无</span><span class="sxs-lookup"><span data-stu-id="fe6b1-126">None</span></span> |<span data-ttu-id="fe6b1-127">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-127">Delete contact object.</span></span> |
|[<span data-ttu-id="fe6b1-128">delta</span><span class="sxs-lookup"><span data-stu-id="fe6b1-128">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="fe6b1-129">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe6b1-129">[contact](contact.md) collection</span></span>| <span data-ttu-id="fe6b1-130">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-130">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="fe6b1-131">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="fe6b1-131">**Open extensions**</span></span>| | |
|[<span data-ttu-id="fe6b1-132">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="fe6b1-132">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="fe6b1-133">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="fe6b1-133">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="fe6b1-134">创建开放扩展，并在新建或现有的资源实例中添加自定义属性。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-134">Create an open extension and add custom properties in a new or existing instance of a resource.</span></span>|
|[<span data-ttu-id="fe6b1-135">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="fe6b1-135">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="fe6b1-136">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe6b1-136">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="fe6b1-137">获取通过名称或完全限定的名称识别的一个或多个开放扩展对象。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-137">Get an open extension object or objects identified by name or fully qualified name.</span></span>|
|<span data-ttu-id="fe6b1-138">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="fe6b1-138">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="fe6b1-139">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="fe6b1-139">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="fe6b1-140">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-140">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="fe6b1-141">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="fe6b1-141">**Extended properties**</span></span>| | |
|[<span data-ttu-id="fe6b1-142">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="fe6b1-142">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="fe6b1-143">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-143">contact</span></span>](contact.md)  |<span data-ttu-id="fe6b1-144">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-144">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="fe6b1-145">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-145">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="fe6b1-146">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-146">contact</span></span>](contact.md) | <span data-ttu-id="fe6b1-147">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-147">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="fe6b1-148">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="fe6b1-148">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="fe6b1-149">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-149">contact</span></span>](contact.md) | <span data-ttu-id="fe6b1-150">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-150">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="fe6b1-151">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-151">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="fe6b1-152">联系人</span><span class="sxs-lookup"><span data-stu-id="fe6b1-152">contact</span></span>](contact.md) | <span data-ttu-id="fe6b1-153">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-153">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="properties"></a><span data-ttu-id="fe6b1-154">属性</span><span class="sxs-lookup"><span data-stu-id="fe6b1-154">Properties</span></span>
| <span data-ttu-id="fe6b1-155">属性</span><span class="sxs-lookup"><span data-stu-id="fe6b1-155">Property</span></span>     | <span data-ttu-id="fe6b1-156">类型</span><span class="sxs-lookup"><span data-stu-id="fe6b1-156">Type</span></span>   |<span data-ttu-id="fe6b1-157">说明</span><span class="sxs-lookup"><span data-stu-id="fe6b1-157">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe6b1-158">assistantName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-158">assistantName</span></span>|<span data-ttu-id="fe6b1-159">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-159">String</span></span>|<span data-ttu-id="fe6b1-160">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-160">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="fe6b1-161">birthday</span><span class="sxs-lookup"><span data-stu-id="fe6b1-161">birthday</span></span>|<span data-ttu-id="fe6b1-162">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe6b1-162">DateTimeOffset</span></span>|<span data-ttu-id="fe6b1-163">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-163">The contact's birthday.</span></span> <span data-ttu-id="fe6b1-164">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-164">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe6b1-165">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe6b1-165">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fe6b1-166">businessAddress</span><span class="sxs-lookup"><span data-stu-id="fe6b1-166">businessAddress</span></span>|[<span data-ttu-id="fe6b1-167">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="fe6b1-167">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="fe6b1-168">联系人的公司地址。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-168">The contact's business address.</span></span>|
|<span data-ttu-id="fe6b1-169">businessHomePage</span><span class="sxs-lookup"><span data-stu-id="fe6b1-169">businessHomePage</span></span>|<span data-ttu-id="fe6b1-170">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-170">String</span></span>|<span data-ttu-id="fe6b1-171">联系人的公司主页。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-171">The business home page of the contact.</span></span>|
|<span data-ttu-id="fe6b1-172">businessPhones</span><span class="sxs-lookup"><span data-stu-id="fe6b1-172">businessPhones</span></span>|<span data-ttu-id="fe6b1-173">String collection</span><span class="sxs-lookup"><span data-stu-id="fe6b1-173">String collection</span></span>|<span data-ttu-id="fe6b1-174">联系人的公司电话号码。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-174">The contact's business phone numbers.</span></span>|
|<span data-ttu-id="fe6b1-175">categories</span><span class="sxs-lookup"><span data-stu-id="fe6b1-175">categories</span></span>|<span data-ttu-id="fe6b1-176">String collection</span><span class="sxs-lookup"><span data-stu-id="fe6b1-176">String collection</span></span>|<span data-ttu-id="fe6b1-177">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-177">The categories associated with the contact.</span></span>|
|<span data-ttu-id="fe6b1-178">changeKey</span><span class="sxs-lookup"><span data-stu-id="fe6b1-178">changeKey</span></span>|<span data-ttu-id="fe6b1-179">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-179">String</span></span>|<span data-ttu-id="fe6b1-p104">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p104">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="fe6b1-183">children</span><span class="sxs-lookup"><span data-stu-id="fe6b1-183">children</span></span>|<span data-ttu-id="fe6b1-184">String collection</span><span class="sxs-lookup"><span data-stu-id="fe6b1-184">String collection</span></span>|<span data-ttu-id="fe6b1-185">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-185">The names of the contact's children.</span></span>|
|<span data-ttu-id="fe6b1-186">companyName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-186">companyName</span></span>|<span data-ttu-id="fe6b1-187">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-187">String</span></span>|<span data-ttu-id="fe6b1-188">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-188">The name of the contact's company.</span></span>|
|<span data-ttu-id="fe6b1-189">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fe6b1-189">createdDateTime</span></span>|<span data-ttu-id="fe6b1-190">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe6b1-190">DateTimeOffset</span></span>|<span data-ttu-id="fe6b1-191">创建联系人的时间。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-191">The time the contact was created.</span></span> <span data-ttu-id="fe6b1-192">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-192">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe6b1-193">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe6b1-193">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fe6b1-194">department</span><span class="sxs-lookup"><span data-stu-id="fe6b1-194">department</span></span>|<span data-ttu-id="fe6b1-195">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-195">String</span></span>|<span data-ttu-id="fe6b1-196">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-196">The contact's department.</span></span>|
|<span data-ttu-id="fe6b1-197">displayName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-197">displayName</span></span>|<span data-ttu-id="fe6b1-198">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-198">String</span></span>|<span data-ttu-id="fe6b1-199">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-199">The contact's display name.</span></span> <span data-ttu-id="fe6b1-200">可以在[创建](../api/user-post-contacts.md)或[更新](../api/contact-update.md)操作中指定显示名称。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-200">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="fe6b1-201">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-201">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="fe6b1-202">若要保留预先存在的值，请始终在[更新](../api/contact-update.md)操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-202">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="fe6b1-203">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="fe6b1-203">emailAddresses</span></span>|<span data-ttu-id="fe6b1-204">[EmailAddress](emailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe6b1-204">[EmailAddress](emailaddress.md) collection</span></span>|<span data-ttu-id="fe6b1-205">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-205">The contact's email addresses.</span></span>|
|<span data-ttu-id="fe6b1-206">fileAs</span><span class="sxs-lookup"><span data-stu-id="fe6b1-206">fileAs</span></span>|<span data-ttu-id="fe6b1-207">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-207">String</span></span>|<span data-ttu-id="fe6b1-208">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-208">The name the contact is filed under.</span></span>|
|<span data-ttu-id="fe6b1-209">generation</span><span class="sxs-lookup"><span data-stu-id="fe6b1-209">generation</span></span>|<span data-ttu-id="fe6b1-210">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-210">String</span></span>|<span data-ttu-id="fe6b1-211">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-211">The contact's generation.</span></span>|
|<span data-ttu-id="fe6b1-212">givenName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-212">givenName</span></span>|<span data-ttu-id="fe6b1-213">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-213">String</span></span>|<span data-ttu-id="fe6b1-214">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-214">The contact's given name.</span></span>|
|<span data-ttu-id="fe6b1-215">homeAddress</span><span class="sxs-lookup"><span data-stu-id="fe6b1-215">homeAddress</span></span>|[<span data-ttu-id="fe6b1-216">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="fe6b1-216">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="fe6b1-217">联系人的住宅地址。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-217">The contact's home address.</span></span>|
|<span data-ttu-id="fe6b1-218">homePhones</span><span class="sxs-lookup"><span data-stu-id="fe6b1-218">homePhones</span></span>|<span data-ttu-id="fe6b1-219">String collection</span><span class="sxs-lookup"><span data-stu-id="fe6b1-219">String collection</span></span>|<span data-ttu-id="fe6b1-220">联系人的住宅电话号码。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-220">The contact's home phone numbers.</span></span>|
|<span data-ttu-id="fe6b1-221">id</span><span class="sxs-lookup"><span data-stu-id="fe6b1-221">id</span></span>|<span data-ttu-id="fe6b1-222">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-222">String</span></span>|<span data-ttu-id="fe6b1-p107">联系人的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p107">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="fe6b1-225">imAddresses</span><span class="sxs-lookup"><span data-stu-id="fe6b1-225">imAddresses</span></span>|<span data-ttu-id="fe6b1-226">String collection</span><span class="sxs-lookup"><span data-stu-id="fe6b1-226">String collection</span></span>|<span data-ttu-id="fe6b1-227">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-227">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="fe6b1-228">initials</span><span class="sxs-lookup"><span data-stu-id="fe6b1-228">initials</span></span>|<span data-ttu-id="fe6b1-229">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-229">String</span></span>|<span data-ttu-id="fe6b1-230">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-230">The contact's initials.</span></span>|
|<span data-ttu-id="fe6b1-231">jobTitle</span><span class="sxs-lookup"><span data-stu-id="fe6b1-231">jobTitle</span></span>|<span data-ttu-id="fe6b1-232">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-232">String</span></span>|<span data-ttu-id="fe6b1-233">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-233">The contact’s job title.</span></span>|
|<span data-ttu-id="fe6b1-234">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fe6b1-234">lastModifiedDateTime</span></span>|<span data-ttu-id="fe6b1-235">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fe6b1-235">DateTimeOffset</span></span>|<span data-ttu-id="fe6b1-236">修改联系人的时间。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-236">The time the contact was modified.</span></span> <span data-ttu-id="fe6b1-237">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-237">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="fe6b1-238">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="fe6b1-238">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="fe6b1-239">manager</span><span class="sxs-lookup"><span data-stu-id="fe6b1-239">manager</span></span>|<span data-ttu-id="fe6b1-240">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-240">String</span></span>|<span data-ttu-id="fe6b1-241">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-241">The name of the contact's manager.</span></span>
|<span data-ttu-id="fe6b1-242">middleName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-242">middleName</span></span>|<span data-ttu-id="fe6b1-243">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-243">String</span></span>|<span data-ttu-id="fe6b1-244">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-244">The contact's middle name.</span></span>|
|<span data-ttu-id="fe6b1-245">mobilePhone</span><span class="sxs-lookup"><span data-stu-id="fe6b1-245">mobilePhone</span></span>|<span data-ttu-id="fe6b1-246">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-246">String</span></span>|<span data-ttu-id="fe6b1-247">联系人的移动电话号码。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-247">The contact's mobile phone number.</span></span>|
|<span data-ttu-id="fe6b1-248">nickName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-248">nickName</span></span>|<span data-ttu-id="fe6b1-249">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-249">String</span></span>|<span data-ttu-id="fe6b1-250">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-250">The contact's nickname.</span></span>|
|<span data-ttu-id="fe6b1-251">officeLocation</span><span class="sxs-lookup"><span data-stu-id="fe6b1-251">officeLocation</span></span>|<span data-ttu-id="fe6b1-252">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-252">String</span></span>|<span data-ttu-id="fe6b1-253">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-253">The location of the contact's office.</span></span>|
|<span data-ttu-id="fe6b1-254">otherAddress</span><span class="sxs-lookup"><span data-stu-id="fe6b1-254">otherAddress</span></span>|[<span data-ttu-id="fe6b1-255">PhysicalAddress</span><span class="sxs-lookup"><span data-stu-id="fe6b1-255">PhysicalAddress</span></span>](physicaladdress.md)|<span data-ttu-id="fe6b1-256">联系人的其他地址。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-256">Other addresses for the contact.</span></span>|
|<span data-ttu-id="fe6b1-257">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="fe6b1-257">parentFolderId</span></span>|<span data-ttu-id="fe6b1-258">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-258">String</span></span>|<span data-ttu-id="fe6b1-259">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-259">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="fe6b1-260">personalNotes</span><span class="sxs-lookup"><span data-stu-id="fe6b1-260">personalNotes</span></span>|<span data-ttu-id="fe6b1-261">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-261">String</span></span>|<span data-ttu-id="fe6b1-262">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-262">The user's notes about the contact.</span></span>|
|<span data-ttu-id="fe6b1-263">profession</span><span class="sxs-lookup"><span data-stu-id="fe6b1-263">profession</span></span>|<span data-ttu-id="fe6b1-264">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-264">String</span></span>|<span data-ttu-id="fe6b1-265">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-265">The contact's profession.</span></span>|
|<span data-ttu-id="fe6b1-266">spouseName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-266">spouseName</span></span>|<span data-ttu-id="fe6b1-267">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-267">String</span></span>|<span data-ttu-id="fe6b1-268">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-268">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="fe6b1-269">surname</span><span class="sxs-lookup"><span data-stu-id="fe6b1-269">surname</span></span>|<span data-ttu-id="fe6b1-270">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-270">String</span></span>|<span data-ttu-id="fe6b1-271">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-271">The contact's surname.</span></span>|
|<span data-ttu-id="fe6b1-272">title</span><span class="sxs-lookup"><span data-stu-id="fe6b1-272">title</span></span>|<span data-ttu-id="fe6b1-273">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-273">String</span></span>|<span data-ttu-id="fe6b1-274">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-274">The contact's title.</span></span>|
|<span data-ttu-id="fe6b1-275">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-275">yomiCompanyName</span></span>|<span data-ttu-id="fe6b1-276">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-276">String</span></span>|<span data-ttu-id="fe6b1-277">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-277">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="fe6b1-278">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="fe6b1-278">yomiGivenName</span></span>|<span data-ttu-id="fe6b1-279">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-279">String</span></span>|<span data-ttu-id="fe6b1-280">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-280">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="fe6b1-281">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="fe6b1-281">yomiSurname</span></span>|<span data-ttu-id="fe6b1-282">String</span><span class="sxs-lookup"><span data-stu-id="fe6b1-282">String</span></span>|<span data-ttu-id="fe6b1-283">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-283">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe6b1-284">关系</span><span class="sxs-lookup"><span data-stu-id="fe6b1-284">Relationships</span></span>
| <span data-ttu-id="fe6b1-285">关系</span><span class="sxs-lookup"><span data-stu-id="fe6b1-285">Relationship</span></span> | <span data-ttu-id="fe6b1-286">类型</span><span class="sxs-lookup"><span data-stu-id="fe6b1-286">Type</span></span>   |<span data-ttu-id="fe6b1-287">说明</span><span class="sxs-lookup"><span data-stu-id="fe6b1-287">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe6b1-288">extensions</span><span class="sxs-lookup"><span data-stu-id="fe6b1-288">extensions</span></span>|<span data-ttu-id="fe6b1-289">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="fe6b1-289">[extension](extension.md) collection</span></span>|<span data-ttu-id="fe6b1-p109">为联系人定义的开放扩展集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p109">The collection of open extensions defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="fe6b1-293">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="fe6b1-293">multiValueExtendedProperties</span></span>|<span data-ttu-id="fe6b1-294">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="fe6b1-294">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="fe6b1-p110">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p110">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="fe6b1-298">照片</span><span class="sxs-lookup"><span data-stu-id="fe6b1-298">photo</span></span>|[<span data-ttu-id="fe6b1-299">profilePhoto</span><span class="sxs-lookup"><span data-stu-id="fe6b1-299">profilePhoto</span></span>](profilephoto.md)| <span data-ttu-id="fe6b1-p111">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p111">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="fe6b1-302">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="fe6b1-302">singleValueExtendedProperties</span></span>|<span data-ttu-id="fe6b1-303">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="fe6b1-303">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="fe6b1-p112">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-p112">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe6b1-307">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="fe6b1-307">JSON representation</span></span>

<span data-ttu-id="fe6b1-308">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fe6b1-308">Here is a JSON representation of the resource</span></span>

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

## <a name="see-also"></a><span data-ttu-id="fe6b1-309">另请参阅</span><span class="sxs-lookup"><span data-stu-id="fe6b1-309">See also</span></span>

- [<span data-ttu-id="fe6b1-310">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="fe6b1-310">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="fe6b1-311">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="fe6b1-311">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="fe6b1-312">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fe6b1-312">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="fe6b1-313">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fe6b1-313">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="fe6b1-314">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="fe6b1-314">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

