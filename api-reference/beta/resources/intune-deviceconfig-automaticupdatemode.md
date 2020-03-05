---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d44c4db05be66f568ba5c0b9182a6d2ab509088
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527069"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="6ffe1-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6ffe1-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="6ffe1-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6ffe1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ffe1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ffe1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ffe1-107">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="6ffe1-108">成员</span><span class="sxs-lookup"><span data-stu-id="6ffe1-108">Members</span></span>
|<span data-ttu-id="6ffe1-109">成员</span><span class="sxs-lookup"><span data-stu-id="6ffe1-109">Member</span></span>|<span data-ttu-id="6ffe1-110">值</span><span class="sxs-lookup"><span data-stu-id="6ffe1-110">Value</span></span>|<span data-ttu-id="6ffe1-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ffe1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ffe1-112">定制</span><span class="sxs-lookup"><span data-stu-id="6ffe1-112">userDefined</span></span>|<span data-ttu-id="6ffe1-113">0</span><span class="sxs-lookup"><span data-stu-id="6ffe1-113">0</span></span>|<span data-ttu-id="6ffe1-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6ffe1-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="6ffe1-115">notifyDownload</span></span>|<span data-ttu-id="6ffe1-116">1 </span><span class="sxs-lookup"><span data-stu-id="6ffe1-116">1</span></span>|<span data-ttu-id="6ffe1-117">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-117">Notify on download.</span></span>|
|<span data-ttu-id="6ffe1-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="6ffe1-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="6ffe1-119">2 </span><span class="sxs-lookup"><span data-stu-id="6ffe1-119">2</span></span>|<span data-ttu-id="6ffe1-120">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="6ffe1-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="6ffe1-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="6ffe1-122">3 </span><span class="sxs-lookup"><span data-stu-id="6ffe1-122">3</span></span>|<span data-ttu-id="6ffe1-123">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="6ffe1-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="6ffe1-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="6ffe1-125">4 </span><span class="sxs-lookup"><span data-stu-id="6ffe1-125">4</span></span>|<span data-ttu-id="6ffe1-126">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="6ffe1-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="6ffe1-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="6ffe1-128">5 </span><span class="sxs-lookup"><span data-stu-id="6ffe1-128">5</span></span>|<span data-ttu-id="6ffe1-129">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="6ffe1-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="6ffe1-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="6ffe1-130">windowsDefault</span></span>|<span data-ttu-id="6ffe1-131">6 </span><span class="sxs-lookup"><span data-stu-id="6ffe1-131">6</span></span>|<span data-ttu-id="6ffe1-132">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="6ffe1-132">Reset to Windows default value.</span></span>|



