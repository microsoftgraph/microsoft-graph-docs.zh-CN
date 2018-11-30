---
title: 成员
description: 介绍 teamsApp 的当前安装状态。
ms.openlocfilehash: 7f358a621a25219e78e3a02ce081d07a27395d2c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047336"
---
#<a name="teamsappinstalledstate-enum-type"></a><span data-ttu-id="0b4bb-103">teamsAppInstalledState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0b4bb-103">teamsAppInstalledState enum type</span></span>

> <span data-ttu-id="0b4bb-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0b4bb-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0b4bb-106">介绍[teamsApp](teamsapp.md)的当前安装状态。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-106">Describes the current installation status of a [teamsApp](teamsapp.md).</span></span>

## <a name="members"></a><span data-ttu-id="0b4bb-107">成员</span><span class="sxs-lookup"><span data-stu-id="0b4bb-107">Members</span></span>

| <span data-ttu-id="0b4bb-108">成员</span><span class="sxs-lookup"><span data-stu-id="0b4bb-108">Member</span></span> | <span data-ttu-id="0b4bb-109">值</span><span class="sxs-lookup"><span data-stu-id="0b4bb-109">Value</span></span>| <span data-ttu-id="0b4bb-110">说明</span><span class="sxs-lookup"><span data-stu-id="0b4bb-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="0b4bb-111">notInstalled</span><span class="sxs-lookup"><span data-stu-id="0b4bb-111">notInstalled</span></span>|<span data-ttu-id="0b4bb-112">0</span><span class="sxs-lookup"><span data-stu-id="0b4bb-112">0</span></span>|<span data-ttu-id="0b4bb-113">应用程序并不安装到团队。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-113">App is not installed to team.</span></span>|
|<span data-ttu-id="0b4bb-114">安装</span><span class="sxs-lookup"><span data-stu-id="0b4bb-114">installed</span></span>|<span data-ttu-id="0b4bb-115">1</span><span class="sxs-lookup"><span data-stu-id="0b4bb-115">1</span></span>|<span data-ttu-id="0b4bb-116">通常安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-116">App is installed normally.</span></span>|
|<span data-ttu-id="0b4bb-117">installedAndHidden</span><span class="sxs-lookup"><span data-stu-id="0b4bb-117">installedAndHidden</span></span>|<span data-ttu-id="0b4bb-118">2</span><span class="sxs-lookup"><span data-stu-id="0b4bb-118">2</span></span>|<span data-ttu-id="0b4bb-119">应用程序是安装，但从视图中隐藏。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-119">App is installed but hidden from view.</span></span>|
|<span data-ttu-id="0b4bb-120">installedAndPermanent</span><span class="sxs-lookup"><span data-stu-id="0b4bb-120">installedAndPermanent</span></span>|<span data-ttu-id="0b4bb-121">3</span><span class="sxs-lookup"><span data-stu-id="0b4bb-121">3</span></span>|<span data-ttu-id="0b4bb-122">应用程序永久安装，并且不会删除。</span><span class="sxs-lookup"><span data-stu-id="0b4bb-122">App is permanently installed and may not be removed.</span></span>|
