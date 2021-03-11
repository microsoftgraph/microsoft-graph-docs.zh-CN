---
title: 联系人资源类型
description: 联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。
author: kevinbellinger
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 5be9d6b9ad408d69a347990cfa458be07edef7b7
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721675"
---
# <a name="contact-resource-type"></a><span data-ttu-id="197c1-104">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="197c1-104">contact resource type</span></span>

<span data-ttu-id="197c1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="197c1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="197c1-p102">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="197c1-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="197c1-108">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="197c1-108">This resource supports:</span></span>

- <span data-ttu-id="197c1-109">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="197c1-109">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="197c1-110">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="197c1-110">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="197c1-111">通过提供 [delta](../api/contact-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="197c1-111">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="197c1-112">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="197c1-112">JSON representation</span></span>

<span data-ttu-id="197c1-113">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="197c1-113">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
  "keyProperty":"id",
  "@odata.type": "microsoft.graph.contact"
}-->

```json
{
  "assistantName": "string",
  "birthday": "String (timestamp)",
  "categories": ["string"],
  "changeKey": "string",
  "children": ["string"],
  "companyName": "string",
  "createdDateTime": "String (timestamp)",
  "department": "string",
  "displayName": "string",
  "emailAddresses": [{"@odata.type": "microsoft.graph.typedEmailAddress"}],
  "fileAs": "string",
  "flag": {"@odata.type": "microsoft.graph.followupFlag"},
  "gender": "string",
  "generation": "string",
  "givenName": "string",
  "id": "string (identifier)",
  "imAddresses": ["string"],
  "initials": "string",
  "jobTitle": "string",
  "lastModifiedDateTime": "String (timestamp)",
  "manager": "string",
  "middleName": "string",
  "nickName": "string",
  "officeLocation": "string",
  "parentFolderId": "string",
  "personalNotes": "string",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "postalAddresses": [{"@odata.type": "microsoft.graph.physicalAddress"}],
  "profession": "string",
  "spouseName": "string",
  "surname": "string",
  "title": "string",
  "websites": [{"@odata.type": "microsoft.graph.website"}],
  "weddingAnniversary": "date",
  "yomiCompanyName": "string",
  "yomiGivenName": "string",
  "yomiSurname": "string"
}

```
## <a name="properties"></a><span data-ttu-id="197c1-114">属性</span><span class="sxs-lookup"><span data-stu-id="197c1-114">Properties</span></span>
| <span data-ttu-id="197c1-115">属性</span><span class="sxs-lookup"><span data-stu-id="197c1-115">Property</span></span>     | <span data-ttu-id="197c1-116">类型</span><span class="sxs-lookup"><span data-stu-id="197c1-116">Type</span></span>   |<span data-ttu-id="197c1-117">说明</span><span class="sxs-lookup"><span data-stu-id="197c1-117">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="197c1-118">assistantName</span><span class="sxs-lookup"><span data-stu-id="197c1-118">assistantName</span></span>|<span data-ttu-id="197c1-119">String</span><span class="sxs-lookup"><span data-stu-id="197c1-119">String</span></span>|<span data-ttu-id="197c1-120">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="197c1-120">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="197c1-121">birthday</span><span class="sxs-lookup"><span data-stu-id="197c1-121">birthday</span></span>|<span data-ttu-id="197c1-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="197c1-122">DateTimeOffset</span></span>|<span data-ttu-id="197c1-123">联系人的生日。</span><span class="sxs-lookup"><span data-stu-id="197c1-123">The contact's birthday.</span></span> <span data-ttu-id="197c1-124">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="197c1-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="197c1-125">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="197c1-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="197c1-126">categories</span><span class="sxs-lookup"><span data-stu-id="197c1-126">categories</span></span>|<span data-ttu-id="197c1-127">String collection</span><span class="sxs-lookup"><span data-stu-id="197c1-127">String collection</span></span>|<span data-ttu-id="197c1-128">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="197c1-128">The categories associated with the contact.</span></span> <span data-ttu-id="197c1-129">每个类别对应于为用户定义的 [outlookCategory](outlookcategory.md) 的 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="197c1-129">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) defined for the user.</span></span>|
|<span data-ttu-id="197c1-130">changeKey</span><span class="sxs-lookup"><span data-stu-id="197c1-130">changeKey</span></span>|<span data-ttu-id="197c1-131">String</span><span class="sxs-lookup"><span data-stu-id="197c1-131">String</span></span>|<span data-ttu-id="197c1-p105">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="197c1-p105">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="197c1-135">children</span><span class="sxs-lookup"><span data-stu-id="197c1-135">children</span></span>|<span data-ttu-id="197c1-136">String collection</span><span class="sxs-lookup"><span data-stu-id="197c1-136">String collection</span></span>|<span data-ttu-id="197c1-137">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="197c1-137">The names of the contact's children.</span></span>|
|<span data-ttu-id="197c1-138">companyName</span><span class="sxs-lookup"><span data-stu-id="197c1-138">companyName</span></span>|<span data-ttu-id="197c1-139">String</span><span class="sxs-lookup"><span data-stu-id="197c1-139">String</span></span>|<span data-ttu-id="197c1-140">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="197c1-140">The name of the contact's company.</span></span>|
|<span data-ttu-id="197c1-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="197c1-141">createdDateTime</span></span>|<span data-ttu-id="197c1-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="197c1-142">DateTimeOffset</span></span>|<span data-ttu-id="197c1-143">创建联系人的时间。</span><span class="sxs-lookup"><span data-stu-id="197c1-143">The time the contact was created.</span></span> <span data-ttu-id="197c1-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="197c1-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="197c1-145">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="197c1-145">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="197c1-146">department</span><span class="sxs-lookup"><span data-stu-id="197c1-146">department</span></span>|<span data-ttu-id="197c1-147">String</span><span class="sxs-lookup"><span data-stu-id="197c1-147">String</span></span>|<span data-ttu-id="197c1-148">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="197c1-148">The contact's department.</span></span>|
|<span data-ttu-id="197c1-149">displayName</span><span class="sxs-lookup"><span data-stu-id="197c1-149">displayName</span></span>|<span data-ttu-id="197c1-150">String</span><span class="sxs-lookup"><span data-stu-id="197c1-150">String</span></span>|<span data-ttu-id="197c1-151">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="197c1-151">The contact's display name.</span></span> <span data-ttu-id="197c1-152">可以在[创建](../api/user-post-contacts.md)或[更新](../api/contact-update.md)操作中指定显示名称。</span><span class="sxs-lookup"><span data-stu-id="197c1-152">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="197c1-153">请注意，对其他属性的后续更新可能会导致自动生成的值覆盖你指定的 displayName 值。</span><span class="sxs-lookup"><span data-stu-id="197c1-153">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="197c1-154">若要保留预先存在的值，请始终在[更新](../api/contact-update.md)操作中将其作为 displayName。</span><span class="sxs-lookup"><span data-stu-id="197c1-154">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="197c1-155">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="197c1-155">emailAddresses</span></span>|<span data-ttu-id="197c1-156">[typedEmailAddress](typedemailaddress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="197c1-156">[typedEmailAddress](typedemailaddress.md) collection</span></span>|<span data-ttu-id="197c1-157">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="197c1-157">The contact's email addresses.</span></span>|
|<span data-ttu-id="197c1-158">fileAs</span><span class="sxs-lookup"><span data-stu-id="197c1-158">fileAs</span></span>|<span data-ttu-id="197c1-159">String</span><span class="sxs-lookup"><span data-stu-id="197c1-159">String</span></span>|<span data-ttu-id="197c1-160">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="197c1-160">The name the contact is filed under.</span></span>|
|<span data-ttu-id="197c1-161">flag</span><span class="sxs-lookup"><span data-stu-id="197c1-161">flag</span></span>|[<span data-ttu-id="197c1-162">followupFlag</span><span class="sxs-lookup"><span data-stu-id="197c1-162">followupFlag</span></span>](followupflag.md)|<span data-ttu-id="197c1-163">指示联系人的状态、开始日期、截止日期或完成日期的标志值。</span><span class="sxs-lookup"><span data-stu-id="197c1-163">The flag value that indicates the status, start date, due date, or completion date for the contact.</span></span> |
|<span data-ttu-id="197c1-164">gender</span><span class="sxs-lookup"><span data-stu-id="197c1-164">gender</span></span> |<span data-ttu-id="197c1-165">String</span><span class="sxs-lookup"><span data-stu-id="197c1-165">String</span></span> |<span data-ttu-id="197c1-166">联系人的性别。</span><span class="sxs-lookup"><span data-stu-id="197c1-166">The contact's gender.</span></span> |
|<span data-ttu-id="197c1-167">generation</span><span class="sxs-lookup"><span data-stu-id="197c1-167">generation</span></span>|<span data-ttu-id="197c1-168">String</span><span class="sxs-lookup"><span data-stu-id="197c1-168">String</span></span>|<span data-ttu-id="197c1-169">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="197c1-169">The contact's generation.</span></span>|
|<span data-ttu-id="197c1-170">givenName</span><span class="sxs-lookup"><span data-stu-id="197c1-170">givenName</span></span>|<span data-ttu-id="197c1-171">String</span><span class="sxs-lookup"><span data-stu-id="197c1-171">String</span></span>|<span data-ttu-id="197c1-172">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="197c1-172">The contact's given name.</span></span>|
|<span data-ttu-id="197c1-173">id</span><span class="sxs-lookup"><span data-stu-id="197c1-173">id</span></span>|<span data-ttu-id="197c1-174">String</span><span class="sxs-lookup"><span data-stu-id="197c1-174">String</span></span>| <span data-ttu-id="197c1-175">联系人的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="197c1-175">Unique identifier for the contact.</span></span> <span data-ttu-id="197c1-176">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] 只读。</span><span class="sxs-lookup"><span data-stu-id="197c1-176">[!INCLUDE [outlook-beta-id](../../includes/outlook-beta-id.md)] Read-only.</span></span> |
|<span data-ttu-id="197c1-177">imAddresses</span><span class="sxs-lookup"><span data-stu-id="197c1-177">imAddresses</span></span>|<span data-ttu-id="197c1-178">String collection</span><span class="sxs-lookup"><span data-stu-id="197c1-178">String collection</span></span>|<span data-ttu-id="197c1-179">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="197c1-179">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="197c1-180">initials</span><span class="sxs-lookup"><span data-stu-id="197c1-180">initials</span></span>|<span data-ttu-id="197c1-181">String</span><span class="sxs-lookup"><span data-stu-id="197c1-181">String</span></span>|<span data-ttu-id="197c1-182">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="197c1-182">The contact's initials.</span></span>|
|<span data-ttu-id="197c1-183">jobTitle</span><span class="sxs-lookup"><span data-stu-id="197c1-183">jobTitle</span></span>|<span data-ttu-id="197c1-184">String</span><span class="sxs-lookup"><span data-stu-id="197c1-184">String</span></span>|<span data-ttu-id="197c1-185">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="197c1-185">The contact’s job title.</span></span>|
|<span data-ttu-id="197c1-186">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="197c1-186">lastModifiedDateTime</span></span>|<span data-ttu-id="197c1-187">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="197c1-187">DateTimeOffset</span></span>|<span data-ttu-id="197c1-188">修改联系人的时间。</span><span class="sxs-lookup"><span data-stu-id="197c1-188">The time the contact was modified.</span></span> <span data-ttu-id="197c1-189">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="197c1-189">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="197c1-190">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="197c1-190">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="197c1-191">manager</span><span class="sxs-lookup"><span data-stu-id="197c1-191">manager</span></span>|<span data-ttu-id="197c1-192">String</span><span class="sxs-lookup"><span data-stu-id="197c1-192">String</span></span>|<span data-ttu-id="197c1-193">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="197c1-193">The name of the contact's manager.</span></span>
|<span data-ttu-id="197c1-194">middleName</span><span class="sxs-lookup"><span data-stu-id="197c1-194">middleName</span></span>|<span data-ttu-id="197c1-195">String</span><span class="sxs-lookup"><span data-stu-id="197c1-195">String</span></span>|<span data-ttu-id="197c1-196">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="197c1-196">The contact's middle name.</span></span>|
|<span data-ttu-id="197c1-197">nickName</span><span class="sxs-lookup"><span data-stu-id="197c1-197">nickName</span></span>|<span data-ttu-id="197c1-198">String</span><span class="sxs-lookup"><span data-stu-id="197c1-198">String</span></span>|<span data-ttu-id="197c1-199">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="197c1-199">The contact's nickname.</span></span>|
|<span data-ttu-id="197c1-200">officeLocation</span><span class="sxs-lookup"><span data-stu-id="197c1-200">officeLocation</span></span>|<span data-ttu-id="197c1-201">String</span><span class="sxs-lookup"><span data-stu-id="197c1-201">String</span></span>|<span data-ttu-id="197c1-202">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="197c1-202">The location of the contact's office.</span></span>|
|<span data-ttu-id="197c1-203">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="197c1-203">parentFolderId</span></span>|<span data-ttu-id="197c1-204">String</span><span class="sxs-lookup"><span data-stu-id="197c1-204">String</span></span>|<span data-ttu-id="197c1-205">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="197c1-205">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="197c1-206">personalNotes</span><span class="sxs-lookup"><span data-stu-id="197c1-206">personalNotes</span></span>|<span data-ttu-id="197c1-207">String</span><span class="sxs-lookup"><span data-stu-id="197c1-207">String</span></span>|<span data-ttu-id="197c1-208">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="197c1-208">The user's notes about the contact.</span></span>|
|<span data-ttu-id="197c1-209">phones</span><span class="sxs-lookup"><span data-stu-id="197c1-209">phones</span></span> |<span data-ttu-id="197c1-210">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="197c1-210">[phone](phone.md) collection</span></span> |<span data-ttu-id="197c1-211">与联系人关联的电话号码，例如住宅电话、移动电话和业务电话。</span><span class="sxs-lookup"><span data-stu-id="197c1-211">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="197c1-212">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="197c1-212">postalAddresses</span></span> |<span data-ttu-id="197c1-213">[physicalAddress](physicaladdress.md) 集合</span><span class="sxs-lookup"><span data-stu-id="197c1-213">[physicalAddress](physicaladdress.md) collection</span></span> |<span data-ttu-id="197c1-214">与联系人关联的地址，例如，住宅地址和业务地址。</span><span class="sxs-lookup"><span data-stu-id="197c1-214">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="197c1-215">profession</span><span class="sxs-lookup"><span data-stu-id="197c1-215">profession</span></span>|<span data-ttu-id="197c1-216">String</span><span class="sxs-lookup"><span data-stu-id="197c1-216">String</span></span>|<span data-ttu-id="197c1-217">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="197c1-217">The contact's profession.</span></span>|
|<span data-ttu-id="197c1-218">spouseName</span><span class="sxs-lookup"><span data-stu-id="197c1-218">spouseName</span></span>|<span data-ttu-id="197c1-219">String</span><span class="sxs-lookup"><span data-stu-id="197c1-219">String</span></span>|<span data-ttu-id="197c1-220">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="197c1-220">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="197c1-221">surname</span><span class="sxs-lookup"><span data-stu-id="197c1-221">surname</span></span>|<span data-ttu-id="197c1-222">String</span><span class="sxs-lookup"><span data-stu-id="197c1-222">String</span></span>|<span data-ttu-id="197c1-223">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="197c1-223">The contact's surname.</span></span>|
|<span data-ttu-id="197c1-224">title</span><span class="sxs-lookup"><span data-stu-id="197c1-224">title</span></span>|<span data-ttu-id="197c1-225">String</span><span class="sxs-lookup"><span data-stu-id="197c1-225">String</span></span>|<span data-ttu-id="197c1-226">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="197c1-226">The contact's title.</span></span>|
|<span data-ttu-id="197c1-227">websites</span><span class="sxs-lookup"><span data-stu-id="197c1-227">websites</span></span> |<span data-ttu-id="197c1-228">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="197c1-228">[website](website.md) collection</span></span>|<span data-ttu-id="197c1-229">与联系人关联的网站。</span><span class="sxs-lookup"><span data-stu-id="197c1-229">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="197c1-230">aryAnniversary</span><span class="sxs-lookup"><span data-stu-id="197c1-230">weddingAnniversary</span></span> |<span data-ttu-id="197c1-231">日期</span><span class="sxs-lookup"><span data-stu-id="197c1-231">Date</span></span> |<span data-ttu-id="197c1-232">联系人的周年日。</span><span class="sxs-lookup"><span data-stu-id="197c1-232">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="197c1-233">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="197c1-233">yomiCompanyName</span></span>|<span data-ttu-id="197c1-234">String</span><span class="sxs-lookup"><span data-stu-id="197c1-234">String</span></span>|<span data-ttu-id="197c1-235">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="197c1-235">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="197c1-236">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="197c1-236">yomiGivenName</span></span>|<span data-ttu-id="197c1-237">String</span><span class="sxs-lookup"><span data-stu-id="197c1-237">String</span></span>|<span data-ttu-id="197c1-238">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="197c1-238">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="197c1-239">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="197c1-239">yomiSurname</span></span>|<span data-ttu-id="197c1-240">String</span><span class="sxs-lookup"><span data-stu-id="197c1-240">String</span></span>|<span data-ttu-id="197c1-241">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="197c1-241">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="197c1-242">关系</span><span class="sxs-lookup"><span data-stu-id="197c1-242">Relationships</span></span>
| <span data-ttu-id="197c1-243">关系</span><span class="sxs-lookup"><span data-stu-id="197c1-243">Relationship</span></span> | <span data-ttu-id="197c1-244">类型</span><span class="sxs-lookup"><span data-stu-id="197c1-244">Type</span></span>   |<span data-ttu-id="197c1-245">说明</span><span class="sxs-lookup"><span data-stu-id="197c1-245">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="197c1-246">extensions</span><span class="sxs-lookup"><span data-stu-id="197c1-246">extensions</span></span>|<span data-ttu-id="197c1-247">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="197c1-247">[extension](extension.md) collection</span></span>|<span data-ttu-id="197c1-248">为联系人定义的开放扩展集合。</span><span class="sxs-lookup"><span data-stu-id="197c1-248">The collection of open extensions defined for the contact.</span></span> <span data-ttu-id="197c1-249">可为空。</span><span class="sxs-lookup"><span data-stu-id="197c1-249">Nullable.</span></span>|
|<span data-ttu-id="197c1-250">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="197c1-250">multiValueExtendedProperties</span></span>|<span data-ttu-id="197c1-251">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="197c1-251">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="197c1-p111">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="197c1-p111">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="197c1-255">photo</span><span class="sxs-lookup"><span data-stu-id="197c1-255">photo</span></span>|[<span data-ttu-id="197c1-256">照片</span><span class="sxs-lookup"><span data-stu-id="197c1-256">photo</span></span>](profilephoto.md)| <span data-ttu-id="197c1-p112">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="197c1-p112">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="197c1-259">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="197c1-259">singleValueExtendedProperties</span></span>|<span data-ttu-id="197c1-260">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="197c1-260">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="197c1-p113">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="197c1-p113">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="197c1-264">方法</span><span class="sxs-lookup"><span data-stu-id="197c1-264">Methods</span></span>
| <span data-ttu-id="197c1-265">方法</span><span class="sxs-lookup"><span data-stu-id="197c1-265">Method</span></span>           | <span data-ttu-id="197c1-266">返回类型</span><span class="sxs-lookup"><span data-stu-id="197c1-266">Return Type</span></span>    |<span data-ttu-id="197c1-267">说明</span><span class="sxs-lookup"><span data-stu-id="197c1-267">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="197c1-268">获取联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-268">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="197c1-269">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-269">contact</span></span>](contact.md) |<span data-ttu-id="197c1-270">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="197c1-270">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="197c1-271">创建</span><span class="sxs-lookup"><span data-stu-id="197c1-271">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="197c1-272">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-272">contact</span></span>](contact.md) |<span data-ttu-id="197c1-273">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="197c1-273">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="197c1-274">更新</span><span class="sxs-lookup"><span data-stu-id="197c1-274">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="197c1-275">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-275">contact</span></span>](contact.md) |<span data-ttu-id="197c1-276">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="197c1-276">Update contact object.</span></span> |
|[<span data-ttu-id="197c1-277">删除</span><span class="sxs-lookup"><span data-stu-id="197c1-277">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="197c1-278">无</span><span class="sxs-lookup"><span data-stu-id="197c1-278">None</span></span> |<span data-ttu-id="197c1-279">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="197c1-279">Delete contact object.</span></span> |
|[<span data-ttu-id="197c1-280">delta</span><span class="sxs-lookup"><span data-stu-id="197c1-280">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="197c1-281">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="197c1-281">[contact](contact.md) collection</span></span>| <span data-ttu-id="197c1-282">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="197c1-282">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="197c1-283">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="197c1-283">**Open extensions**</span></span>| | |
|[<span data-ttu-id="197c1-284">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="197c1-284">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="197c1-285">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="197c1-285">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="197c1-286">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="197c1-286">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="197c1-287">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="197c1-287">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="197c1-288">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="197c1-288">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="197c1-289">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="197c1-289">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="197c1-290">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="197c1-290">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="197c1-291">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="197c1-291">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="197c1-292">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="197c1-292">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="197c1-293">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="197c1-293">**Extended properties**</span></span>| | |
|[<span data-ttu-id="197c1-294">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="197c1-294">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="197c1-295">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-295">contact</span></span>](contact.md)  |<span data-ttu-id="197c1-296">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="197c1-296">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="197c1-297">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-297">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="197c1-298">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-298">contact</span></span>](contact.md) | <span data-ttu-id="197c1-299">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="197c1-299">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="197c1-300">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="197c1-300">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="197c1-301">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-301">contact</span></span>](contact.md) | <span data-ttu-id="197c1-302">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="197c1-302">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="197c1-303">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-303">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="197c1-304">联系人</span><span class="sxs-lookup"><span data-stu-id="197c1-304">contact</span></span>](contact.md) | <span data-ttu-id="197c1-305">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="197c1-305">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="197c1-306">另请参阅</span><span class="sxs-lookup"><span data-stu-id="197c1-306">See also</span></span>

- [<span data-ttu-id="197c1-307">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="197c1-307">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="197c1-308">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="197c1-308">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="197c1-309">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="197c1-309">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="197c1-310">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="197c1-310">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="197c1-311">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="197c1-311">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


