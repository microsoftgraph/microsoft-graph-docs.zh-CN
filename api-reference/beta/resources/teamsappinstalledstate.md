---
title: Members
description: 介绍 teamsApp 的当前安装状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 82e46faccd2a91a82ba4fb7352391f58a42c33a9
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517272"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="c499c-103">teamsAppInstalledState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c499c-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c499c-104">介绍[teamsApp](teamsapp.md)的当前安装状态。</span><span class="sxs-lookup"><span data-stu-id="c499c-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="c499c-105">成员</span><span class="sxs-lookup"><span data-stu-id="c499c-105">Members</span></span>

| <span data-ttu-id="c499c-106">成员</span><span class="sxs-lookup"><span data-stu-id="c499c-106">Member</span></span> | <span data-ttu-id="c499c-107">值</span><span class="sxs-lookup"><span data-stu-id="c499c-107">Value</span></span>| <span data-ttu-id="c499c-108">说明</span><span class="sxs-lookup"><span data-stu-id="c499c-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c499c-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="c499c-109">notInstalled</span></span>|<span data-ttu-id="c499c-110">0%</span><span class="sxs-lookup"><span data-stu-id="c499c-110">0</span></span>|<span data-ttu-id="c499c-111">应用程序并不安装到团队。</span><span class="sxs-lookup"><span data-stu-id="c499c-111">App is not installed to team.</span></span>|
|<span data-ttu-id="c499c-112">Installed</span><span class="sxs-lookup"><span data-stu-id="c499c-112">installed</span></span>|<span data-ttu-id="c499c-113">$1</span><span class="sxs-lookup"><span data-stu-id="c499c-113">1</span></span>|<span data-ttu-id="c499c-114">通常安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="c499c-114">App is installed normally.</span></span>|
|<span data-ttu-id="c499c-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="c499c-115">installedAndHidden</span></span>|<span data-ttu-id="c499c-116">-2</span><span class="sxs-lookup"><span data-stu-id="c499c-116">2</span></span>|<span data-ttu-id="c499c-117">应用程序是安装，但从视图中隐藏。</span><span class="sxs-lookup"><span data-stu-id="c499c-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="c499c-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="c499c-118">installedAndPermanent</span></span>|<span data-ttu-id="c499c-119">-3</span><span class="sxs-lookup"><span data-stu-id="c499c-119">3</span></span>|<span data-ttu-id="c499c-120">应用程序永久安装，并且不会删除。</span><span class="sxs-lookup"><span data-stu-id="c499c-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
