---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d982c4c9ee524712c212eba1b8b44349d0a70377
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402634"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="21740-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21740-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="21740-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="21740-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="21740-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21740-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21740-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21740-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21740-107">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="21740-107">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="21740-108">成员</span><span class="sxs-lookup"><span data-stu-id="21740-108">Members</span></span>
|<span data-ttu-id="21740-109">成员</span><span class="sxs-lookup"><span data-stu-id="21740-109">Member</span></span>|<span data-ttu-id="21740-110">值</span><span class="sxs-lookup"><span data-stu-id="21740-110">Value</span></span>|<span data-ttu-id="21740-111">说明</span><span class="sxs-lookup"><span data-stu-id="21740-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21740-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="21740-112">userDefined</span></span>|<span data-ttu-id="21740-113">0</span><span class="sxs-lookup"><span data-stu-id="21740-113">0</span></span>|<span data-ttu-id="21740-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="21740-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="21740-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="21740-115">notifyDownload</span></span>|<span data-ttu-id="21740-116">1</span><span class="sxs-lookup"><span data-stu-id="21740-116">1</span></span>|<span data-ttu-id="21740-117">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="21740-117">Notify on download.</span></span>|
|<span data-ttu-id="21740-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="21740-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="21740-119">2</span><span class="sxs-lookup"><span data-stu-id="21740-119">2</span></span>|<span data-ttu-id="21740-120">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="21740-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="21740-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="21740-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="21740-122">3</span><span class="sxs-lookup"><span data-stu-id="21740-122">3</span></span>|<span data-ttu-id="21740-123">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="21740-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="21740-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="21740-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="21740-125">4</span><span class="sxs-lookup"><span data-stu-id="21740-125">4</span></span>|<span data-ttu-id="21740-126">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="21740-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="21740-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="21740-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="21740-128">5</span><span class="sxs-lookup"><span data-stu-id="21740-128">5</span></span>|<span data-ttu-id="21740-129">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="21740-129">Auto-install and restart without end-user control</span></span>|
|<span data-ttu-id="21740-130">windowsDefault</span><span class="sxs-lookup"><span data-stu-id="21740-130">windowsDefault</span></span>|<span data-ttu-id="21740-131">6</span><span class="sxs-lookup"><span data-stu-id="21740-131">6</span></span>|<span data-ttu-id="21740-132">重置为 Windows 默认值。</span><span class="sxs-lookup"><span data-stu-id="21740-132">Reset to Windows default value.</span></span>|




