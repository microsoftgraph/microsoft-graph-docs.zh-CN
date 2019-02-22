---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8302566eea465ec4477a01845778ab2d7ddee9fe
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30146709"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="9c447-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9c447-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="9c447-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9c447-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c447-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c447-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c447-106">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="9c447-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="9c447-107">成员</span><span class="sxs-lookup"><span data-stu-id="9c447-107">Members</span></span>
|<span data-ttu-id="9c447-108">成员</span><span class="sxs-lookup"><span data-stu-id="9c447-108">Member</span></span>|<span data-ttu-id="9c447-109">值</span><span class="sxs-lookup"><span data-stu-id="9c447-109">Value</span></span>|<span data-ttu-id="9c447-110">说明</span><span class="sxs-lookup"><span data-stu-id="9c447-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c447-111">定制</span><span class="sxs-lookup"><span data-stu-id="9c447-111">userDefined</span></span>|<span data-ttu-id="9c447-112">0</span><span class="sxs-lookup"><span data-stu-id="9c447-112">0</span></span>|<span data-ttu-id="9c447-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="9c447-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="9c447-114">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="9c447-114">alwaysNotify</span></span>|<span data-ttu-id="9c447-115">1</span><span class="sxs-lookup"><span data-stu-id="9c447-115">1</span></span>|<span data-ttu-id="9c447-116">总是通知。</span><span class="sxs-lookup"><span data-stu-id="9c447-116">Always notify.</span></span>|
|<span data-ttu-id="9c447-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="9c447-117">notifyOnAppChanges</span></span>|<span data-ttu-id="9c447-118">双面</span><span class="sxs-lookup"><span data-stu-id="9c447-118">2</span></span>|<span data-ttu-id="9c447-119">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="9c447-119">Notify on app changes.</span></span>|
|<span data-ttu-id="9c447-120">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="9c447-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="9c447-121">第三章</span><span class="sxs-lookup"><span data-stu-id="9c447-121">3</span></span>|<span data-ttu-id="9c447-122">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="9c447-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="9c447-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="9c447-123">neverNotify</span></span>|<span data-ttu-id="9c447-124">4</span><span class="sxs-lookup"><span data-stu-id="9c447-124">4</span></span>|<span data-ttu-id="9c447-125">从不通知。</span><span class="sxs-lookup"><span data-stu-id="9c447-125">Never notify.</span></span>|




