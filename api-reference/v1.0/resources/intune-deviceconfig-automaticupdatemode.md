---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b4cd222db425a9a8a2647f2ffbeb6056dddbe1c5
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755901"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="d86f0-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d86f0-103">automaticUpdateMode enum type</span></span>

<span data-ttu-id="d86f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d86f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d86f0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d86f0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d86f0-106">自动更新模式的可能值。</span><span class="sxs-lookup"><span data-stu-id="d86f0-106">Possible values for automatic update mode.</span></span>

## <a name="members"></a><span data-ttu-id="d86f0-107">成员</span><span class="sxs-lookup"><span data-stu-id="d86f0-107">Members</span></span>
|<span data-ttu-id="d86f0-108">成员</span><span class="sxs-lookup"><span data-stu-id="d86f0-108">Member</span></span>|<span data-ttu-id="d86f0-109">值</span><span class="sxs-lookup"><span data-stu-id="d86f0-109">Value</span></span>|<span data-ttu-id="d86f0-110">Description</span><span class="sxs-lookup"><span data-stu-id="d86f0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d86f0-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="d86f0-111">userDefined</span></span>|<span data-ttu-id="d86f0-112">0</span><span class="sxs-lookup"><span data-stu-id="d86f0-112">0</span></span>|<span data-ttu-id="d86f0-113">用户定义，默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="d86f0-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d86f0-114">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="d86f0-114">notifyDownload</span></span>|<span data-ttu-id="d86f0-115">1</span><span class="sxs-lookup"><span data-stu-id="d86f0-115">1</span></span>|<span data-ttu-id="d86f0-116">下载时通知。</span><span class="sxs-lookup"><span data-stu-id="d86f0-116">Notify on download.</span></span>|
|<span data-ttu-id="d86f0-117">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d86f0-117">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="d86f0-118">2</span><span class="sxs-lookup"><span data-stu-id="d86f0-118">2</span></span>|<span data-ttu-id="d86f0-119">在维护时自动安装。</span><span class="sxs-lookup"><span data-stu-id="d86f0-119">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="d86f0-120">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d86f0-120">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="d86f0-121">3</span><span class="sxs-lookup"><span data-stu-id="d86f0-121">3</span></span>|<span data-ttu-id="d86f0-122">在维护时自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="d86f0-122">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="d86f0-123">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="d86f0-123">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="d86f0-124">4 </span><span class="sxs-lookup"><span data-stu-id="d86f0-124">4</span></span>|<span data-ttu-id="d86f0-125">按计划时间自动安装和重启。</span><span class="sxs-lookup"><span data-stu-id="d86f0-125">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="d86f0-126">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="d86f0-126">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="d86f0-127">5 </span><span class="sxs-lookup"><span data-stu-id="d86f0-127">5</span></span>|<span data-ttu-id="d86f0-128">在没有最终用户控制的情况下自动安装和重启</span><span class="sxs-lookup"><span data-stu-id="d86f0-128">Auto-install and restart without end-user control</span></span>|




