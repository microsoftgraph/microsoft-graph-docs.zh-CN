---
title: windowsUpdateNotificationDisplayOption 枚举类型
description: Windows 更新通知显示选项
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7e792e3a866a0fadae5f866654e50ffe16cdc4c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523641"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a><span data-ttu-id="4d561-103">windowsUpdateNotificationDisplayOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4d561-103">windowsUpdateNotificationDisplayOption enum type</span></span>

> <span data-ttu-id="4d561-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4d561-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4d561-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4d561-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4d561-106">Windows 更新通知显示选项</span><span class="sxs-lookup"><span data-stu-id="4d561-106">Windows Update Notification Display Options</span></span>

## <a name="members"></a><span data-ttu-id="4d561-107">成员</span><span class="sxs-lookup"><span data-stu-id="4d561-107">Members</span></span>
|<span data-ttu-id="4d561-108">成员</span><span class="sxs-lookup"><span data-stu-id="4d561-108">Member</span></span>|<span data-ttu-id="4d561-109">值</span><span class="sxs-lookup"><span data-stu-id="4d561-109">Value</span></span>|<span data-ttu-id="4d561-110">说明</span><span class="sxs-lookup"><span data-stu-id="4d561-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4d561-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4d561-111">notConfigured</span></span>|<span data-ttu-id="4d561-112">0</span><span class="sxs-lookup"><span data-stu-id="4d561-112">0</span></span>|<span data-ttu-id="4d561-113">未配置</span><span class="sxs-lookup"><span data-stu-id="4d561-113">Not configured</span></span>|
|<span data-ttu-id="4d561-114">defaultNotifications</span><span class="sxs-lookup"><span data-stu-id="4d561-114">defaultNotifications</span></span>|<span data-ttu-id="4d561-115">1</span><span class="sxs-lookup"><span data-stu-id="4d561-115">1</span></span>|<span data-ttu-id="4d561-116">使用默认的 Windows 更新通知。</span><span class="sxs-lookup"><span data-stu-id="4d561-116">Use the default Windows Update notifications.</span></span>|
|<span data-ttu-id="4d561-117">restartWarningsOnly</span><span class="sxs-lookup"><span data-stu-id="4d561-117">restartWarningsOnly</span></span>|<span data-ttu-id="4d561-118">2 </span><span class="sxs-lookup"><span data-stu-id="4d561-118">2</span></span>|<span data-ttu-id="4d561-119">关闭所有通知, 但不包括重新启动警告。</span><span class="sxs-lookup"><span data-stu-id="4d561-119">Turn off all notifications, excluding restart warnings.</span></span>|
|<span data-ttu-id="4d561-120">disableAllNotifications</span><span class="sxs-lookup"><span data-stu-id="4d561-120">disableAllNotifications</span></span>|<span data-ttu-id="4d561-121">3 </span><span class="sxs-lookup"><span data-stu-id="4d561-121">3</span></span>|<span data-ttu-id="4d561-122">关闭所有通知, 包括重启警告。</span><span class="sxs-lookup"><span data-stu-id="4d561-122">Turn off all notifications, including restart warnings.</span></span>|





