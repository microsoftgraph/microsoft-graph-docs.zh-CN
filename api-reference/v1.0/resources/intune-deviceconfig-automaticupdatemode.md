---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7fd45ff85cbab934aa2549f13ee3e6671c65f9ae
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30251375"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="f55e2-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f55e2-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="f55e2-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f55e2-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f55e2-105">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="f55e2-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="f55e2-106">成员</span><span class="sxs-lookup"><span data-stu-id="f55e2-106">Members</span></span>
|<span data-ttu-id="f55e2-107">成员</span><span class="sxs-lookup"><span data-stu-id="f55e2-107">Member</span></span>|<span data-ttu-id="f55e2-108">值</span><span class="sxs-lookup"><span data-stu-id="f55e2-108">Value</span></span>|<span data-ttu-id="f55e2-109">说明</span><span class="sxs-lookup"><span data-stu-id="f55e2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f55e2-110">定制</span><span class="sxs-lookup"><span data-stu-id="f55e2-110">userDefined</span></span>|<span data-ttu-id="f55e2-111">0</span><span class="sxs-lookup"><span data-stu-id="f55e2-111">0</span></span>|<span data-ttu-id="f55e2-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f55e2-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f55e2-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="f55e2-113">notifyDownload</span></span>|<span data-ttu-id="f55e2-114">1</span><span class="sxs-lookup"><span data-stu-id="f55e2-114">1</span></span>|<span data-ttu-id="f55e2-115">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="f55e2-115">Notify on download.</span></span>|
|<span data-ttu-id="f55e2-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f55e2-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="f55e2-117">双面</span><span class="sxs-lookup"><span data-stu-id="f55e2-117">2</span></span>|<span data-ttu-id="f55e2-118">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="f55e2-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="f55e2-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f55e2-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="f55e2-120">第三章</span><span class="sxs-lookup"><span data-stu-id="f55e2-120">3</span></span>|<span data-ttu-id="f55e2-121">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="f55e2-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="f55e2-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="f55e2-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="f55e2-123">4</span><span class="sxs-lookup"><span data-stu-id="f55e2-123">4</span></span>|<span data-ttu-id="f55e2-124">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="f55e2-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="f55e2-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="f55e2-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="f55e2-126">5</span><span class="sxs-lookup"><span data-stu-id="f55e2-126">5</span></span>|<span data-ttu-id="f55e2-127">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="f55e2-127">Auto-install and restart without end-user control</span></span>|



