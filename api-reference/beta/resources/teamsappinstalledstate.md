---
title: Members
description: 介绍 teamsApp 的当前安装状态。
author: nkramer
ms.openlocfilehash: a73c68298c4cdf65deee68fb3bd707d50bc2475a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316791"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="c67b1-103">teamsAppInstalledState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c67b1-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="c67b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c67b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c67b1-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c67b1-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c67b1-106">介绍[teamsApp](teamsapp.md)的当前安装状态。</span><span class="sxs-lookup"><span data-stu-id="c67b1-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="c67b1-107">成员</span><span class="sxs-lookup"><span data-stu-id="c67b1-107">Members</span></span>

| <span data-ttu-id="c67b1-108">成员</span><span class="sxs-lookup"><span data-stu-id="c67b1-108">Member</span></span> | <span data-ttu-id="c67b1-109">值</span><span class="sxs-lookup"><span data-stu-id="c67b1-109">Value</span></span>| <span data-ttu-id="c67b1-110">说明</span><span class="sxs-lookup"><span data-stu-id="c67b1-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="c67b1-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="c67b1-111">notInstalled</span></span>|<span data-ttu-id="c67b1-112">0</span><span class="sxs-lookup"><span data-stu-id="c67b1-112">0</span></span>|<span data-ttu-id="c67b1-113">应用程序并不安装到团队。</span><span class="sxs-lookup"><span data-stu-id="c67b1-113">App is not installed to team.</span></span>|
|<span data-ttu-id="c67b1-114">安装</span><span class="sxs-lookup"><span data-stu-id="c67b1-114">installed</span></span>|<span data-ttu-id="c67b1-115">1</span><span class="sxs-lookup"><span data-stu-id="c67b1-115">1</span></span>|<span data-ttu-id="c67b1-116">通常安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="c67b1-116">App is installed normally.</span></span>|
|<span data-ttu-id="c67b1-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="c67b1-117">installedAndHidden</span></span>|<span data-ttu-id="c67b1-118">2</span><span class="sxs-lookup"><span data-stu-id="c67b1-118">2</span></span>|<span data-ttu-id="c67b1-119">应用程序是安装，但从视图中隐藏。</span><span class="sxs-lookup"><span data-stu-id="c67b1-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="c67b1-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="c67b1-120">installedAndPermanent</span></span>|<span data-ttu-id="c67b1-121">3</span><span class="sxs-lookup"><span data-stu-id="c67b1-121">3</span></span>|<span data-ttu-id="c67b1-122">应用程序永久安装，并且不会删除。</span><span class="sxs-lookup"><span data-stu-id="c67b1-122">App is permanently installed and may not be removed.</span></span>|
