---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07a6b410289ea6455d0f6756efa7d1ec4d735ce4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27849985"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="f5397-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5397-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="f5397-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5397-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5397-105">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="f5397-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="f5397-106">成员</span><span class="sxs-lookup"><span data-stu-id="f5397-106">Members</span></span>
|<span data-ttu-id="f5397-107">成员</span><span class="sxs-lookup"><span data-stu-id="f5397-107">Member</span></span>|<span data-ttu-id="f5397-108">值</span><span class="sxs-lookup"><span data-stu-id="f5397-108">Value</span></span>|<span data-ttu-id="f5397-109">Description</span><span class="sxs-lookup"><span data-stu-id="f5397-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5397-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="f5397-110">userDefined</span></span>|<span data-ttu-id="f5397-111">0</span><span class="sxs-lookup"><span data-stu-id="f5397-111">0</span></span>|<span data-ttu-id="f5397-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="f5397-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f5397-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="f5397-113">notifyDownload</span></span>|<span data-ttu-id="f5397-114">1</span><span class="sxs-lookup"><span data-stu-id="f5397-114">1</span></span>|<span data-ttu-id="f5397-115">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="f5397-115">Notify on download.</span></span>|
|<span data-ttu-id="f5397-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f5397-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="f5397-117">2</span><span class="sxs-lookup"><span data-stu-id="f5397-117">2</span></span>|<span data-ttu-id="f5397-118">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="f5397-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="f5397-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="f5397-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="f5397-120">3</span><span class="sxs-lookup"><span data-stu-id="f5397-120">3</span></span>|<span data-ttu-id="f5397-121">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="f5397-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="f5397-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="f5397-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="f5397-123">4</span><span class="sxs-lookup"><span data-stu-id="f5397-123">4</span></span>|<span data-ttu-id="f5397-124">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="f5397-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="f5397-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="f5397-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="f5397-126">5</span><span class="sxs-lookup"><span data-stu-id="f5397-126">5</span></span>|<span data-ttu-id="f5397-127">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="f5397-127">Auto-install and restart without end-user control</span></span>|



