---
title: windowsUpdateNotificationDisplayOption 枚举类型
description: Windows 更新通知显示选项
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b5ff0352aa1b80f6ca5fceb4cc7855d92cee3493
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43441113"
---
# <a name="windowsupdatenotificationdisplayoption-enum-type"></a><span data-ttu-id="fb006-103">windowsUpdateNotificationDisplayOption 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fb006-103">windowsUpdateNotificationDisplayOption enum type</span></span>

<span data-ttu-id="fb006-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb006-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fb006-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fb006-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fb006-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fb006-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fb006-107">Windows 更新通知显示选项</span><span class="sxs-lookup"><span data-stu-id="fb006-107">Windows Update Notification Display Options</span></span>

## <a name="members"></a><span data-ttu-id="fb006-108">成员</span><span class="sxs-lookup"><span data-stu-id="fb006-108">Members</span></span>
|<span data-ttu-id="fb006-109">成员</span><span class="sxs-lookup"><span data-stu-id="fb006-109">Member</span></span>|<span data-ttu-id="fb006-110">值</span><span class="sxs-lookup"><span data-stu-id="fb006-110">Value</span></span>|<span data-ttu-id="fb006-111">说明</span><span class="sxs-lookup"><span data-stu-id="fb006-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb006-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fb006-112">notConfigured</span></span>|<span data-ttu-id="fb006-113">0</span><span class="sxs-lookup"><span data-stu-id="fb006-113">0</span></span>|<span data-ttu-id="fb006-114">未配置</span><span class="sxs-lookup"><span data-stu-id="fb006-114">Not configured</span></span>|
|<span data-ttu-id="fb006-115">defaultNotifications</span><span class="sxs-lookup"><span data-stu-id="fb006-115">defaultNotifications</span></span>|<span data-ttu-id="fb006-116">1</span><span class="sxs-lookup"><span data-stu-id="fb006-116">1</span></span>|<span data-ttu-id="fb006-117">使用默认的 Windows 更新通知。</span><span class="sxs-lookup"><span data-stu-id="fb006-117">Use the default Windows Update notifications.</span></span>|
|<span data-ttu-id="fb006-118">restartWarningsOnly</span><span class="sxs-lookup"><span data-stu-id="fb006-118">restartWarningsOnly</span></span>|<span data-ttu-id="fb006-119">双面</span><span class="sxs-lookup"><span data-stu-id="fb006-119">2</span></span>|<span data-ttu-id="fb006-120">关闭所有通知，但不包括重新启动警告。</span><span class="sxs-lookup"><span data-stu-id="fb006-120">Turn off all notifications, excluding restart warnings.</span></span>|
|<span data-ttu-id="fb006-121">disableAllNotifications</span><span class="sxs-lookup"><span data-stu-id="fb006-121">disableAllNotifications</span></span>|<span data-ttu-id="fb006-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fb006-122">3</span></span>|<span data-ttu-id="fb006-123">关闭所有通知，包括重启警告。</span><span class="sxs-lookup"><span data-stu-id="fb006-123">Turn off all notifications, including restart warnings.</span></span>|



