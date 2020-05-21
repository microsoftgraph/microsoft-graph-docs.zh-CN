---
title: Members
description: 描述 teamsApp 的当前安装状态。
author: nkramer
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: c157d4acc074aacc1025b15902491197d0563106
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44335892"
---
# <a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="da82a-103">teamsAppInstalledState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="da82a-103">teamsAppInstalledState enum type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="da82a-104">描述[teamsApp](teamsapp.md)的当前安装状态。</span><span class="sxs-lookup"><span data-stu-id="da82a-104">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="da82a-105">成员</span><span class="sxs-lookup"><span data-stu-id="da82a-105">Members</span></span>

| <span data-ttu-id="da82a-106">成员</span><span class="sxs-lookup"><span data-stu-id="da82a-106">Member</span></span> | <span data-ttu-id="da82a-107">值</span><span class="sxs-lookup"><span data-stu-id="da82a-107">Value</span></span>| <span data-ttu-id="da82a-108">Description</span><span class="sxs-lookup"><span data-stu-id="da82a-108">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="da82a-109">notInstalled</span><span class="sxs-lookup"><span data-stu-id="da82a-109">notInstalled</span></span>|<span data-ttu-id="da82a-110">0</span><span class="sxs-lookup"><span data-stu-id="da82a-110">0</span></span>|<span data-ttu-id="da82a-111">未将应用安装到团队。</span><span class="sxs-lookup"><span data-stu-id="da82a-111">App is not installed to team.</span></span>|
|<span data-ttu-id="da82a-112">了</span><span class="sxs-lookup"><span data-stu-id="da82a-112">installed</span></span>|<span data-ttu-id="da82a-113">1 </span><span class="sxs-lookup"><span data-stu-id="da82a-113">1</span></span>|<span data-ttu-id="da82a-114">应用程序以正常方式安装。</span><span class="sxs-lookup"><span data-stu-id="da82a-114">App is installed normally.</span></span>|
|<span data-ttu-id="da82a-115">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="da82a-115">installedAndHidden</span></span>|<span data-ttu-id="da82a-116">2 </span><span class="sxs-lookup"><span data-stu-id="da82a-116">2</span></span>|<span data-ttu-id="da82a-117">已安装应用程序，但已在视图中隐藏。</span><span class="sxs-lookup"><span data-stu-id="da82a-117">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="da82a-118">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="da82a-118">installedAndPermanent</span></span>|<span data-ttu-id="da82a-119">第三章</span><span class="sxs-lookup"><span data-stu-id="da82a-119">3</span></span>|<span data-ttu-id="da82a-120">应用程序永久安装且不可能删除。</span><span class="sxs-lookup"><span data-stu-id="da82a-120">App is permanently installed and may not be removed.</span></span>|
