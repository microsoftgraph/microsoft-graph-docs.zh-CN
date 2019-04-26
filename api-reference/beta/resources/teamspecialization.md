---
title: teamSpecialization 枚举类型
description: 描述团队的特殊用例。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8700896c32a83a3e157186f405c435589ce03815
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345679"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="2755f-103">teamSpecialization 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2755f-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2755f-104">指示[团队](../resources/team.md)是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="2755f-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="2755f-105">每个[团队](../resources/team.md)特殊化都有权访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="2755f-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="2755f-106">默认值为 "无"。</span><span class="sxs-lookup"><span data-stu-id="2755f-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="2755f-107">成员</span><span class="sxs-lookup"><span data-stu-id="2755f-107">Members</span></span>

| <span data-ttu-id="2755f-108">成员</span><span class="sxs-lookup"><span data-stu-id="2755f-108">Member</span></span>             | <span data-ttu-id="2755f-109">值</span><span class="sxs-lookup"><span data-stu-id="2755f-109">Value</span></span> | <span data-ttu-id="2755f-110">说明</span><span class="sxs-lookup"><span data-stu-id="2755f-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="2755f-111">无</span><span class="sxs-lookup"><span data-stu-id="2755f-111">none</span></span>               | <span data-ttu-id="2755f-112">0</span><span class="sxs-lookup"><span data-stu-id="2755f-112">0</span></span>     | <span data-ttu-id="2755f-113">团队的默认类型, 可提供标准团队体验。</span><span class="sxs-lookup"><span data-stu-id="2755f-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="2755f-114">educationStandard</span><span class="sxs-lookup"><span data-stu-id="2755f-114">educationStandard</span></span>  | <span data-ttu-id="2755f-115">1</span><span class="sxs-lookup"><span data-stu-id="2755f-115">1</span></span>     | <span data-ttu-id="2755f-116">由教育用户创建的团队。</span><span class="sxs-lookup"><span data-stu-id="2755f-116">Team created by an education user.</span></span> <span data-ttu-id="2755f-117">教育用户创建的所有团队都属于 Edu 类型。</span><span class="sxs-lookup"><span data-stu-id="2755f-117">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="2755f-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="2755f-118">educationClass</span></span>     | <span data-ttu-id="2755f-119">双面</span><span class="sxs-lookup"><span data-stu-id="2755f-119">2</span></span>     | <span data-ttu-id="2755f-120">针对某个类进行了优化的团队体验。</span><span class="sxs-lookup"><span data-stu-id="2755f-120">Team experience optimized for a class.</span></span> <span data-ttu-id="2755f-121">这样可以跨 O365 分段功能。</span><span class="sxs-lookup"><span data-stu-id="2755f-121">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="2755f-122">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="2755f-122">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="2755f-123">第三章</span><span class="sxs-lookup"><span data-stu-id="2755f-123">3</span></span> | <span data-ttu-id="2755f-124">为 PLC 优化的团队体验。</span><span class="sxs-lookup"><span data-stu-id="2755f-124">Team experience optimized for a PLC.</span></span> <span data-ttu-id="2755f-125">[在此处](https://en.wikipedia.org/wiki/Professional_learning_community)了解有关 PLC 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="2755f-125">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="2755f-126">educationStaff</span><span class="sxs-lookup"><span data-stu-id="2755f-126">educationStaff</span></span>     | <span data-ttu-id="2755f-127">4</span><span class="sxs-lookup"><span data-stu-id="2755f-127">4</span></span>     |  <span data-ttu-id="2755f-128">对于组织中员工的优化体验的团队类型, 员工主管 (如主体) 是管理员, 而教师是一个专门的笔记本提供的团队成员。</span><span class="sxs-lookup"><span data-stu-id="2755f-128">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="2755f-129">有关更多详细信息, 请参阅[OneNote 教职员工笔记本教育](https://www.onenote.com/staffnotebookedu)版。</span><span class="sxs-lookup"><span data-stu-id="2755f-129">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="2755f-130">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="2755f-130">unknownFutureValue</span></span> | <span data-ttu-id="2755f-131">步</span><span class="sxs-lookup"><span data-stu-id="2755f-131">7</span></span>     | <span data-ttu-id="2755f-132">将 Sentinel 值保留为占位符, 以便将来扩展枚举。</span><span class="sxs-lookup"><span data-stu-id="2755f-132">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
