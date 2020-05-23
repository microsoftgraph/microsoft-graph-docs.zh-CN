---
title: 设置 Microsoft 365 组行为和设置选项
description: 在 Microsoft Graph 中使用组资源，您可以设置特定的组行为和资源，以便在创建 Microsoft 365 组时进行设置。
author: yyuank
localization_priority: Priority
ms.openlocfilehash: 9df8f3d4fadea93e45089870351531619cd2fde9
ms.sourcegitcommit: c1935e442ee973c6c3fcb01a15d76bcfa625362e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/22/2020
ms.locfileid: "44345785"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a><span data-ttu-id="ca204-103">设置 Microsoft 365 组行为和设置选项（预览）</span><span class="sxs-lookup"><span data-stu-id="ca204-103">Set Microsoft 365 group behaviors and provisioning options (preview)</span></span>

<span data-ttu-id="ca204-104">在 Microsoft Graph 中使用[组](/graph/api/resources/group?view=graph-rest-beta)资源，您可以设置特定的组行为和资源，以便在创建 Microsoft 365 组时进行设置。</span><span class="sxs-lookup"><span data-stu-id="ca204-104">Using the [group](/graph/api/resources/group?view=graph-rest-beta) resource in Microsoft Graph, you can set specific group behaviors and resources to provision when creating a Microsoft 365 group.</span></span> <span data-ttu-id="ca204-105">根据资源的不同，还可以在组更新中进行设置。</span><span class="sxs-lookup"><span data-stu-id="ca204-105">Depending on the resource, some can also be provisioned on group update.</span></span>

### <a name="configuring-and-provisioning-groups"></a><span data-ttu-id="ca204-106">配置和设置组</span><span class="sxs-lookup"><span data-stu-id="ca204-106">Configuring and provisioning groups</span></span>

<span data-ttu-id="ca204-107">**Group**资源公开两个属性（ **resourceBehaviorOptions**和**resourceProvisioningOptions**），以自定义要在创建组时设置的行为和资源。</span><span class="sxs-lookup"><span data-stu-id="ca204-107">The **group** resource exposes two properties, **resourceBehaviorOptions** and **resourceProvisioningOptions**, to customize the behaviors and resources to be provisioned upon group creation.</span></span> 

> [!NOTE]
> <span data-ttu-id="ca204-108">**ResourceBehaviorOptions**和**resourceProvisioningOptions**属性当前仅在 Microsoft Graph beta 终结点中可用。</span><span class="sxs-lookup"><span data-stu-id="ca204-108">The **resourceBehaviorOptions** and **resourceProvisioningOptions** properties are currently available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="ca204-109">请勿在生产应用程序中使用它们，因为它们可能会更改，恕不另行通知。</span><span class="sxs-lookup"><span data-stu-id="ca204-109">Do not use them in production apps, as they are subject to change without notice.</span></span>

<span data-ttu-id="ca204-110">**resourceBehaviorOptions**是一个字符串集合，用于指定 Microsoft 365 组的组行为。</span><span class="sxs-lookup"><span data-stu-id="ca204-110">**resourceBehaviorOptions** is a string collection that specifies group behaviors for a Microsoft 365 group.</span></span> <span data-ttu-id="ca204-111">只能在 "[创建组](/graph/api/group-post-groups?view=graph-rest-beta)" （）中设置这些 bahaviors `POST` 。</span><span class="sxs-lookup"><span data-stu-id="ca204-111">These bahaviors can be set only on [group creation](/graph/api/group-post-groups?view=graph-rest-beta) (`POST`).</span></span>

| <span data-ttu-id="ca204-112">ResourceBehaviorOptions 支持的值</span><span class="sxs-lookup"><span data-stu-id="ca204-112">Supported values for resourceBehaviorOptions</span></span>   |<span data-ttu-id="ca204-113">说明</span><span class="sxs-lookup"><span data-stu-id="ca204-113">Description</span></span>|<span data-ttu-id="ca204-114">如果未设置，则为默认值</span><span class="sxs-lookup"><span data-stu-id="ca204-114">Default if not set</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="ca204-115">AllowOnlyMembersToPost</span><span class="sxs-lookup"><span data-stu-id="ca204-115">AllowOnlyMembersToPost</span></span>|<span data-ttu-id="ca204-116">只有组*成员*可以向组发布对话。</span><span class="sxs-lookup"><span data-stu-id="ca204-116">Only group *members* can post conversations to the group.</span></span>|<span data-ttu-id="ca204-117">组织中的任何用户都可以向组发布对话。</span><span class="sxs-lookup"><span data-stu-id="ca204-117">Any user in the organization can post conversations to the group.</span></span>|
| <span data-ttu-id="ca204-118">HideGroupInOutlook</span><span class="sxs-lookup"><span data-stu-id="ca204-118">HideGroupInOutlook</span></span>|<span data-ttu-id="ca204-119">此组在 Outlook 体验中处于隐藏状态。</span><span class="sxs-lookup"><span data-stu-id="ca204-119">This group is hidden in Outlook experiences.</span></span>|<span data-ttu-id="ca204-120">在 Outlook 体验中，所有组都是可见且可发现的。</span><span class="sxs-lookup"><span data-stu-id="ca204-120">All groups are visible and discoverable in Outlook experiences.</span></span>|
| <span data-ttu-id="ca204-121">SubscribeNewGroupMembers</span><span class="sxs-lookup"><span data-stu-id="ca204-121">SubscribeNewGroupMembers</span></span>|<span data-ttu-id="ca204-122">成员可以订阅接收组对话。</span><span class="sxs-lookup"><span data-stu-id="ca204-122">Group members are subscribed to receive group conversations.</span></span> |<span data-ttu-id="ca204-123">组成员不接收组对话。</span><span class="sxs-lookup"><span data-stu-id="ca204-123">Group members do not receive group conversations.</span></span>|
| <span data-ttu-id="ca204-124">WelcomeEmailDisabled</span><span class="sxs-lookup"><span data-stu-id="ca204-124">WelcomeEmailDisabled</span></span>|<span data-ttu-id="ca204-125">加入组时，会将欢迎电子邮件发送到新成员。</span><span class="sxs-lookup"><span data-stu-id="ca204-125">A welcome email is sent to a new member on joining the group.</span></span>|<span data-ttu-id="ca204-126">欢迎电子邮件不会发送给新成员。</span><span class="sxs-lookup"><span data-stu-id="ca204-126">Welcome emails are not sent to new members.</span></span>|

<span data-ttu-id="ca204-127">**resourceProvisioningOptions**是一个字符串集合，用于指定要作为创建 Microsoft 365 组的一部分进行设置的组资源，这些资源通常不是默认组创建的一部分。</span><span class="sxs-lookup"><span data-stu-id="ca204-127">**resourceProvisioningOptions** is a string collection that specifies group resources to be provisioned as part of creating the Microsoft 365 group, that are not normally part of default group creation.</span></span>

| <span data-ttu-id="ca204-128">ResourceProvisioningOptions 支持的值</span><span class="sxs-lookup"><span data-stu-id="ca204-128">Supported values for resourceProvisioningOptions</span></span>   |<span data-ttu-id="ca204-129">说明</span><span class="sxs-lookup"><span data-stu-id="ca204-129">Description</span></span>| <span data-ttu-id="ca204-130">如果未设置，则为默认值</span><span class="sxs-lookup"><span data-stu-id="ca204-130">Default if not set</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="ca204-131">Teams</span><span class="sxs-lookup"><span data-stu-id="ca204-131">Teams</span></span>|<span data-ttu-id="ca204-132">将此组设置为 Microsoft 团队中的团队。</span><span class="sxs-lookup"><span data-stu-id="ca204-132">Provision this group as a team in Microsoft Teams.</span></span> <span data-ttu-id="ca204-133">此外，还可以通过操作将此值添加到[组更新](/graph/api/group-update?view=graph-rest-beta)中的**resourceProvisioningOptions**字符串集合 `PATCH` ，以便将现有的 Microsoft 365 组转换为团队。</span><span class="sxs-lookup"><span data-stu-id="ca204-133">Additionally, this value can be added to the **resourceProvisioningOptions** string collection on [group update](/graph/api/group-update?view=graph-rest-beta) through a `PATCH` operation, in order to convert an existing Microsoft 365 group to a team.</span></span>| <span data-ttu-id="ca204-134">该组是不带团队功能的常规 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="ca204-134">The group is a regular Microsoft 365 group without Teams capabilities.</span></span>|


## <a name="see-also"></a><span data-ttu-id="ca204-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="ca204-135">See also</span></span>

- [<span data-ttu-id="ca204-136">Microsoft Graph 中的 Microsoft 365 组概述</span><span class="sxs-lookup"><span data-stu-id="ca204-136">Overview of Microsoft 365 groups in Microsoft Graph</span></span>](office365-groups-concept-overview.md)
- [<span data-ttu-id="ca204-137">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="ca204-137">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
