---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: bd3b2a63fe933fcd20de4f76a0ba92e31fe75b38
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725587"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="13745-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="13745-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="13745-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13745-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13745-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13745-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13745-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13745-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13745-107">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="13745-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="13745-108">成员</span><span class="sxs-lookup"><span data-stu-id="13745-108">Members</span></span>
|<span data-ttu-id="13745-109">成员</span><span class="sxs-lookup"><span data-stu-id="13745-109">Member</span></span>|<span data-ttu-id="13745-110">值</span><span class="sxs-lookup"><span data-stu-id="13745-110">Value</span></span>|<span data-ttu-id="13745-111">说明</span><span class="sxs-lookup"><span data-stu-id="13745-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13745-112">定制</span><span class="sxs-lookup"><span data-stu-id="13745-112">userDefined</span></span>|<span data-ttu-id="13745-113">0</span><span class="sxs-lookup"><span data-stu-id="13745-113">0</span></span>|<span data-ttu-id="13745-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="13745-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="13745-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="13745-115">notifyDownload</span></span>|<span data-ttu-id="13745-116">1</span><span class="sxs-lookup"><span data-stu-id="13745-116">1</span></span>|<span data-ttu-id="13745-117">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="13745-117">Notify on download.</span></span>|
|<span data-ttu-id="13745-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="13745-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="13745-119">双面</span><span class="sxs-lookup"><span data-stu-id="13745-119">2</span></span>|<span data-ttu-id="13745-120">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="13745-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="13745-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="13745-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="13745-122">第三章</span><span class="sxs-lookup"><span data-stu-id="13745-122">3</span></span>|<span data-ttu-id="13745-123">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="13745-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="13745-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="13745-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="13745-125">4 </span><span class="sxs-lookup"><span data-stu-id="13745-125">4</span></span>|<span data-ttu-id="13745-126">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="13745-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="13745-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="13745-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="13745-128">5 </span><span class="sxs-lookup"><span data-stu-id="13745-128">5</span></span>|<span data-ttu-id="13745-129">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="13745-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="13745-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="13745-130">windowsDefault</span></span>|<span data-ttu-id="13745-131">6 </span><span class="sxs-lookup"><span data-stu-id="13745-131">6</span></span>|<span data-ttu-id="13745-132">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="13745-132">Reset to Windows default value.</span></span>|





