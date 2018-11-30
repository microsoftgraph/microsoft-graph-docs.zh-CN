---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
ms.openlocfilehash: b7eac8337d6c8286e538bbe98b5ecbc13a448628
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047251"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="ec5c2-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ec5c2-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="ec5c2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ec5c2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ec5c2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec5c2-107">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-107">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="ec5c2-108">成员</span><span class="sxs-lookup"><span data-stu-id="ec5c2-108">Members</span></span>
|<span data-ttu-id="ec5c2-109">成员</span><span class="sxs-lookup"><span data-stu-id="ec5c2-109">Member</span></span>|<span data-ttu-id="ec5c2-110">值</span><span class="sxs-lookup"><span data-stu-id="ec5c2-110">Value</span></span>|<span data-ttu-id="ec5c2-111">说明</span><span class="sxs-lookup"><span data-stu-id="ec5c2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec5c2-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="ec5c2-112">userDefined</span></span>|<span data-ttu-id="ec5c2-113">0</span><span class="sxs-lookup"><span data-stu-id="ec5c2-113">0</span></span>|<span data-ttu-id="ec5c2-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ec5c2-115">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="ec5c2-115">notifyDownload</span></span>|<span data-ttu-id="ec5c2-116">1</span><span class="sxs-lookup"><span data-stu-id="ec5c2-116">1</span></span>|<span data-ttu-id="ec5c2-117">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-117">Notify on download.</span></span>|
|<span data-ttu-id="ec5c2-118">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="ec5c2-118">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="ec5c2-119">2</span><span class="sxs-lookup"><span data-stu-id="ec5c2-119">2</span></span>|<span data-ttu-id="ec5c2-120">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-120">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="ec5c2-121">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="ec5c2-121">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="ec5c2-122">3</span><span class="sxs-lookup"><span data-stu-id="ec5c2-122">3</span></span>|<span data-ttu-id="ec5c2-123">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-123">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="ec5c2-124">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="ec5c2-124">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="ec5c2-125">4</span><span class="sxs-lookup"><span data-stu-id="ec5c2-125">4</span></span>|<span data-ttu-id="ec5c2-126">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="ec5c2-126">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="ec5c2-127">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="ec5c2-127">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="ec5c2-128">5</span><span class="sxs-lookup"><span data-stu-id="ec5c2-128">5</span></span>|<span data-ttu-id="ec5c2-129">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="ec5c2-129">Auto-install and restart without end-user control</span></span>|





