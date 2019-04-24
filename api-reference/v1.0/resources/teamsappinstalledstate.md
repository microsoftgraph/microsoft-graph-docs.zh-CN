---
title: 成员
description: 描述 teamsApp 的当前安装状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: a58a0d046ef9c42f197e841ab542bf8dcb5f96f5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462247"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="8986a-103">teamsAppInstalledState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8986a-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8986a-104">描述[teamsApp](teamsapp.md)的当前安装状态。</span><span class="sxs-lookup"><span data-stu-id="8986a-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="8986a-105">成员</span><span class="sxs-lookup"><span data-stu-id="8986a-105">Members</span></span>

| <span data-ttu-id="8986a-106">成员</span><span class="sxs-lookup"><span data-stu-id="8986a-106">Member</span></span> | <span data-ttu-id="8986a-107">值</span><span class="sxs-lookup"><span data-stu-id="8986a-107">Value</span></span>| <span data-ttu-id="8986a-108">说明</span><span class="sxs-lookup"><span data-stu-id="8986a-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="8986a-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="8986a-109">notInstalled</span></span>|<span data-ttu-id="8986a-110">0</span><span class="sxs-lookup"><span data-stu-id="8986a-110">0</span></span>|<span data-ttu-id="8986a-111">未将应用安装到团队。</span><span class="sxs-lookup"><span data-stu-id="8986a-111">App is not installed to team.</span></span>|
|<span data-ttu-id="8986a-112">了</span><span class="sxs-lookup"><span data-stu-id="8986a-112">installed</span></span>|<span data-ttu-id="8986a-113">1</span><span class="sxs-lookup"><span data-stu-id="8986a-113">1</span></span>|<span data-ttu-id="8986a-114">应用程序以正常方式安装。</span><span class="sxs-lookup"><span data-stu-id="8986a-114">App is installed normally.</span></span>|
|<span data-ttu-id="8986a-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="8986a-115">installedAndHidden</span></span>|<span data-ttu-id="8986a-116">2 </span><span class="sxs-lookup"><span data-stu-id="8986a-116">2</span></span>|<span data-ttu-id="8986a-117">已安装应用程序, 但已在视图中隐藏。</span><span class="sxs-lookup"><span data-stu-id="8986a-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="8986a-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="8986a-118">installedAndPermanent</span></span>|<span data-ttu-id="8986a-119">3 </span><span class="sxs-lookup"><span data-stu-id="8986a-119">3</span></span>|<span data-ttu-id="8986a-120">应用程序永久安装且不可能删除。</span><span class="sxs-lookup"><span data-stu-id="8986a-120">App is permanently installed and may not be removed.</span></span>|
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/teamsappinstalledstate.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
