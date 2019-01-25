---
title: 联系人资源类型
description: 联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: d2bdc1be9e504bc72ce12ffe924b6da0812b99ce
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29513576"
---
# <a name="contact-resource-type"></a><span data-ttu-id="319fe-104">联系人资源类型</span><span class="sxs-lookup"><span data-stu-id="319fe-104">contact resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="319fe-p102">联系人是 Outlook 中的一个项目，你可以在这里组织和保存有关你通信的人员和组织的信息。联系人包含在联系人文件夹中。</span><span class="sxs-lookup"><span data-stu-id="319fe-p102">A contact is an item in Outlook where you can organize and save information about the people and organizations you communicate with. Contacts are contained in contact folders.</span></span>

<span data-ttu-id="319fe-107">该资源支持：</span><span class="sxs-lookup"><span data-stu-id="319fe-107">This resource supports:</span></span>

- <span data-ttu-id="319fe-108">将你自己的数据作为[扩展](/graph/extensibility-overview)添加到自定义属性。</span><span class="sxs-lookup"><span data-stu-id="319fe-108">Adding your own data to custom properties as [extensions](/graph/extensibility-overview).</span></span>
- <span data-ttu-id="319fe-109">订阅[更改通知](/graph/webhooks)。</span><span class="sxs-lookup"><span data-stu-id="319fe-109">Subscribing to [change notifications](/graph/webhooks).</span></span>
- <span data-ttu-id="319fe-110">通过提供 [delta](../api/contact-delta.md) 函数，使用 [delta 查询](/graph/delta-query-overview)跟踪增量添加、删除和更新。</span><span class="sxs-lookup"><span data-stu-id="319fe-110">Using [delta query](/graph/delta-query-overview) to track incremental additions, deletions, and updates, by providing a [delta](../api/contact-delta.md) function.</span></span>

## <a name="json-representation"></a><span data-ttu-id="319fe-111">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="319fe-111">JSON representation</span></span>

<span data-ttu-id="319fe-112">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="319fe-112">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
    "extensions",
    "multiValueExtendedProperties",
    "photo",
    "singleValueExtendedProperties"
  ],
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
## <a name="properties"></a><span data-ttu-id="319fe-113">属性</span><span class="sxs-lookup"><span data-stu-id="319fe-113">Properties</span></span>
| <span data-ttu-id="319fe-114">属性</span><span class="sxs-lookup"><span data-stu-id="319fe-114">Property</span></span>     | <span data-ttu-id="319fe-115">类型</span><span class="sxs-lookup"><span data-stu-id="319fe-115">Type</span></span>   |<span data-ttu-id="319fe-116">说明</span><span class="sxs-lookup"><span data-stu-id="319fe-116">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="319fe-117">assistantName</span><span class="sxs-lookup"><span data-stu-id="319fe-117">assistantName</span></span>|<span data-ttu-id="319fe-118">String</span><span class="sxs-lookup"><span data-stu-id="319fe-118">String</span></span>|<span data-ttu-id="319fe-119">联系人助理的姓名。</span><span class="sxs-lookup"><span data-stu-id="319fe-119">The name of the contact's assistant.</span></span>|
|<span data-ttu-id="319fe-120">birthday</span><span class="sxs-lookup"><span data-stu-id="319fe-120">birthday</span></span>|<span data-ttu-id="319fe-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319fe-121">DateTimeOffset</span></span>|<span data-ttu-id="319fe-p103">联系人的生日。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="319fe-p103">The contact's birthday. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="319fe-125">categories</span><span class="sxs-lookup"><span data-stu-id="319fe-125">categories</span></span>|<span data-ttu-id="319fe-126">字符串集合</span><span class="sxs-lookup"><span data-stu-id="319fe-126">String collection</span></span>|<span data-ttu-id="319fe-127">与联系人关联的类别。</span><span class="sxs-lookup"><span data-stu-id="319fe-127">The categories associated with the contact.</span></span> <span data-ttu-id="319fe-128">每个类别对应于[outlookCategory](outlookcategory.md)为用户定义的**displayName**属性。</span><span class="sxs-lookup"><span data-stu-id="319fe-128">Each category corresponds to the **displayName** property of an [outlookCategory](outlookcategory.md) defined for the user.</span></span>|
|<span data-ttu-id="319fe-129">changeKey</span><span class="sxs-lookup"><span data-stu-id="319fe-129">changeKey</span></span>|<span data-ttu-id="319fe-130">String</span><span class="sxs-lookup"><span data-stu-id="319fe-130">String</span></span>|<span data-ttu-id="319fe-p105">标识联系人的版本。每次联系人更改时，ChangeKey 也将更改。这样，Exchange 可以将更改应用于该对象的正确版本。</span><span class="sxs-lookup"><span data-stu-id="319fe-p105">Identifies the version of the contact. Every time the contact is changed, ChangeKey changes as well. This allows Exchange to apply changes to the correct version of the object.</span></span>|
|<span data-ttu-id="319fe-134">children</span><span class="sxs-lookup"><span data-stu-id="319fe-134">children</span></span>|<span data-ttu-id="319fe-135">String 集合</span><span class="sxs-lookup"><span data-stu-id="319fe-135">String collection</span></span>|<span data-ttu-id="319fe-136">联系人子女的姓名。</span><span class="sxs-lookup"><span data-stu-id="319fe-136">The names of the contact's children.</span></span>|
|<span data-ttu-id="319fe-137">companyName</span><span class="sxs-lookup"><span data-stu-id="319fe-137">companyName</span></span>|<span data-ttu-id="319fe-138">String</span><span class="sxs-lookup"><span data-stu-id="319fe-138">String</span></span>|<span data-ttu-id="319fe-139">联系人所在公司的名称。</span><span class="sxs-lookup"><span data-stu-id="319fe-139">The name of the contact's company.</span></span>|
|<span data-ttu-id="319fe-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="319fe-140">createdDateTime</span></span>|<span data-ttu-id="319fe-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319fe-141">DateTimeOffset</span></span>|<span data-ttu-id="319fe-p106">创建联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="319fe-p106">The time the contact was created. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="319fe-145">部门</span><span class="sxs-lookup"><span data-stu-id="319fe-145">department</span></span>|<span data-ttu-id="319fe-146">String</span><span class="sxs-lookup"><span data-stu-id="319fe-146">String</span></span>|<span data-ttu-id="319fe-147">联系人所在的部门。</span><span class="sxs-lookup"><span data-stu-id="319fe-147">The contact's department.</span></span>|
|<span data-ttu-id="319fe-148">displayName</span><span class="sxs-lookup"><span data-stu-id="319fe-148">displayName</span></span>|<span data-ttu-id="319fe-149">String</span><span class="sxs-lookup"><span data-stu-id="319fe-149">String</span></span>|<span data-ttu-id="319fe-150">联系人的显示名称。</span><span class="sxs-lookup"><span data-stu-id="319fe-150">The contact's display name.</span></span> <span data-ttu-id="319fe-151">您可以[创建](../api/user-post-contacts.md)或[更新](../api/contact-update.md)操作中指定的显示名称。</span><span class="sxs-lookup"><span data-stu-id="319fe-151">You can specify the display name in a [create](../api/user-post-contacts.md) or [update](../api/contact-update.md) operation.</span></span> <span data-ttu-id="319fe-152">请注意，以后对其他属性更新可能会导致自动生成的值覆盖已指定的显示名称值。</span><span class="sxs-lookup"><span data-stu-id="319fe-152">Note that later updates to other properties may cause an automatically generated value to overwrite the displayName value you have specified.</span></span> <span data-ttu-id="319fe-153">若要保留现有的值，请始终作为[更新](../api/contact-update.md)操作中的 displayName 包括它。</span><span class="sxs-lookup"><span data-stu-id="319fe-153">To preserve a pre-existing value, always include it as displayName in an [update](../api/contact-update.md) operation.</span></span>|
|<span data-ttu-id="319fe-154">emailAddresses</span><span class="sxs-lookup"><span data-stu-id="319fe-154">emailAddresses</span></span>|<span data-ttu-id="319fe-155">[typedEmailAddress](typedemailaddress.md)集合</span><span class="sxs-lookup"><span data-stu-id="319fe-155">[typedEmailAddress](typedemailaddress.md) collection</span></span>|<span data-ttu-id="319fe-156">联系人的电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="319fe-156">The contact's email addresses.</span></span>|
|<span data-ttu-id="319fe-157">fileAs</span><span class="sxs-lookup"><span data-stu-id="319fe-157">fileAs</span></span>|<span data-ttu-id="319fe-158">String</span><span class="sxs-lookup"><span data-stu-id="319fe-158">String</span></span>|<span data-ttu-id="319fe-159">联系人备案的姓名。</span><span class="sxs-lookup"><span data-stu-id="319fe-159">The name the contact is filed under.</span></span>|
|<span data-ttu-id="319fe-160">flag</span><span class="sxs-lookup"><span data-stu-id="319fe-160">flag</span></span>|[<span data-ttu-id="319fe-161">followupFlag</span><span class="sxs-lookup"><span data-stu-id="319fe-161">followupFlag</span></span>](followupflag.md)|<span data-ttu-id="319fe-162">标志值，该值指示状态、 开始日期、 截止日期或为该联系人的完成日期。</span><span class="sxs-lookup"><span data-stu-id="319fe-162">The flag value that indicates the status, start date, due date, or completion date for the contact.</span></span> |
|<span data-ttu-id="319fe-163">gender</span><span class="sxs-lookup"><span data-stu-id="319fe-163">gender</span></span> |<span data-ttu-id="319fe-164">String</span><span class="sxs-lookup"><span data-stu-id="319fe-164">String</span></span> |<span data-ttu-id="319fe-165">联系人的性别。</span><span class="sxs-lookup"><span data-stu-id="319fe-165">The contact's gender.</span></span> |
|<span data-ttu-id="319fe-166">generation</span><span class="sxs-lookup"><span data-stu-id="319fe-166">generation</span></span>|<span data-ttu-id="319fe-167">String</span><span class="sxs-lookup"><span data-stu-id="319fe-167">String</span></span>|<span data-ttu-id="319fe-168">联系人所属的代。</span><span class="sxs-lookup"><span data-stu-id="319fe-168">The contact's generation.</span></span>|
|<span data-ttu-id="319fe-169">givenName</span><span class="sxs-lookup"><span data-stu-id="319fe-169">givenName</span></span>|<span data-ttu-id="319fe-170">String</span><span class="sxs-lookup"><span data-stu-id="319fe-170">String</span></span>|<span data-ttu-id="319fe-171">联系人的名。</span><span class="sxs-lookup"><span data-stu-id="319fe-171">The contact's given name.</span></span>|
|<span data-ttu-id="319fe-172">id</span><span class="sxs-lookup"><span data-stu-id="319fe-172">id</span></span>|<span data-ttu-id="319fe-173">字串符号</span><span class="sxs-lookup"><span data-stu-id="319fe-173">String</span></span>|<span data-ttu-id="319fe-p108">联系人的唯一标识符。只读。</span><span class="sxs-lookup"><span data-stu-id="319fe-p108">The contact's unique identifier. Read-only.</span></span>|
|<span data-ttu-id="319fe-176">imAddresses</span><span class="sxs-lookup"><span data-stu-id="319fe-176">imAddresses</span></span>|<span data-ttu-id="319fe-177">String collection</span><span class="sxs-lookup"><span data-stu-id="319fe-177">String collection</span></span>|<span data-ttu-id="319fe-178">联系人的即时消息 (IM) 地址。</span><span class="sxs-lookup"><span data-stu-id="319fe-178">The contact's instant messaging (IM) addresses.</span></span>|
|<span data-ttu-id="319fe-179">initials</span><span class="sxs-lookup"><span data-stu-id="319fe-179">initials</span></span>|<span data-ttu-id="319fe-180">String</span><span class="sxs-lookup"><span data-stu-id="319fe-180">String</span></span>|<span data-ttu-id="319fe-181">联系人的姓名缩写。</span><span class="sxs-lookup"><span data-stu-id="319fe-181">The contact's initials.</span></span>|
|<span data-ttu-id="319fe-182">jobTitle</span><span class="sxs-lookup"><span data-stu-id="319fe-182">jobTitle</span></span>|<span data-ttu-id="319fe-183">String</span><span class="sxs-lookup"><span data-stu-id="319fe-183">String</span></span>|<span data-ttu-id="319fe-184">联系人的职务。</span><span class="sxs-lookup"><span data-stu-id="319fe-184">The contact’s job title.</span></span>|
|<span data-ttu-id="319fe-185">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="319fe-185">lastModifiedDateTime</span></span>|<span data-ttu-id="319fe-186">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="319fe-186">DateTimeOffset</span></span>|<span data-ttu-id="319fe-p109">修改联系人的时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。例如，2014 年 1 月 1 日午夜 UTC 类似于如下形式：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="319fe-p109">The time the contact was modified. The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="319fe-190">manager</span><span class="sxs-lookup"><span data-stu-id="319fe-190">manager</span></span>|<span data-ttu-id="319fe-191">String</span><span class="sxs-lookup"><span data-stu-id="319fe-191">String</span></span>|<span data-ttu-id="319fe-192">联系人经理的姓名。</span><span class="sxs-lookup"><span data-stu-id="319fe-192">The name of the contact's manager.</span></span>
|<span data-ttu-id="319fe-193">middleName</span><span class="sxs-lookup"><span data-stu-id="319fe-193">middleName</span></span>|<span data-ttu-id="319fe-194">String</span><span class="sxs-lookup"><span data-stu-id="319fe-194">String</span></span>|<span data-ttu-id="319fe-195">联系人的中间名。</span><span class="sxs-lookup"><span data-stu-id="319fe-195">The contact's middle name.</span></span>|
|<span data-ttu-id="319fe-196">nickName</span><span class="sxs-lookup"><span data-stu-id="319fe-196">nickName</span></span>|<span data-ttu-id="319fe-197">String</span><span class="sxs-lookup"><span data-stu-id="319fe-197">String</span></span>|<span data-ttu-id="319fe-198">联系人的昵称。</span><span class="sxs-lookup"><span data-stu-id="319fe-198">The contact's nickname.</span></span>|
|<span data-ttu-id="319fe-199">officeLocation</span><span class="sxs-lookup"><span data-stu-id="319fe-199">officeLocation</span></span>|<span data-ttu-id="319fe-200">String</span><span class="sxs-lookup"><span data-stu-id="319fe-200">String</span></span>|<span data-ttu-id="319fe-201">联系人的办公室位置。</span><span class="sxs-lookup"><span data-stu-id="319fe-201">The location of the contact's office.</span></span>|
|<span data-ttu-id="319fe-202">parentFolderId</span><span class="sxs-lookup"><span data-stu-id="319fe-202">parentFolderId</span></span>|<span data-ttu-id="319fe-203">String</span><span class="sxs-lookup"><span data-stu-id="319fe-203">String</span></span>|<span data-ttu-id="319fe-204">联系人的父文件夹 ID。</span><span class="sxs-lookup"><span data-stu-id="319fe-204">The ID of the contact's parent folder.</span></span>|
|<span data-ttu-id="319fe-205">personalNotes</span><span class="sxs-lookup"><span data-stu-id="319fe-205">personalNotes</span></span>|<span data-ttu-id="319fe-206">String</span><span class="sxs-lookup"><span data-stu-id="319fe-206">String</span></span>|<span data-ttu-id="319fe-207">有关联系人的用户备注。</span><span class="sxs-lookup"><span data-stu-id="319fe-207">The user's notes about the contact.</span></span>|
|<span data-ttu-id="319fe-208">phones</span><span class="sxs-lookup"><span data-stu-id="319fe-208">phones</span></span> |<span data-ttu-id="319fe-209">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="319fe-209">[phone](phone.md) collection</span></span> |<span data-ttu-id="319fe-210">例如，家庭电话、 移动电话和商务电话与该联系人，关联的电话号码。</span><span class="sxs-lookup"><span data-stu-id="319fe-210">Phone numbers associated with the contact, for example, home phone, mobile phone, and business phone.</span></span> |
|<span data-ttu-id="319fe-211">postalAddresses</span><span class="sxs-lookup"><span data-stu-id="319fe-211">postalAddresses</span></span> |<span data-ttu-id="319fe-212">[physicalAddress](physicaladdress.md)集合</span><span class="sxs-lookup"><span data-stu-id="319fe-212">[physicalAddress](physicaladdress.md) collection</span></span> |<span data-ttu-id="319fe-213">解决与该联系人，例如家庭地址和业务地址。</span><span class="sxs-lookup"><span data-stu-id="319fe-213">Addresses associated with the contact, for example, home address and business address.</span></span> |
|<span data-ttu-id="319fe-214">profession</span><span class="sxs-lookup"><span data-stu-id="319fe-214">profession</span></span>|<span data-ttu-id="319fe-215">String</span><span class="sxs-lookup"><span data-stu-id="319fe-215">String</span></span>|<span data-ttu-id="319fe-216">联系人的职业。</span><span class="sxs-lookup"><span data-stu-id="319fe-216">The contact's profession.</span></span>|
|<span data-ttu-id="319fe-217">spouseName</span><span class="sxs-lookup"><span data-stu-id="319fe-217">spouseName</span></span>|<span data-ttu-id="319fe-218">String</span><span class="sxs-lookup"><span data-stu-id="319fe-218">String</span></span>|<span data-ttu-id="319fe-219">联系人配偶/伴侣的姓名。</span><span class="sxs-lookup"><span data-stu-id="319fe-219">The name of the contact's spouse/partner.</span></span>|
|<span data-ttu-id="319fe-220">surname</span><span class="sxs-lookup"><span data-stu-id="319fe-220">surname</span></span>|<span data-ttu-id="319fe-221">String</span><span class="sxs-lookup"><span data-stu-id="319fe-221">String</span></span>|<span data-ttu-id="319fe-222">联系人的姓氏。</span><span class="sxs-lookup"><span data-stu-id="319fe-222">The contact's surname.</span></span>|
|<span data-ttu-id="319fe-223">title</span><span class="sxs-lookup"><span data-stu-id="319fe-223">title</span></span>|<span data-ttu-id="319fe-224">字符串</span><span class="sxs-lookup"><span data-stu-id="319fe-224">String</span></span>|<span data-ttu-id="319fe-225">联系人的职位。</span><span class="sxs-lookup"><span data-stu-id="319fe-225">The contact's title.</span></span>|
|<span data-ttu-id="319fe-226">websites</span><span class="sxs-lookup"><span data-stu-id="319fe-226">websites</span></span> |<span data-ttu-id="319fe-227">[website](website.md) collection</span><span class="sxs-lookup"><span data-stu-id="319fe-227">[website](website.md) collection</span></span>|<span data-ttu-id="319fe-228">与联系人关联的网站。</span><span class="sxs-lookup"><span data-stu-id="319fe-228">Web sites associated with the contact.</span></span> |
|<span data-ttu-id="319fe-229">WeddingAnniversary</span><span class="sxs-lookup"><span data-stu-id="319fe-229">weddingAnniversary</span></span> |<span data-ttu-id="319fe-230">日期</span><span class="sxs-lookup"><span data-stu-id="319fe-230">Date</span></span> |<span data-ttu-id="319fe-231">联系人的婚礼周年日。</span><span class="sxs-lookup"><span data-stu-id="319fe-231">The contact's wedding anniversary.</span></span> |
|<span data-ttu-id="319fe-232">yomiCompanyName</span><span class="sxs-lookup"><span data-stu-id="319fe-232">yomiCompanyName</span></span>|<span data-ttu-id="319fe-233">String</span><span class="sxs-lookup"><span data-stu-id="319fe-233">String</span></span>|<span data-ttu-id="319fe-234">联系人的注音日文公司名称。</span><span class="sxs-lookup"><span data-stu-id="319fe-234">The phonetic Japanese company name of the contact.</span></span>|
|<span data-ttu-id="319fe-235">yomiGivenName</span><span class="sxs-lookup"><span data-stu-id="319fe-235">yomiGivenName</span></span>|<span data-ttu-id="319fe-236">String</span><span class="sxs-lookup"><span data-stu-id="319fe-236">String</span></span>|<span data-ttu-id="319fe-237">联系人的注音日文名字。</span><span class="sxs-lookup"><span data-stu-id="319fe-237">The phonetic Japanese given name (first name) of the contact.</span></span>|
|<span data-ttu-id="319fe-238">yomiSurname</span><span class="sxs-lookup"><span data-stu-id="319fe-238">yomiSurname</span></span>|<span data-ttu-id="319fe-239">String</span><span class="sxs-lookup"><span data-stu-id="319fe-239">String</span></span>|<span data-ttu-id="319fe-240">联系人的注音日文姓氏。</span><span class="sxs-lookup"><span data-stu-id="319fe-240">The phonetic Japanese surname (last name)  of the contact.</span></span>|

## <a name="relationships"></a><span data-ttu-id="319fe-241">关系</span><span class="sxs-lookup"><span data-stu-id="319fe-241">Relationships</span></span>
| <span data-ttu-id="319fe-242">关系</span><span class="sxs-lookup"><span data-stu-id="319fe-242">Relationship</span></span> | <span data-ttu-id="319fe-243">类型</span><span class="sxs-lookup"><span data-stu-id="319fe-243">Type</span></span>   |<span data-ttu-id="319fe-244">说明</span><span class="sxs-lookup"><span data-stu-id="319fe-244">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="319fe-245">extensions</span><span class="sxs-lookup"><span data-stu-id="319fe-245">extensions</span></span>|<span data-ttu-id="319fe-246">[扩展](extension.md)集合</span><span class="sxs-lookup"><span data-stu-id="319fe-246">[extension](extension.md) collection</span></span>|<span data-ttu-id="319fe-247">打开扩展名为该联系人定义的集合。</span><span class="sxs-lookup"><span data-stu-id="319fe-247">The collection of open extensions defined for the contact.</span></span> <span data-ttu-id="319fe-248">可为 Null。</span><span class="sxs-lookup"><span data-stu-id="319fe-248">Nullable.</span></span>|
|<span data-ttu-id="319fe-249">multiValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="319fe-249">multiValueExtendedProperties</span></span>|<span data-ttu-id="319fe-250">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="319fe-250">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="319fe-p111">为联系人定义的多值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="319fe-p111">The collection of multi-value extended properties defined for the contact. Read-only. Nullable.</span></span>|
|<span data-ttu-id="319fe-254">photo</span><span class="sxs-lookup"><span data-stu-id="319fe-254">photo</span></span>|[<span data-ttu-id="319fe-255">照片</span><span class="sxs-lookup"><span data-stu-id="319fe-255">photo</span></span>](profilephoto.md)| <span data-ttu-id="319fe-p112">可选的联系人照片。可以获取或设置联系人的照片。</span><span class="sxs-lookup"><span data-stu-id="319fe-p112">Optional contact picture. You can get or set a photo for a contact.</span></span>|
|<span data-ttu-id="319fe-258">singleValueExtendedProperties</span><span class="sxs-lookup"><span data-stu-id="319fe-258">singleValueExtendedProperties</span></span>|<span data-ttu-id="319fe-259">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span><span class="sxs-lookup"><span data-stu-id="319fe-259">[singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) collection</span></span>| <span data-ttu-id="319fe-p113">为联系人定义的单值扩展属性的集合。只读。可为 Null。</span><span class="sxs-lookup"><span data-stu-id="319fe-p113">The collection of single-value extended properties defined for the contact. Read-only. Nullable.</span></span>|

## <a name="methods"></a><span data-ttu-id="319fe-263">方法</span><span class="sxs-lookup"><span data-stu-id="319fe-263">Methods</span></span>
| <span data-ttu-id="319fe-264">方法</span><span class="sxs-lookup"><span data-stu-id="319fe-264">Method</span></span>           | <span data-ttu-id="319fe-265">返回类型</span><span class="sxs-lookup"><span data-stu-id="319fe-265">Return Type</span></span>    |<span data-ttu-id="319fe-266">说明</span><span class="sxs-lookup"><span data-stu-id="319fe-266">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="319fe-267">获取联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-267">Get contact</span></span>](../api/contact-get.md) | [<span data-ttu-id="319fe-268">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-268">contact</span></span>](contact.md) |<span data-ttu-id="319fe-269">读取 contact 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="319fe-269">Read properties and relationships of contact object.</span></span>|
|[<span data-ttu-id="319fe-270">创建</span><span class="sxs-lookup"><span data-stu-id="319fe-270">Create</span></span>](../api/user-post-contacts.md) | [<span data-ttu-id="319fe-271">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-271">contact</span></span>](contact.md) |<span data-ttu-id="319fe-272">将联系人添加到联系人根文件夹或其他联系人文件夹的联系人端点中。</span><span class="sxs-lookup"><span data-stu-id="319fe-272">Add a contact to the root Contacts folder or to the contacts endpoint of another contact folder.</span></span>|
|[<span data-ttu-id="319fe-273">更新</span><span class="sxs-lookup"><span data-stu-id="319fe-273">Update</span></span>](../api/contact-update.md) | [<span data-ttu-id="319fe-274">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-274">contact</span></span>](contact.md) |<span data-ttu-id="319fe-275">更新 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="319fe-275">Update contact object.</span></span> |
|[<span data-ttu-id="319fe-276">删除</span><span class="sxs-lookup"><span data-stu-id="319fe-276">Delete</span></span>](../api/contact-delete.md) | <span data-ttu-id="319fe-277">无</span><span class="sxs-lookup"><span data-stu-id="319fe-277">None</span></span> |<span data-ttu-id="319fe-278">删除 contact 对象。</span><span class="sxs-lookup"><span data-stu-id="319fe-278">Delete contact object.</span></span> |
|[<span data-ttu-id="319fe-279">delta</span><span class="sxs-lookup"><span data-stu-id="319fe-279">delta</span></span>](../api/contact-delta.md)|<span data-ttu-id="319fe-280">[联系人](contact.md)集合</span><span class="sxs-lookup"><span data-stu-id="319fe-280">[contact](contact.md) collection</span></span>| <span data-ttu-id="319fe-281">获取指定文件夹中已添加、删除或更新的联系人集。</span><span class="sxs-lookup"><span data-stu-id="319fe-281">Get a set of contacts that have been added, deleted, or updated in a specified folder.</span></span>|
|<span data-ttu-id="319fe-282">**开放扩展**</span><span class="sxs-lookup"><span data-stu-id="319fe-282">**Open extensions**</span></span>| | |
|[<span data-ttu-id="319fe-283">创建开放扩展</span><span class="sxs-lookup"><span data-stu-id="319fe-283">Create open extension</span></span>](../api/opentypeextension-post-opentypeextension.md) |[<span data-ttu-id="319fe-284">openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="319fe-284">openTypeExtension</span></span>](opentypeextension.md)| <span data-ttu-id="319fe-285">创建开放扩展，并将自定义属性添加到新资源或现有资源。</span><span class="sxs-lookup"><span data-stu-id="319fe-285">Create an open extension and add custom properties to a new or existing resource.</span></span>|
|[<span data-ttu-id="319fe-286">获取开放扩展</span><span class="sxs-lookup"><span data-stu-id="319fe-286">Get open extension</span></span>](../api/opentypeextension-get.md) |<span data-ttu-id="319fe-287">[openTypeExtension](opentypeextension.md) 集合</span><span class="sxs-lookup"><span data-stu-id="319fe-287">[openTypeExtension](opentypeextension.md) collection</span></span>| <span data-ttu-id="319fe-288">获取扩展名称标识的开放扩展。</span><span class="sxs-lookup"><span data-stu-id="319fe-288">Get an open extension identified by the extension name.</span></span>|
|<span data-ttu-id="319fe-289">**架构扩展**</span><span class="sxs-lookup"><span data-stu-id="319fe-289">**Schema extensions**</span></span>| | |
|[<span data-ttu-id="319fe-290">添加架构扩展值</span><span class="sxs-lookup"><span data-stu-id="319fe-290">Add schema extension values</span></span>](/graph/extensibility-schema-groups) || <span data-ttu-id="319fe-291">创建架构扩展定义，然后使用它向资源添加自定义键入数据。</span><span class="sxs-lookup"><span data-stu-id="319fe-291">Create a schema extension definition and then use it to add custom typed data to a resource.</span></span>|
|<span data-ttu-id="319fe-292">**扩展属性**</span><span class="sxs-lookup"><span data-stu-id="319fe-292">**Extended properties**</span></span>| | |
|[<span data-ttu-id="319fe-293">创建单值扩展属性</span><span class="sxs-lookup"><span data-stu-id="319fe-293">Create single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) |[<span data-ttu-id="319fe-294">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-294">contact</span></span>](contact.md)  |<span data-ttu-id="319fe-295">在新建或现有的联系人中创建一个或多个单值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="319fe-295">Create one or more single-value extended properties in a new or existing contact.</span></span>   |
|[<span data-ttu-id="319fe-296">获取具有单值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-296">Get contact with single-value extended property</span></span>](../api/singlevaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="319fe-297">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-297">contact</span></span>](contact.md) | <span data-ttu-id="319fe-298">通过使用 `$expand` 或 `$filter` 获取包含一个单值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="319fe-298">Get contacts that contain a single-value extended property by using `$expand` or `$filter`.</span></span> |
|[<span data-ttu-id="319fe-299">创建多值扩展属性</span><span class="sxs-lookup"><span data-stu-id="319fe-299">Create multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | [<span data-ttu-id="319fe-300">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-300">contact</span></span>](contact.md) | <span data-ttu-id="319fe-301">在新建或现有的联系人中创建一个或多个多值扩展属性。</span><span class="sxs-lookup"><span data-stu-id="319fe-301">Create one or more multi-value extended properties in a new or existing contact.</span></span>  |
|[<span data-ttu-id="319fe-302">获取具有多值扩展属性的联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-302">Get contact with multi-value extended property</span></span>](../api/multivaluelegacyextendedproperty-get.md)  | [<span data-ttu-id="319fe-303">联系人</span><span class="sxs-lookup"><span data-stu-id="319fe-303">contact</span></span>](contact.md) | <span data-ttu-id="319fe-304">使用 `$expand` 获取包含一个多值扩展属性的联系人。</span><span class="sxs-lookup"><span data-stu-id="319fe-304">Get a contact that contains a multi-value extended property by using `$expand`.</span></span> |

## <a name="see-also"></a><span data-ttu-id="319fe-305">另请参阅</span><span class="sxs-lookup"><span data-stu-id="319fe-305">See also</span></span>

- [<span data-ttu-id="319fe-306">使用增量查询跟踪 Microsoft Graph 数据更改</span><span class="sxs-lookup"><span data-stu-id="319fe-306">Use delta query to track changes in Microsoft Graph data</span></span>](/graph/delta-query-overview)
- [<span data-ttu-id="319fe-307">获取文件夹中邮件的增量更改</span><span class="sxs-lookup"><span data-stu-id="319fe-307">Get incremental changes to messages in a folder</span></span>](/graph/delta-query-messages)
- [<span data-ttu-id="319fe-308">使用扩展向资源添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="319fe-308">Add custom data to resources using extensions</span></span>](/graph/extensibility-overview)
- [<span data-ttu-id="319fe-309">使用开放扩展向用户添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="319fe-309">Add custom data to users using open extensions</span></span>](/graph/extensibility-open-users)
- [<span data-ttu-id="319fe-310">使用架构扩展向组添加自定义数据</span><span class="sxs-lookup"><span data-stu-id="319fe-310">Add custom data to groups using schema extensions</span></span>](/graph/extensibility-schema-groups)


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "contact resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contact.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
