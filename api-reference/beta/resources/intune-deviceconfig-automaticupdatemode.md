---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9af00bda442c1a152820323fc0b7e1ddfcd8c384
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31791479"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="23ab8-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="23ab8-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="23ab8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="23ab8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="23ab8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="23ab8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="23ab8-106">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="23ab8-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="23ab8-107">成员</span><span class="sxs-lookup"><span data-stu-id="23ab8-107">Members</span></span>
|<span data-ttu-id="23ab8-108">成员</span><span class="sxs-lookup"><span data-stu-id="23ab8-108">Member</span></span>|<span data-ttu-id="23ab8-109">值</span><span class="sxs-lookup"><span data-stu-id="23ab8-109">Value</span></span>|<span data-ttu-id="23ab8-110">说明</span><span class="sxs-lookup"><span data-stu-id="23ab8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23ab8-111">定制</span><span class="sxs-lookup"><span data-stu-id="23ab8-111">userDefined</span></span>|<span data-ttu-id="23ab8-112">0</span><span class="sxs-lookup"><span data-stu-id="23ab8-112">0</span></span>|<span data-ttu-id="23ab8-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="23ab8-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="23ab8-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="23ab8-114">notifyDownload</span></span>|<span data-ttu-id="23ab8-115">1</span><span class="sxs-lookup"><span data-stu-id="23ab8-115">1</span></span>|<span data-ttu-id="23ab8-116">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="23ab8-116">Notify on download.</span></span>|
|<span data-ttu-id="23ab8-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="23ab8-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="23ab8-118">双面</span><span class="sxs-lookup"><span data-stu-id="23ab8-118">2</span></span>|<span data-ttu-id="23ab8-119">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="23ab8-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="23ab8-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="23ab8-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="23ab8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="23ab8-121">3</span></span>|<span data-ttu-id="23ab8-122">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="23ab8-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="23ab8-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="23ab8-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="23ab8-124">4</span><span class="sxs-lookup"><span data-stu-id="23ab8-124">4</span></span>|<span data-ttu-id="23ab8-125">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="23ab8-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="23ab8-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="23ab8-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="23ab8-127">5</span><span class="sxs-lookup"><span data-stu-id="23ab8-127">5</span></span>|<span data-ttu-id="23ab8-128">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="23ab8-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="23ab8-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="23ab8-129">windowsDefault</span></span>|<span data-ttu-id="23ab8-130">型</span><span class="sxs-lookup"><span data-stu-id="23ab8-130">6</span></span>|<span data-ttu-id="23ab8-131">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="23ab8-131">Reset to Windows default value.</span></span>|





