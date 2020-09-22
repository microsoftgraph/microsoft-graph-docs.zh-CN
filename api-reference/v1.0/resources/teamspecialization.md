---
title: teamSpecialization 枚举类型
description: 描述团队的特殊用例。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: enumPageType
ms.openlocfilehash: ed104ee94468d8331ca0d1f172513337da1f0db9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48022846"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="14b63-103">teamSpecialization 枚举类型</span><span class="sxs-lookup"><span data-stu-id="14b63-103">teamSpecialization enum type</span></span>

<span data-ttu-id="14b63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="14b63-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="14b63-105">指示 [团队](../resources/team.md) 是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="14b63-105">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="14b63-106">每个 [团队](../resources/team.md) 特殊化都有权访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="14b63-106">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="14b63-107">默认值为 "无"。</span><span class="sxs-lookup"><span data-stu-id="14b63-107">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="14b63-108">成员</span><span class="sxs-lookup"><span data-stu-id="14b63-108">Members</span></span>

| <span data-ttu-id="14b63-109">成员</span><span class="sxs-lookup"><span data-stu-id="14b63-109">Member</span></span>             | <span data-ttu-id="14b63-110">值</span><span class="sxs-lookup"><span data-stu-id="14b63-110">Value</span></span> | <span data-ttu-id="14b63-111">说明</span><span class="sxs-lookup"><span data-stu-id="14b63-111">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="14b63-112">无</span><span class="sxs-lookup"><span data-stu-id="14b63-112">none</span></span>               | <span data-ttu-id="14b63-113">0</span><span class="sxs-lookup"><span data-stu-id="14b63-113">0</span></span>     | <span data-ttu-id="14b63-114">团队的默认类型，可提供标准团队体验。</span><span class="sxs-lookup"><span data-stu-id="14b63-114">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="14b63-115">educationStandard</span><span class="sxs-lookup"><span data-stu-id="14b63-115">educationStandard</span></span>  | <span data-ttu-id="14b63-116">1 </span><span class="sxs-lookup"><span data-stu-id="14b63-116">1</span></span>     | <span data-ttu-id="14b63-117">由教育用户创建的团队。</span><span class="sxs-lookup"><span data-stu-id="14b63-117">Team created by an education user.</span></span> <span data-ttu-id="14b63-118">教育用户创建的所有团队都属于 Edu 类型。</span><span class="sxs-lookup"><span data-stu-id="14b63-118">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="14b63-119">educationClass</span><span class="sxs-lookup"><span data-stu-id="14b63-119">educationClass</span></span>     | <span data-ttu-id="14b63-120">2 </span><span class="sxs-lookup"><span data-stu-id="14b63-120">2</span></span>     | <span data-ttu-id="14b63-121">针对某个类进行了优化的团队体验。</span><span class="sxs-lookup"><span data-stu-id="14b63-121">Team experience optimized for a class.</span></span> <span data-ttu-id="14b63-122">这样可以跨 O365 分段功能。</span><span class="sxs-lookup"><span data-stu-id="14b63-122">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="14b63-123">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="14b63-123">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="14b63-124">第三章</span><span class="sxs-lookup"><span data-stu-id="14b63-124">3</span></span> | <span data-ttu-id="14b63-125">为 PLC 优化的团队体验。</span><span class="sxs-lookup"><span data-stu-id="14b63-125">Team experience optimized for a PLC.</span></span> <span data-ttu-id="14b63-126">[在此处](https://en.wikipedia.org/wiki/Professional_learning_community)了解有关 PLC 的详细信息。</span><span class="sxs-lookup"><span data-stu-id="14b63-126">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="14b63-127">educationStaff</span><span class="sxs-lookup"><span data-stu-id="14b63-127">educationStaff</span></span>     | <span data-ttu-id="14b63-128">4 </span><span class="sxs-lookup"><span data-stu-id="14b63-128">4</span></span>     |  <span data-ttu-id="14b63-129">对于组织中员工的优化体验的团队类型，员工主管（如主体）是管理员，而教师是一个专门的笔记本提供的团队成员。</span><span class="sxs-lookup"><span data-stu-id="14b63-129">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="14b63-130">有关更多详细信息，请参阅 [OneNote 教职员工笔记本教育](https://www.onenote.com/staffnotebookedu)版。</span><span class="sxs-lookup"><span data-stu-id="14b63-130">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="14b63-131">向 unknownfuturevalue</span><span class="sxs-lookup"><span data-stu-id="14b63-131">unknownFutureValue</span></span> | <span data-ttu-id="14b63-132">7 </span><span class="sxs-lookup"><span data-stu-id="14b63-132">7</span></span>     | <span data-ttu-id="14b63-133">将 Sentinel 值保留为占位符，以便将来扩展枚举。</span><span class="sxs-lookup"><span data-stu-id="14b63-133">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |

