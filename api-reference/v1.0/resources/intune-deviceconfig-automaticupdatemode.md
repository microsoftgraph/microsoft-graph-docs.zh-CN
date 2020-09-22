---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: e02f1a3ed99840382148d4f1434df667e2391739
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051114"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="b813a-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b813a-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="b813a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b813a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b813a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b813a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b813a-106">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="b813a-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="b813a-107">成员</span><span class="sxs-lookup"><span data-stu-id="b813a-107">Members</span></span>
|<span data-ttu-id="b813a-108">成员</span><span class="sxs-lookup"><span data-stu-id="b813a-108">Member</span></span>|<span data-ttu-id="b813a-109">值</span><span class="sxs-lookup"><span data-stu-id="b813a-109">Value</span></span>|<span data-ttu-id="b813a-110">说明</span><span class="sxs-lookup"><span data-stu-id="b813a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b813a-111">定制</span><span class="sxs-lookup"><span data-stu-id="b813a-111">userDefined</span></span>|<span data-ttu-id="b813a-112">0</span><span class="sxs-lookup"><span data-stu-id="b813a-112">0</span></span>|<span data-ttu-id="b813a-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="b813a-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="b813a-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="b813a-114">notifyDownload</span></span>|<span data-ttu-id="b813a-115">1 </span><span class="sxs-lookup"><span data-stu-id="b813a-115">1</span></span>|<span data-ttu-id="b813a-116">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="b813a-116">Notify on download.</span></span>|
|<span data-ttu-id="b813a-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b813a-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="b813a-118">2 </span><span class="sxs-lookup"><span data-stu-id="b813a-118">2</span></span>|<span data-ttu-id="b813a-119">在维护时间自动安装。</span><span class="sxs-lookup"><span data-stu-id="b813a-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="b813a-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="b813a-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="b813a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b813a-121">3</span></span>|<span data-ttu-id="b813a-122">在维护时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="b813a-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="b813a-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="b813a-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="b813a-124">4 </span><span class="sxs-lookup"><span data-stu-id="b813a-124">4</span></span>|<span data-ttu-id="b813a-125">在计划的时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="b813a-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="b813a-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="b813a-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="b813a-127">5 </span><span class="sxs-lookup"><span data-stu-id="b813a-127">5</span></span>|<span data-ttu-id="b813a-128">在没有最终用户控件的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="b813a-128">Auto-install and restart without end-user control</span></span>|









