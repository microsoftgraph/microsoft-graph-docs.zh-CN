---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90366deee96e898d8339d59cb1a49879ba019c16
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075901"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="0e5fb-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0e5fb-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="0e5fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0e5fb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0e5fb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0e5fb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0e5fb-107">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="0e5fb-108">成员</span><span class="sxs-lookup"><span data-stu-id="0e5fb-108">Members</span></span>
|<span data-ttu-id="0e5fb-109">成员</span><span class="sxs-lookup"><span data-stu-id="0e5fb-109">Member</span></span>|<span data-ttu-id="0e5fb-110">值</span><span class="sxs-lookup"><span data-stu-id="0e5fb-110">Value</span></span>|<span data-ttu-id="0e5fb-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e5fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e5fb-112">定制</span><span class="sxs-lookup"><span data-stu-id="0e5fb-112">userDefined</span></span>|<span data-ttu-id="0e5fb-113">0</span><span class="sxs-lookup"><span data-stu-id="0e5fb-113">0</span></span>|<span data-ttu-id="0e5fb-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="0e5fb-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="0e5fb-115">notifyDownload</span></span>|<span data-ttu-id="0e5fb-116">1 </span><span class="sxs-lookup"><span data-stu-id="0e5fb-116">1</span></span>|<span data-ttu-id="0e5fb-117">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-117">Notify on download.</span></span>|
|<span data-ttu-id="0e5fb-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="0e5fb-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="0e5fb-119">2 </span><span class="sxs-lookup"><span data-stu-id="0e5fb-119">2</span></span>|<span data-ttu-id="0e5fb-120">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="0e5fb-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="0e5fb-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="0e5fb-122">第三章</span><span class="sxs-lookup"><span data-stu-id="0e5fb-122">3</span></span>|<span data-ttu-id="0e5fb-123">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="0e5fb-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="0e5fb-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="0e5fb-125">4 </span><span class="sxs-lookup"><span data-stu-id="0e5fb-125">4</span></span>|<span data-ttu-id="0e5fb-126">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="0e5fb-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="0e5fb-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="0e5fb-128">5 </span><span class="sxs-lookup"><span data-stu-id="0e5fb-128">5</span></span>|<span data-ttu-id="0e5fb-129">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="0e5fb-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="0e5fb-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="0e5fb-130">windowsDefault</span></span>|<span data-ttu-id="0e5fb-131">6 </span><span class="sxs-lookup"><span data-stu-id="0e5fb-131">6</span></span>|<span data-ttu-id="0e5fb-132">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="0e5fb-132">Reset to Windows default value.</span></span>|






