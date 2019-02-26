---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 478e525847f7f6519b3bd2cb230ce2657b409f9b
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30264104"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="313bb-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="313bb-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="313bb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="313bb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="313bb-105">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="313bb-105">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="313bb-106">成员</span><span class="sxs-lookup"><span data-stu-id="313bb-106">Members</span></span>
|<span data-ttu-id="313bb-107">成员</span><span class="sxs-lookup"><span data-stu-id="313bb-107">Member</span></span>|<span data-ttu-id="313bb-108">值</span><span class="sxs-lookup"><span data-stu-id="313bb-108">Value</span></span>|<span data-ttu-id="313bb-109">说明</span><span class="sxs-lookup"><span data-stu-id="313bb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="313bb-110">定制</span><span class="sxs-lookup"><span data-stu-id="313bb-110">userDefined</span></span>|<span data-ttu-id="313bb-111">0</span><span class="sxs-lookup"><span data-stu-id="313bb-111">0</span></span>|<span data-ttu-id="313bb-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="313bb-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="313bb-113">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="313bb-113">alwaysNotify</span></span>|<span data-ttu-id="313bb-114">1</span><span class="sxs-lookup"><span data-stu-id="313bb-114">1</span></span>|<span data-ttu-id="313bb-115">总是通知。</span><span class="sxs-lookup"><span data-stu-id="313bb-115">Always notify.</span></span>|
|<span data-ttu-id="313bb-116">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="313bb-116">notifyOnAppChanges</span></span>|<span data-ttu-id="313bb-117">双面</span><span class="sxs-lookup"><span data-stu-id="313bb-117">2</span></span>|<span data-ttu-id="313bb-118">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="313bb-118">Notify on app changes.</span></span>|
|<span data-ttu-id="313bb-119">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="313bb-119">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="313bb-120">第三章</span><span class="sxs-lookup"><span data-stu-id="313bb-120">3</span></span>|<span data-ttu-id="313bb-121">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="313bb-121">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="313bb-122">neverNotify</span><span class="sxs-lookup"><span data-stu-id="313bb-122">neverNotify</span></span>|<span data-ttu-id="313bb-123">4</span><span class="sxs-lookup"><span data-stu-id="313bb-123">4</span></span>|<span data-ttu-id="313bb-124">从不通知。</span><span class="sxs-lookup"><span data-stu-id="313bb-124">Never notify.</span></span>|



