---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 3a0cc2d3918573fca6480c6eecd07889534cda4b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028572"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="0f99e-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0f99e-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="0f99e-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0f99e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0f99e-105">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="0f99e-105">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="0f99e-106">成员</span><span class="sxs-lookup"><span data-stu-id="0f99e-106">Members</span></span>
|<span data-ttu-id="0f99e-107">成员</span><span class="sxs-lookup"><span data-stu-id="0f99e-107">Member</span></span>|<span data-ttu-id="0f99e-108">值</span><span class="sxs-lookup"><span data-stu-id="0f99e-108">Value</span></span>|<span data-ttu-id="0f99e-109">说明</span><span class="sxs-lookup"><span data-stu-id="0f99e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0f99e-110">定制</span><span class="sxs-lookup"><span data-stu-id="0f99e-110">userDefined</span></span>|<span data-ttu-id="0f99e-111">0</span><span class="sxs-lookup"><span data-stu-id="0f99e-111">0</span></span>|<span data-ttu-id="0f99e-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="0f99e-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="0f99e-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="0f99e-113">notifyDownload</span></span>|<span data-ttu-id="0f99e-114">1</span><span class="sxs-lookup"><span data-stu-id="0f99e-114">1</span></span>|<span data-ttu-id="0f99e-115">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="0f99e-115">Notify on download.</span></span>|
|<span data-ttu-id="0f99e-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="0f99e-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="0f99e-117">双面</span><span class="sxs-lookup"><span data-stu-id="0f99e-117">2</span></span>|<span data-ttu-id="0f99e-118">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="0f99e-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="0f99e-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="0f99e-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="0f99e-120">第三章</span><span class="sxs-lookup"><span data-stu-id="0f99e-120">3</span></span>|<span data-ttu-id="0f99e-121">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="0f99e-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="0f99e-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="0f99e-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="0f99e-123">4</span><span class="sxs-lookup"><span data-stu-id="0f99e-123">4</span></span>|<span data-ttu-id="0f99e-124">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="0f99e-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="0f99e-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="0f99e-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="0f99e-126">5</span><span class="sxs-lookup"><span data-stu-id="0f99e-126">5</span></span>|<span data-ttu-id="0f99e-127">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="0f99e-127">Auto-install and restart without end-user control</span></span>|



