---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 280cdcf50e19736077a10668a7cfc507aca9412e
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947545"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="af234-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="af234-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="af234-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="af234-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="af234-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="af234-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="af234-106">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="af234-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="af234-107">成员</span><span class="sxs-lookup"><span data-stu-id="af234-107">Members</span></span>
|<span data-ttu-id="af234-108">成员</span><span class="sxs-lookup"><span data-stu-id="af234-108">Member</span></span>|<span data-ttu-id="af234-109">值</span><span class="sxs-lookup"><span data-stu-id="af234-109">Value</span></span>|<span data-ttu-id="af234-110">说明</span><span class="sxs-lookup"><span data-stu-id="af234-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="af234-111">定制</span><span class="sxs-lookup"><span data-stu-id="af234-111">userDefined</span></span>|<span data-ttu-id="af234-112">0</span><span class="sxs-lookup"><span data-stu-id="af234-112">0</span></span>|<span data-ttu-id="af234-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="af234-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="af234-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="af234-114">notifyDownload</span></span>|<span data-ttu-id="af234-115">1</span><span class="sxs-lookup"><span data-stu-id="af234-115">1</span></span>|<span data-ttu-id="af234-116">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="af234-116">Notify on download.</span></span>|
|<span data-ttu-id="af234-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="af234-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="af234-118">双面</span><span class="sxs-lookup"><span data-stu-id="af234-118">2</span></span>|<span data-ttu-id="af234-119">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="af234-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="af234-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="af234-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="af234-121">第三章</span><span class="sxs-lookup"><span data-stu-id="af234-121">3</span></span>|<span data-ttu-id="af234-122">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="af234-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="af234-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="af234-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="af234-124">4</span><span class="sxs-lookup"><span data-stu-id="af234-124">4</span></span>|<span data-ttu-id="af234-125">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="af234-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="af234-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="af234-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="af234-127">5</span><span class="sxs-lookup"><span data-stu-id="af234-127">5</span></span>|<span data-ttu-id="af234-128">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="af234-128">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="af234-129">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="af234-129">windowsDefault</span></span>|<span data-ttu-id="af234-130">型</span><span class="sxs-lookup"><span data-stu-id="af234-130">6</span></span>|<span data-ttu-id="af234-131">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="af234-131">Reset to Windows default value.</span></span>|




