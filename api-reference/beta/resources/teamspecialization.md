---
title: teamSpecialization 枚举类型
description: 描述为团队的特殊的使用情况。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 9e19c6b2242256f0d1b7a23c89aa07787bfc1913
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522649"
---
# <a name="teamspecialization-enum-type"></a><span data-ttu-id="357b9-103">teamSpecialization 枚举类型</span><span class="sxs-lookup"><span data-stu-id="357b9-103">teamSpecialization enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="357b9-104">指示团队是否适用于特定用例。</span><span class="sxs-lookup"><span data-stu-id="357b9-104">Indicates whether the [team](../resources/team.md) is intended for a particular use case.</span></span> <span data-ttu-id="357b9-105">每个团队专用化都可以访问针对其用例的独特行为和体验。</span><span class="sxs-lookup"><span data-stu-id="357b9-105">Each [team](../resources/team.md) specialization has access to unique behaviors and experiences targeted to its use case.</span></span> <span data-ttu-id="357b9-106">默认值为无。</span><span class="sxs-lookup"><span data-stu-id="357b9-106">Default is 'none'.</span></span>

## <a name="members"></a><span data-ttu-id="357b9-107">成员</span><span class="sxs-lookup"><span data-stu-id="357b9-107">Members</span></span>

| <span data-ttu-id="357b9-108">成员</span><span class="sxs-lookup"><span data-stu-id="357b9-108">Member</span></span>             | <span data-ttu-id="357b9-109">值</span><span class="sxs-lookup"><span data-stu-id="357b9-109">Value</span></span> | <span data-ttu-id="357b9-110">说明</span><span class="sxs-lookup"><span data-stu-id="357b9-110">Description</span></span>                                                                |
| :----------------- | :---- | :------------------------------------------------------------------------- |
| <span data-ttu-id="357b9-111">无</span><span class="sxs-lookup"><span data-stu-id="357b9-111">none</span></span>               | <span data-ttu-id="357b9-112">0%</span><span class="sxs-lookup"><span data-stu-id="357b9-112">0</span></span>     | <span data-ttu-id="357b9-113">默认为团队通过该组件的标准团队体验的类型。</span><span class="sxs-lookup"><span data-stu-id="357b9-113">Default type for a team which gives the standard team experience.</span></span>          |
| <span data-ttu-id="357b9-114">unknownFutureValue</span><span class="sxs-lookup"><span data-stu-id="357b9-114">unknownFutureValue</span></span> | <span data-ttu-id="357b9-115">-7</span><span class="sxs-lookup"><span data-stu-id="357b9-115">7</span></span>     | <span data-ttu-id="357b9-116">Sentinel 保留作为以供将来扩展枚举的占位符值。</span><span class="sxs-lookup"><span data-stu-id="357b9-116">Sentinel value reserved as a placeholder for future expansion of the enum.</span></span> |
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamspecialization.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
