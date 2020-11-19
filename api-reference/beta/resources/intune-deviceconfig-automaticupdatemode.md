---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a1ea942a2418f763a6914329dabe26cd0ace1e8a
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260760"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="c3e90-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c3e90-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="c3e90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3e90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3e90-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3e90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3e90-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3e90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3e90-107">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="c3e90-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="c3e90-108">成员</span><span class="sxs-lookup"><span data-stu-id="c3e90-108">Members</span></span>
|<span data-ttu-id="c3e90-109">成员</span><span class="sxs-lookup"><span data-stu-id="c3e90-109">Member</span></span>|<span data-ttu-id="c3e90-110">值</span><span class="sxs-lookup"><span data-stu-id="c3e90-110">Value</span></span>|<span data-ttu-id="c3e90-111">说明</span><span class="sxs-lookup"><span data-stu-id="c3e90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3e90-112">定制</span><span class="sxs-lookup"><span data-stu-id="c3e90-112">userDefined</span></span>|<span data-ttu-id="c3e90-113">0</span><span class="sxs-lookup"><span data-stu-id="c3e90-113">0</span></span>|<span data-ttu-id="c3e90-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="c3e90-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c3e90-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="c3e90-115">notifyDownload</span></span>|<span data-ttu-id="c3e90-116">1</span><span class="sxs-lookup"><span data-stu-id="c3e90-116">1</span></span>|<span data-ttu-id="c3e90-117">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="c3e90-117">Notify on download.</span></span>|
|<span data-ttu-id="c3e90-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c3e90-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="c3e90-119">双面</span><span class="sxs-lookup"><span data-stu-id="c3e90-119">2</span></span>|<span data-ttu-id="c3e90-120">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="c3e90-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="c3e90-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="c3e90-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="c3e90-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c3e90-122">3</span></span>|<span data-ttu-id="c3e90-123">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="c3e90-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="c3e90-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="c3e90-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="c3e90-125">4 </span><span class="sxs-lookup"><span data-stu-id="c3e90-125">4</span></span>|<span data-ttu-id="c3e90-126">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="c3e90-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="c3e90-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="c3e90-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="c3e90-128">5 </span><span class="sxs-lookup"><span data-stu-id="c3e90-128">5</span></span>|<span data-ttu-id="c3e90-129">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="c3e90-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="c3e90-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="c3e90-130">windowsDefault</span></span>|<span data-ttu-id="c3e90-131">6 </span><span class="sxs-lookup"><span data-stu-id="c3e90-131">6</span></span>|<span data-ttu-id="c3e90-132">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="c3e90-132">Reset to Windows default value.</span></span>|




