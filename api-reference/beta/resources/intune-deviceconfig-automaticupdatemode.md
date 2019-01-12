---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20aa217838848af6d85c023fd6587afe3427e82b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913266"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="8bb2b-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8bb2b-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="8bb2b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8bb2b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8bb2b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8bb2b-107">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="8bb2b-108">成员</span><span class="sxs-lookup"><span data-stu-id="8bb2b-108">Members</span></span>
|<span data-ttu-id="8bb2b-109">成员</span><span class="sxs-lookup"><span data-stu-id="8bb2b-109">Member</span></span>|<span data-ttu-id="8bb2b-110">值</span><span class="sxs-lookup"><span data-stu-id="8bb2b-110">Value</span></span>|<span data-ttu-id="8bb2b-111">Description</span><span class="sxs-lookup"><span data-stu-id="8bb2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8bb2b-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="8bb2b-112">userDefined</span></span>|<span data-ttu-id="8bb2b-113">0</span><span class="sxs-lookup"><span data-stu-id="8bb2b-113">0</span></span>|<span data-ttu-id="8bb2b-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8bb2b-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="8bb2b-115">notifyDownload</span></span>|<span data-ttu-id="8bb2b-116">1</span><span class="sxs-lookup"><span data-stu-id="8bb2b-116">1</span></span>|<span data-ttu-id="8bb2b-117">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-117">Notify on download.</span></span>|
|<span data-ttu-id="8bb2b-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="8bb2b-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="8bb2b-119">2</span><span class="sxs-lookup"><span data-stu-id="8bb2b-119">2</span></span>|<span data-ttu-id="8bb2b-120">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="8bb2b-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="8bb2b-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="8bb2b-122">3</span><span class="sxs-lookup"><span data-stu-id="8bb2b-122">3</span></span>|<span data-ttu-id="8bb2b-123">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="8bb2b-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="8bb2b-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="8bb2b-125">4</span><span class="sxs-lookup"><span data-stu-id="8bb2b-125">4</span></span>|<span data-ttu-id="8bb2b-126">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="8bb2b-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="8bb2b-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="8bb2b-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="8bb2b-128">5</span><span class="sxs-lookup"><span data-stu-id="8bb2b-128">5</span></span>|<span data-ttu-id="8bb2b-129">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="8bb2b-129">Auto-install and restart without end-user control</span></span>|





