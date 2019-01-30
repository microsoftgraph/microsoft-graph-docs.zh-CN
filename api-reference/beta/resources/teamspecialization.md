---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: c89f3ef993e55e28f5558f99c3ef87ad5174bc65
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/30/2019
ms.locfileid: "29640320"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="26e1a-103">teamSpecialization 枚举类型</span><span class="sxs-lookup"><span data-stu-id="26e1a-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="26e1a-104">指示是否[团队](../resources/team.md)适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="26e1a-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="26e1a-105">每个[团队](../resources/team.md)具专业性有权访问唯一行为和针对其用例的体验。</span><span class="sxs-lookup"><span data-stu-id="26e1a-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="26e1a-106">默认值为无。</span><span class="sxs-lookup"><span data-stu-id="26e1a-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="26e1a-107">成员</span><span class="sxs-lookup"><span data-stu-id="26e1a-107">Members</span></span>

| <span data-ttu-id="26e1a-108">成员</span><span class="sxs-lookup"><span data-stu-id="26e1a-108">Member</span></span>             | <span data-ttu-id="26e1a-109">值</span><span class="sxs-lookup"><span data-stu-id="26e1a-109">Value</span></span> | <span data-ttu-id="26e1a-110">说明</span><span class="sxs-lookup"><span data-stu-id="26e1a-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="26e1a-111">无</span><span class="sxs-lookup"><span data-stu-id="26e1a-111">none</span></span>               | <span data-ttu-id="26e1a-112">0</span><span class="sxs-lookup"><span data-stu-id="26e1a-112">0</span></span>     | <span data-ttu-id="26e1a-113">默认为团队通过该组件的标准团队体验的类型。</span><span class="sxs-lookup"><span data-stu-id="26e1a-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="26e1a-114">educationStandard</span><span class="sxs-lookup"><span data-stu-id="26e1a-114">educationStandard</span></span>  | <span data-ttu-id="26e1a-115">1</span><span class="sxs-lookup"><span data-stu-id="26e1a-115">1</span></span>     | <span data-ttu-id="26e1a-116">培训用户创建的团队。</span><span class="sxs-lookup"><span data-stu-id="26e1a-116">Team created by an education user.</span></span> <span data-ttu-id="26e1a-117">培训用户创建的所有团队都是类型 Edu。</span><span class="sxs-lookup"><span data-stu-id="26e1a-117">All teams created by education user are of type Edu.</span></span> |
| <span data-ttu-id="26e1a-118">educationClass</span><span class="sxs-lookup"><span data-stu-id="26e1a-118">educationClass</span></span>     | <span data-ttu-id="26e1a-119">2</span><span class="sxs-lookup"><span data-stu-id="26e1a-119">2</span></span>     | <span data-ttu-id="26e1a-120">团队优化类的体验。</span><span class="sxs-lookup"><span data-stu-id="26e1a-120">Team experience optimized for a class.</span></span> <span data-ttu-id="26e1a-121">这样跨 O365 细分的功能。</span><span class="sxs-lookup"><span data-stu-id="26e1a-121">This enables segmentation of features across O365.</span></span> |
| <span data-ttu-id="26e1a-122">educationProfessionalLearningCommunity</span><span class="sxs-lookup"><span data-stu-id="26e1a-122">educationProfessionalLearningCommunity</span></span> | <span data-ttu-id="26e1a-123">3</span><span class="sxs-lookup"><span data-stu-id="26e1a-123">3</span></span> | <span data-ttu-id="26e1a-124">针对 PLC 优化工作组体验。</span><span class="sxs-lookup"><span data-stu-id="26e1a-124">Team experience optimized for a PLC.</span></span> <span data-ttu-id="26e1a-125">了解有关 PLC[此处](https://en.wikipedia.org/wiki/Professional_learning_community)。</span><span class="sxs-lookup"><span data-stu-id="26e1a-125">Learn more about PLC [here](https://en.wikipedia.org/wiki/Professional_learning_community).</span></span> |
| <span data-ttu-id="26e1a-126">educationStaff</span><span class="sxs-lookup"><span data-stu-id="26e1a-126">educationStaff</span></span>     | <span data-ttu-id="26e1a-127">4</span><span class="sxs-lookup"><span data-stu-id="26e1a-127">4</span></span>     |  <span data-ttu-id="26e1a-128">为了优化的员工在组织中，员工主持人，如主体，其中是管理员，教师体验团队类型是附带专用笔记本团队中的成员。</span><span class="sxs-lookup"><span data-stu-id="26e1a-128">Team type for an optimized experience for staff in an organization, where a staff leader, like a principal, is the admin and teachers are members in a team that comes with a specialized notebook.</span></span> <span data-ttu-id="26e1a-129">有关详细信息，请参阅[面向教育机构的 OneNote 员工笔记本](https://www.onenote.com/staffnotebookedu)。</span><span class="sxs-lookup"><span data-stu-id="26e1a-129">For more details, see [OneNote staff notebook for education](https://www.onenote.com/staffnotebookedu).</span></span> |
| <span data-ttu-id="26e1a-130">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="26e1a-130">unknownFutureValue</span></span> | <span data-ttu-id="26e1a-131">7</span><span class="sxs-lookup"><span data-stu-id="26e1a-131">7</span></span>     | <span data-ttu-id="26e1a-132">Sentinel 保留作为以供将来扩展枚举的占位符值。</span><span class="sxs-lookup"><span data-stu-id="26e1a-132">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!-- {
  "type": "#page.annotation",
  "suppressions": [
    "Error:{/api-reference/beta/resources/teamspecialization.md}:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
}-->
