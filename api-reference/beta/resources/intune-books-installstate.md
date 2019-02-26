---
title: installState 枚举类型
description: 安装状态的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0554df30b4d7165c0164749730e2584af6cc35fd
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158210"
---
# <a name="installstate-enum-type"></a><span data-ttu-id="89472-103">installState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89472-103">installState enum type</span></span>

> <span data-ttu-id="89472-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89472-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89472-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89472-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89472-106">安装状态的可能值。</span><span class="sxs-lookup"><span data-stu-id="89472-106">Possible values for install state.</span></span>

## <a name="members"></a><span data-ttu-id="89472-107">成员</span><span class="sxs-lookup"><span data-stu-id="89472-107">Members</span></span>
|<span data-ttu-id="89472-108">成员</span><span class="sxs-lookup"><span data-stu-id="89472-108">Member</span></span>|<span data-ttu-id="89472-109">值</span><span class="sxs-lookup"><span data-stu-id="89472-109">Value</span></span>|<span data-ttu-id="89472-110">说明</span><span class="sxs-lookup"><span data-stu-id="89472-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89472-111">notApplicable</span><span class="sxs-lookup"><span data-stu-id="89472-111">notApplicable</span></span>|<span data-ttu-id="89472-112">0</span><span class="sxs-lookup"><span data-stu-id="89472-112">0</span></span>|<span data-ttu-id="89472-113">不适用。</span><span class="sxs-lookup"><span data-stu-id="89472-113">Not Applicable.</span></span>|
|<span data-ttu-id="89472-114">了</span><span class="sxs-lookup"><span data-stu-id="89472-114">installed</span></span>|<span data-ttu-id="89472-115">1</span><span class="sxs-lookup"><span data-stu-id="89472-115">1</span></span>|<span data-ttu-id="89472-116">了.</span><span class="sxs-lookup"><span data-stu-id="89472-116">Installed.</span></span>|
|<span data-ttu-id="89472-117">failed</span><span class="sxs-lookup"><span data-stu-id="89472-117">failed</span></span>|<span data-ttu-id="89472-118">双面</span><span class="sxs-lookup"><span data-stu-id="89472-118">2</span></span>|<span data-ttu-id="89472-119">未能.</span><span class="sxs-lookup"><span data-stu-id="89472-119">Failed.</span></span>|
|<span data-ttu-id="89472-120">notInstalled</span><span class="sxs-lookup"><span data-stu-id="89472-120">notInstalled</span></span>|<span data-ttu-id="89472-121">第三章</span><span class="sxs-lookup"><span data-stu-id="89472-121">3</span></span>|<span data-ttu-id="89472-122">未安装。</span><span class="sxs-lookup"><span data-stu-id="89472-122">Not Installed.</span></span>|
|<span data-ttu-id="89472-123">uninstallFailed</span><span class="sxs-lookup"><span data-stu-id="89472-123">uninstallFailed</span></span>|<span data-ttu-id="89472-124">4</span><span class="sxs-lookup"><span data-stu-id="89472-124">4</span></span>|<span data-ttu-id="89472-125">卸载失败。</span><span class="sxs-lookup"><span data-stu-id="89472-125">Uninstall Failed.</span></span>|
|<span data-ttu-id="89472-126">unknown</span><span class="sxs-lookup"><span data-stu-id="89472-126">unknown</span></span>|<span data-ttu-id="89472-127">5</span><span class="sxs-lookup"><span data-stu-id="89472-127">5</span></span>|<span data-ttu-id="89472-128">陌生.</span><span class="sxs-lookup"><span data-stu-id="89472-128">Unknown.</span></span>|




