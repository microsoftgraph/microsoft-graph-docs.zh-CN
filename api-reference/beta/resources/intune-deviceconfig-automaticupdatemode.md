---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bb7af7e6a54da14c16313a712e1c745467e61783
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43469840"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="58be2-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="58be2-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="58be2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58be2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58be2-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58be2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58be2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58be2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58be2-107">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="58be2-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="58be2-108">成员</span><span class="sxs-lookup"><span data-stu-id="58be2-108">Members</span></span>
|<span data-ttu-id="58be2-109">成员</span><span class="sxs-lookup"><span data-stu-id="58be2-109">Member</span></span>|<span data-ttu-id="58be2-110">值</span><span class="sxs-lookup"><span data-stu-id="58be2-110">Value</span></span>|<span data-ttu-id="58be2-111">说明</span><span class="sxs-lookup"><span data-stu-id="58be2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58be2-112">定制</span><span class="sxs-lookup"><span data-stu-id="58be2-112">userDefined</span></span>|<span data-ttu-id="58be2-113">0</span><span class="sxs-lookup"><span data-stu-id="58be2-113">0</span></span>|<span data-ttu-id="58be2-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="58be2-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="58be2-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="58be2-115">notifyDownload</span></span>|<span data-ttu-id="58be2-116">1</span><span class="sxs-lookup"><span data-stu-id="58be2-116">1</span></span>|<span data-ttu-id="58be2-117">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="58be2-117">Notify on download.</span></span>|
|<span data-ttu-id="58be2-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="58be2-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="58be2-119">双面</span><span class="sxs-lookup"><span data-stu-id="58be2-119">2</span></span>|<span data-ttu-id="58be2-120">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="58be2-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="58be2-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="58be2-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="58be2-122">第三章</span><span class="sxs-lookup"><span data-stu-id="58be2-122">3</span></span>|<span data-ttu-id="58be2-123">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="58be2-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="58be2-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="58be2-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="58be2-125">4 </span><span class="sxs-lookup"><span data-stu-id="58be2-125">4</span></span>|<span data-ttu-id="58be2-126">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="58be2-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="58be2-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="58be2-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="58be2-128">5 </span><span class="sxs-lookup"><span data-stu-id="58be2-128">5</span></span>|<span data-ttu-id="58be2-129">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="58be2-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="58be2-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="58be2-130">windowsDefault</span></span>|<span data-ttu-id="58be2-131">6 </span><span class="sxs-lookup"><span data-stu-id="58be2-131">6</span></span>|<span data-ttu-id="58be2-132">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="58be2-132">Reset to Windows default value.</span></span>|



