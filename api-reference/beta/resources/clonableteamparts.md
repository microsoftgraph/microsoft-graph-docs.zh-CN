---
title: clonableTeamParts 枚举类型
description: '描述应克隆的工作组的一部分。 '
localization_priority: Normal
ms.openlocfilehash: 3169d6e367484248e581c12c38887e07cf5c95af
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511462"
---
# <a name="clonableteamparts-enum-type"></a><span data-ttu-id="f366c-103">clonableTeamParts 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f366c-103">clonableTeamParts enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f366c-104">描述应克隆的[工作组](../resources/team.md)的一部分。</span><span class="sxs-lookup"><span data-stu-id="f366c-104">Describes which part of a [team](../resources/team.md) should be cloned.</span></span> 

## <a name="members"></a><span data-ttu-id="f366c-105">成员</span><span class="sxs-lookup"><span data-stu-id="f366c-105">Members</span></span>

| <span data-ttu-id="f366c-106">成员</span><span class="sxs-lookup"><span data-stu-id="f366c-106">Member</span></span> | <span data-ttu-id="f366c-107">值</span><span class="sxs-lookup"><span data-stu-id="f366c-107">Value</span></span>| <span data-ttu-id="f366c-108">说明</span><span class="sxs-lookup"><span data-stu-id="f366c-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f366c-109">apps</span><span class="sxs-lookup"><span data-stu-id="f366c-109">apps</span></span>|<span data-ttu-id="f366c-110">$1</span><span class="sxs-lookup"><span data-stu-id="f366c-110">1</span></span>|<span data-ttu-id="f366c-111">将复制已安装的应用程序的列表。</span><span class="sxs-lookup"><span data-stu-id="f366c-111">Copy the list of installed apps.</span></span>|
|<span data-ttu-id="f366c-112">标签</span><span class="sxs-lookup"><span data-stu-id="f366c-112">tabs</span></span>|<span data-ttu-id="f366c-113">-2</span><span class="sxs-lookup"><span data-stu-id="f366c-113">2</span></span>|<span data-ttu-id="f366c-114">将复制通道中的选项卡。</span><span class="sxs-lookup"><span data-stu-id="f366c-114">copies the tabs within channels.</span></span>|
|<span data-ttu-id="f366c-115">settings</span><span class="sxs-lookup"><span data-stu-id="f366c-115">settings</span></span>|<span data-ttu-id="f366c-116">-4</span><span class="sxs-lookup"><span data-stu-id="f366c-116">4</span></span>|<span data-ttu-id="f366c-117">将复制的团队，以及关键组设置中的所有设置。</span><span class="sxs-lookup"><span data-stu-id="f366c-117">Copies all settings within the team, along with key group settings.</span></span>|
|<span data-ttu-id="f366c-118">channels</span><span class="sxs-lookup"><span data-stu-id="f366c-118">channels</span></span>|<span data-ttu-id="f366c-119">-8</span><span class="sxs-lookup"><span data-stu-id="f366c-119">8</span></span>|<span data-ttu-id="f366c-120">将复制的通道结构 （但不是在进入频道的消息）。</span><span class="sxs-lookup"><span data-stu-id="f366c-120">copies the channel structure (but not the messages in the channel).</span></span>|
|<span data-ttu-id="f366c-121">members</span><span class="sxs-lookup"><span data-stu-id="f366c-121">members</span></span>|<span data-ttu-id="f366c-122">1.6</span><span class="sxs-lookup"><span data-stu-id="f366c-122">16</span></span>|<span data-ttu-id="f366c-123">将复制的成员和所有者的团队。</span><span class="sxs-lookup"><span data-stu-id="f366c-123">copies the members and owners of the team.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/clonableteamparts.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
