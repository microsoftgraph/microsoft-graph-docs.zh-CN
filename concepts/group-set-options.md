---
title: 设置 Microsoft 365 组行为与预配选项
description: 在 Microsoft Graph 使用组资源，你可以设置创建 Microsoft 365 组时要预配的特定组行为和资源。
author: Jordanndahl
localization_priority: Priority
ms.openlocfilehash: 54e4622a69f33980494962882ac1aa06d07eaec5
ms.sourcegitcommit: 4fa6fcc058c7f8d8cad58c0b82db23d6c7da37d2
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/27/2021
ms.locfileid: "52682178"
---
# <a name="set-microsoft-365-group-behaviors-and-provisioning-options-preview"></a><span data-ttu-id="6f17c-103">设置 Microsoft 365 组行为与预配选项（预览）</span><span class="sxs-lookup"><span data-stu-id="6f17c-103">Set Microsoft 365 group behaviors and provisioning options (preview)</span></span>

<span data-ttu-id="6f17c-104">使用 Microsoft Graph 中的 [组](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) ，可设置创建 Microsoft 365 组时要预配的特定组行为和资源。</span><span class="sxs-lookup"><span data-stu-id="6f17c-104">Using the [group](/graph/api/resources/group?view=graph-rest-beta&preserve-view=true) resource in Microsoft Graph, you can set specific group behaviors and resources to provision when creating a Microsoft 365 group.</span></span> <span data-ttu-id="6f17c-105">根据资源，还可在组更新时预配某些内容。</span><span class="sxs-lookup"><span data-stu-id="6f17c-105">Depending on the resource, some can also be provisioned on group update.</span></span>

### <a name="configuring-and-provisioning-groups"></a><span data-ttu-id="6f17c-106">配置和预配组</span><span class="sxs-lookup"><span data-stu-id="6f17c-106">Configuring and provisioning groups</span></span>

<span data-ttu-id="6f17c-107">**组** 资源公开两个属性，即 **resourceBehaviorOptions** 和 **resourceProvisioningOptions**，用于自定义创建组时要预配的行为和资源。</span><span class="sxs-lookup"><span data-stu-id="6f17c-107">The **group** resource exposes two properties, **resourceBehaviorOptions** and **resourceProvisioningOptions**, to customize the behaviors and resources to be provisioned upon group creation.</span></span> 

> [!NOTE]
> <span data-ttu-id="6f17c-108">**resourceBehaviortions** 和 **resourceProvisioningOptions** 属性目前仅可用于 Microsoft Graph beta 版终结点。 </span><span class="sxs-lookup"><span data-stu-id="6f17c-108">The **resourceBehaviorOptions** and **resourceProvisioningOptions** properties are currently available in only the Microsoft Graph beta endpoint.</span></span> <span data-ttu-id="6f17c-109">请勿在生产应用中使用它们，因为它们可能在没有通知的情况下随时更改。</span><span class="sxs-lookup"><span data-stu-id="6f17c-109">Do not use them in production apps, as they are subject to change without notice.</span></span>

<span data-ttu-id="6f17c-110">**resourceBehaviorOptions** 是一个字符串集合，用于为 Microsoft 365 组指定组行为。</span><span class="sxs-lookup"><span data-stu-id="6f17c-110">**resourceBehaviorOptions** is a string collection that specifies group behaviors for a Microsoft 365 group.</span></span> <span data-ttu-id="6f17c-111">这些行为只能在 [组创建](/graph/api/group-post-groups?view=graph-rest-beta&preserve-view=true)时设置 (`POST`)。</span><span class="sxs-lookup"><span data-stu-id="6f17c-111">These behaviors can be set only on [group creation](/graph/api/group-post-groups?view=graph-rest-beta&preserve-view=true) (`POST`).</span></span>

| <span data-ttu-id="6f17c-112">resourceBehaviorOptions 支持的值</span><span class="sxs-lookup"><span data-stu-id="6f17c-112">Supported values for resourceBehaviorOptions</span></span>   |<span data-ttu-id="6f17c-113">说明</span><span class="sxs-lookup"><span data-stu-id="6f17c-113">Description</span></span>|<span data-ttu-id="6f17c-114">如果未设置，则为默认值</span><span class="sxs-lookup"><span data-stu-id="6f17c-114">Default if not set</span></span>|
|:---------------|:--------|:-----------|
| <span data-ttu-id="6f17c-115">AllowOnlyMembersToPost</span><span class="sxs-lookup"><span data-stu-id="6f17c-115">AllowOnlyMembersToPost</span></span>|<span data-ttu-id="6f17c-116">只有组 *成员* 可以向组发布对话。</span><span class="sxs-lookup"><span data-stu-id="6f17c-116">Only group *members* can post conversations to the group.</span></span>|<span data-ttu-id="6f17c-117">组织中的任何用户都可以向组发布对话。</span><span class="sxs-lookup"><span data-stu-id="6f17c-117">Any user in the organization can post conversations to the group.</span></span>|
| <span data-ttu-id="6f17c-118">HideGroupInOutlook</span><span class="sxs-lookup"><span data-stu-id="6f17c-118">HideGroupInOutlook</span></span>|<span data-ttu-id="6f17c-119">此组在 Outlook 体验中是隐藏的。</span><span class="sxs-lookup"><span data-stu-id="6f17c-119">This group is hidden in Outlook experiences.</span></span>|<span data-ttu-id="6f17c-120">所有组在 Outlook 体验中都是可见的，也是可发现的。</span><span class="sxs-lookup"><span data-stu-id="6f17c-120">All groups are visible and discoverable in Outlook experiences.</span></span>|
| <span data-ttu-id="6f17c-121">SubscribeNewGroupMembers</span><span class="sxs-lookup"><span data-stu-id="6f17c-121">SubscribeNewGroupMembers</span></span>|<span data-ttu-id="6f17c-122">成员可以订阅接收组对话。</span><span class="sxs-lookup"><span data-stu-id="6f17c-122">Group members are subscribed to receive group conversations.</span></span> |<span data-ttu-id="6f17c-123">组成员不接收组对话。</span><span class="sxs-lookup"><span data-stu-id="6f17c-123">Group members do not receive group conversations.</span></span>|
| <span data-ttu-id="6f17c-124">WelcomeEmailDisabled</span><span class="sxs-lookup"><span data-stu-id="6f17c-124">WelcomeEmailDisabled</span></span>|<span data-ttu-id="6f17c-125">欢迎电子邮件不会发送给新成员。</span><span class="sxs-lookup"><span data-stu-id="6f17c-125">Welcome emails are not sent to new members.</span></span>|<span data-ttu-id="6f17c-126">加入组时，会将欢迎电子邮件发送到新成员。</span><span class="sxs-lookup"><span data-stu-id="6f17c-126">A welcome email is sent to a new member on joining the group.</span></span>|

<span data-ttu-id="6f17c-127">**resourceProvisioningOptions** 是一个字符串集合，用于指定作为创建 Microsoft 365 组的一部分进行预配的组资源，但这些组资源通常不是默认组创建的组成部分。</span><span class="sxs-lookup"><span data-stu-id="6f17c-127">**resourceProvisioningOptions** is a string collection that specifies group resources to be provisioned as part of creating the Microsoft 365 group, that are not normally part of default group creation.</span></span>

| <span data-ttu-id="6f17c-128">resourceProvisioningOptions 支持的值</span><span class="sxs-lookup"><span data-stu-id="6f17c-128">Supported values for resourceProvisioningOptions</span></span>   |<span data-ttu-id="6f17c-129">说明</span><span class="sxs-lookup"><span data-stu-id="6f17c-129">Description</span></span>| <span data-ttu-id="6f17c-130">如果未设置，则为默认值</span><span class="sxs-lookup"><span data-stu-id="6f17c-130">Default if not set</span></span> |
|:---------------|:--------|:------------|
| <span data-ttu-id="6f17c-131">Teams</span><span class="sxs-lookup"><span data-stu-id="6f17c-131">Teams</span></span>|<span data-ttu-id="6f17c-p104">将此组预配为 Microsoft Teams 中的团队。此外，此值可通过 `PATCH` 操作添加到 [组更新](/graph/api/group-update?view=graph-rest-beta&preserve-view=true) 上的 **resourceProvisioningOptions** 字符串集合，以便将现有的 Microsoft 365 组转换为团队。</span><span class="sxs-lookup"><span data-stu-id="6f17c-p104">Provision this group as a team in Microsoft Teams. Additionally, this value can be added to the **resourceProvisioningOptions** string collection on [group update](/graph/api/group-update?view=graph-rest-beta&preserve-view=true) through a `PATCH` operation, in order to convert an existing Microsoft 365 group to a team.</span></span>| <span data-ttu-id="6f17c-134">此组是没有 Teams 功能的常规 Microsoft 365 组。</span><span class="sxs-lookup"><span data-stu-id="6f17c-134">The group is a regular Microsoft 365 group without Teams capabilities.</span></span>|


## <a name="see-also"></a><span data-ttu-id="6f17c-135">另请参阅</span><span class="sxs-lookup"><span data-stu-id="6f17c-135">See also</span></span>

- [<span data-ttu-id="6f17c-136">Microsoft Graph 中的 Microsoft 365 组概述</span><span class="sxs-lookup"><span data-stu-id="6f17c-136">Overview of Microsoft 365 groups in Microsoft Graph</span></span>](office365-groups-concept-overview.md)
- [<span data-ttu-id="6f17c-137">Microsoft Teams API 概述</span><span class="sxs-lookup"><span data-stu-id="6f17c-137">Microsoft Teams API overview</span></span>](teams-concept-overview.md)
