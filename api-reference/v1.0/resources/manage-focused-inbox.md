---
title: 管理重点收件箱
description: '重点收件箱使用户可以查看中的重要邮件`Focused`选项卡的收件箱和收件箱邮件的 rest`Other`选项卡。分类系统 '
ms.openlocfilehash: 1e1a4fa091c618c4f51a5621b8800d35c8c4cf5d
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011625"
---
# <a name="manage-focused-inbox"></a><span data-ttu-id="cbb40-103">管理重点收件箱</span><span class="sxs-lookup"><span data-stu-id="cbb40-103">Manage Focused Inbox</span></span>

<span data-ttu-id="cbb40-p101">通过重点收件箱，你可以查看收件箱的 `Focused` 选项卡中的重要邮件和 `Other` 选项卡中的其余收件箱邮件。分类系统最初按照默认方式组织收件箱邮件。可以随着时间推移通过用户界面或以编程方式对系统进行更正和培训。使用地越多，系统越能更好地推断哪些传入邮件是重要的。</span><span class="sxs-lookup"><span data-stu-id="cbb40-p101">Focused Inbox allows you to view important messages in the `Focused` tab of the Inbox, and the rest of the Inbox messages in the `Other` tab. The classification system initially organizes Inbox messages in a default way. You can correct and train the system over time through the user interface or programmatically. The more you use it, the better the system can infer which incoming message as important.</span></span>

<span data-ttu-id="cbb40-p102">在编程级别，重点收件箱 REST API 适用于指定用户的邮件，并支持每个邮件的 **inferenceClassification** 属性。可能的值为 `Focused` 和 `Other`，分别指示用户是否将邮件视为较重要和不太重要。若要更正系统对邮件进行分类的方式，请 [更新此邮件的 inferenceClassification 属性](../api/message-update.md)。随着时间的推移，这些更正也能对邮件分类系统进行培训。</span><span class="sxs-lookup"><span data-stu-id="cbb40-p102">At the programmatic level, the Focused Inbox REST API works on the specified user's messages, and supports an **inferenceClassification** property for each message. The possible values are `Focused` and `Other`, which indicate whether the user considers that message as, respectively, more important and less important. To correct how the system classifies a message, [update the inferenceClassification property of that message](../api/message-update.md). Over time, these corrections also train the message classification system.</span></span>

<span data-ttu-id="cbb40-p103">重点收件箱 REST API 还使你能够创建替代。由 [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) 实例表示的每个替代，会指示分类系统始终以一致的方式指定来自特定发件人的邮件（即，始终作为“重点”或“其他”），而与任何以前的学习方法无关。可以 [创建](../api/inferenceclassification-post-overrides.md)、[列出](../api/inferenceclassification-list-overrides.md)、[更新](../api/inferenceclassificationoverride-update.md) 和 [删除](../api/inferenceclassificationoverride-delete.md) 指定用户的替代。可以在 **inferenceClassification** 导航属性中访问该用户的替代（如有），这些替代是 **inferenceClassificationOverride** 实例的集合。替代使用户能够更好地控制传入邮件的分类，并提高分类系统的可靠性。</span><span class="sxs-lookup"><span data-stu-id="cbb40-p103">The Focused Inbox REST API also lets you create overrides. Each override, represented by an [inferenceClassificationOverride](../resources/inferenceclassificationoverride.md) instance, is an instruction for the classification system to always designate messages from a specific sender in a consistent way (i.e., always as "Focused" or always as "Other"), regardless of any previously learned approach. You can [create](../api/inferenceclassification-post-overrides.md), [list](../api/inferenceclassification-list-overrides.md), [update](../api/inferenceclassificationoverride-update.md) and [delete](../api/inferenceclassificationoverride-delete.md) overrides for the specified user. That user's overrides, if any, are accessible in an **inferenceClassification** navigation property, which is a collection of **inferenceClassificationOverride** instances. Overrides allow a user more control over the classification of incoming messages, and build greater trust of the classification system.</span></span>

<span data-ttu-id="cbb40-p104">注意，分类系统学习分类并仅对收件箱中的传入邮件应用分类。默认情况下，其他文件夹中的邮件为“重点”邮件。设置替代会影响以后到达收件箱的邮件；替代不会修改任意文件夹（包括收件箱）中现有邮件的 **inferenceClassification** 属性。</span><span class="sxs-lookup"><span data-stu-id="cbb40-p104">Note that the classification system learns and applies classification only on incoming messages in the Inbox. Messages in other folders are by default "Focused". Setting up an override affects future messages arriving in the Inbox; the override doesn't modify the **inferenceClassification** property in existing messages in any folder including the Inbox.</span></span>

## <a name="focused-inbox-api"></a><span data-ttu-id="cbb40-119">重点收件箱 API</span><span class="sxs-lookup"><span data-stu-id="cbb40-119">Focused Inbox API</span></span>

<span data-ttu-id="cbb40-120">**对邮件分类系统进行培训**</span><span class="sxs-lookup"><span data-stu-id="cbb40-120">**Training the message classification system**</span></span>

[<span data-ttu-id="cbb40-121">更新邮件的 inferenceClassification 属性</span><span class="sxs-lookup"><span data-stu-id="cbb40-121">Update the inferenceClassification property of a message</span></span>](../api/message-update.md)


<span data-ttu-id="cbb40-122">**使用替代对每个发件人一致分类**</span><span class="sxs-lookup"><span data-stu-id="cbb40-122">**Using overrides to classify consistently per sender**</span></span>

<span data-ttu-id="cbb40-123">[创建发件人替代](../api/inferenceclassification-post-overrides.md) | [列出所有用户替代](../api/inferenceclassification-list-overrides.md) |</span><span class="sxs-lookup"><span data-stu-id="cbb40-123">[Create an override for a sender](../api/inferenceclassification-post-overrides.md) | [List all user overrides](../api/inferenceclassification-list-overrides.md) |</span></span>

<span data-ttu-id="cbb40-124">[更新发件人替代](../api/inferenceclassificationoverride-update.md) | [删除发件人替代](../api/inferenceclassificationoverride-delete.md)</span><span class="sxs-lookup"><span data-stu-id="cbb40-124">[Update an override for a sender](../api/inferenceclassificationoverride-update.md) | [Delete a sender override](../api/inferenceclassificationoverride-delete.md)</span></span> 
