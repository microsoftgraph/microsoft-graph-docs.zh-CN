---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 55346e5946129393ae9302c9fbc582313be9819f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35968671"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="43008-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="43008-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="43008-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="43008-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43008-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43008-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43008-106">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="43008-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="43008-107">成员</span><span class="sxs-lookup"><span data-stu-id="43008-107">Members</span></span>
|<span data-ttu-id="43008-108">成员</span><span class="sxs-lookup"><span data-stu-id="43008-108">Member</span></span>|<span data-ttu-id="43008-109">值</span><span class="sxs-lookup"><span data-stu-id="43008-109">Value</span></span>|<span data-ttu-id="43008-110">说明</span><span class="sxs-lookup"><span data-stu-id="43008-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43008-111">定制</span><span class="sxs-lookup"><span data-stu-id="43008-111">userDefined</span></span>|<span data-ttu-id="43008-112">0</span><span class="sxs-lookup"><span data-stu-id="43008-112">0</span></span>|<span data-ttu-id="43008-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="43008-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="43008-114">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="43008-114">alwaysNotify</span></span>|<span data-ttu-id="43008-115">1</span><span class="sxs-lookup"><span data-stu-id="43008-115">1</span></span>|<span data-ttu-id="43008-116">总是通知。</span><span class="sxs-lookup"><span data-stu-id="43008-116">Always notify.</span></span>|
|<span data-ttu-id="43008-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="43008-117">notifyOnAppChanges</span></span>|<span data-ttu-id="43008-118">双面</span><span class="sxs-lookup"><span data-stu-id="43008-118">2</span></span>|<span data-ttu-id="43008-119">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="43008-119">Notify on app changes.</span></span>|
|<span data-ttu-id="43008-120">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="43008-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="43008-121">第三章</span><span class="sxs-lookup"><span data-stu-id="43008-121">3</span></span>|<span data-ttu-id="43008-122">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="43008-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="43008-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="43008-123">neverNotify</span></span>|<span data-ttu-id="43008-124">4</span><span class="sxs-lookup"><span data-stu-id="43008-124">4</span></span>|<span data-ttu-id="43008-125">从不通知。</span><span class="sxs-lookup"><span data-stu-id="43008-125">Never notify.</span></span>|





