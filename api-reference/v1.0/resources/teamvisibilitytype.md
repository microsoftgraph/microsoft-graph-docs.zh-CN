---
title: 成员
description: '介绍团队的可见性。 '
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: ea8868924681d3e8f8cd0b4f55ff947c085260e0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456964"
---
# <a name="teamvisibilitytype-enum-type"></a><span data-ttu-id="514c7-103">teamVisibilityType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="514c7-103">teamVisibilityType enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="514c7-104">介绍[团队](../resources/team.md)的可见性。</span><span class="sxs-lookup"><span data-stu-id="514c7-104">Describes the visibility of a [team](../resources/team.md).</span></span> 

## <a name="members"></a><span data-ttu-id="514c7-105">成员</span><span class="sxs-lookup"><span data-stu-id="514c7-105">Members</span></span>

| <span data-ttu-id="514c7-106">成员</span><span class="sxs-lookup"><span data-stu-id="514c7-106">Member</span></span> | <span data-ttu-id="514c7-107">值</span><span class="sxs-lookup"><span data-stu-id="514c7-107">Value</span></span>| <span data-ttu-id="514c7-108">说明</span><span class="sxs-lookup"><span data-stu-id="514c7-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="514c7-109">private</span><span class="sxs-lookup"><span data-stu-id="514c7-109">private</span></span>|<span data-ttu-id="514c7-110">0</span><span class="sxs-lookup"><span data-stu-id="514c7-110">0</span></span>|<span data-ttu-id="514c7-111">任何人都可以看到团队, 但只有所有者可以向团队添加用户。</span><span class="sxs-lookup"><span data-stu-id="514c7-111">Anyone can see the team but only the owner can add a user to the team.</span></span>|
|<span data-ttu-id="514c7-112">公开</span><span class="sxs-lookup"><span data-stu-id="514c7-112">public</span></span>|<span data-ttu-id="514c7-113">1</span><span class="sxs-lookup"><span data-stu-id="514c7-113">1</span></span>|<span data-ttu-id="514c7-114">任何人都可以加入团队。</span><span class="sxs-lookup"><span data-stu-id="514c7-114">Anyone can join the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamvisibilitytype.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
