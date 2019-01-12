---
title: automaticUpdateMode 枚举类型
description: 自动更新模式的的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a31c50b5d16f4b9be8db4f95f2bbd9bd0ca123e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27987858"
---
# <a name="automaticupdatemode-enum-type"></a><span data-ttu-id="d4348-103">automaticUpdateMode 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d4348-103">automaticUpdateMode enum type</span></span>

> <span data-ttu-id="d4348-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d4348-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4348-105">自动更新模式的的可能值。</span><span class="sxs-lookup"><span data-stu-id="d4348-105">Possible values for automatic update mode.</span></span>
## <a name="members"></a><span data-ttu-id="d4348-106">成员</span><span class="sxs-lookup"><span data-stu-id="d4348-106">Members</span></span>
|<span data-ttu-id="d4348-107">成员</span><span class="sxs-lookup"><span data-stu-id="d4348-107">Member</span></span>|<span data-ttu-id="d4348-108">值</span><span class="sxs-lookup"><span data-stu-id="d4348-108">Value</span></span>|<span data-ttu-id="d4348-109">说明</span><span class="sxs-lookup"><span data-stu-id="d4348-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4348-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="d4348-110">userDefined</span></span>|<span data-ttu-id="d4348-111">0</span><span class="sxs-lookup"><span data-stu-id="d4348-111">0</span></span>|<span data-ttu-id="d4348-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="d4348-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="d4348-113">notifyDownload</span><span class="sxs-lookup"><span data-stu-id="d4348-113">notifyDownload</span></span>|<span data-ttu-id="d4348-114">1</span><span class="sxs-lookup"><span data-stu-id="d4348-114">1</span></span>|<span data-ttu-id="d4348-115">在下载通知。</span><span class="sxs-lookup"><span data-stu-id="d4348-115">Notify on download.</span></span>|
|<span data-ttu-id="d4348-116">autoInstallAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d4348-116">autoInstallAtMaintenanceTime</span></span>|<span data-ttu-id="d4348-117">2</span><span class="sxs-lookup"><span data-stu-id="d4348-117">2</span></span>|<span data-ttu-id="d4348-118">自动安装在维护时间。</span><span class="sxs-lookup"><span data-stu-id="d4348-118">Auto-install at maintenance time.</span></span>|
|<span data-ttu-id="d4348-119">autoInstallAndRebootAtMaintenanceTime</span><span class="sxs-lookup"><span data-stu-id="d4348-119">autoInstallAndRebootAtMaintenanceTime</span></span>|<span data-ttu-id="d4348-120">3</span><span class="sxs-lookup"><span data-stu-id="d4348-120">3</span></span>|<span data-ttu-id="d4348-121">自动安装和维护时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="d4348-121">Auto-install and reboot at maintenance time.</span></span>|
|<span data-ttu-id="d4348-122">autoInstallAndRebootAtScheduledTime</span><span class="sxs-lookup"><span data-stu-id="d4348-122">autoInstallAndRebootAtScheduledTime</span></span>|<span data-ttu-id="d4348-123">4</span><span class="sxs-lookup"><span data-stu-id="d4348-123">4</span></span>|<span data-ttu-id="d4348-124">自动安装并在计划时间重新启动。</span><span class="sxs-lookup"><span data-stu-id="d4348-124">Auto-install and reboot at scheduled time.</span></span>|
|<span data-ttu-id="d4348-125">autoInstallAndRebootWithoutEndUserControl</span><span class="sxs-lookup"><span data-stu-id="d4348-125">autoInstallAndRebootWithoutEndUserControl</span></span>|<span data-ttu-id="d4348-126">5</span><span class="sxs-lookup"><span data-stu-id="d4348-126">5</span></span>|<span data-ttu-id="d4348-127">自动安装并重新启动不最终用户控件</span><span class="sxs-lookup"><span data-stu-id="d4348-127">Auto-install and restart without end-user control</span></span>|



