---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c8ff424dbb41356bd732fc2e7b100073b6df2c52
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42786142"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="6b066-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6b066-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="6b066-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6b066-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6b066-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b066-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b066-106">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="6b066-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="6b066-107">成员</span><span class="sxs-lookup"><span data-stu-id="6b066-107">Members</span></span>
|<span data-ttu-id="6b066-108">成员</span><span class="sxs-lookup"><span data-stu-id="6b066-108">Member</span></span>|<span data-ttu-id="6b066-109">值</span><span class="sxs-lookup"><span data-stu-id="6b066-109">Value</span></span>|<span data-ttu-id="6b066-110">说明</span><span class="sxs-lookup"><span data-stu-id="6b066-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b066-111">定制</span><span class="sxs-lookup"><span data-stu-id="6b066-111">userDefined</span></span>|<span data-ttu-id="6b066-112">0</span><span class="sxs-lookup"><span data-stu-id="6b066-112">0</span></span>|<span data-ttu-id="6b066-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="6b066-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="6b066-114">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="6b066-114">alwaysNotify</span></span>|<span data-ttu-id="6b066-115">1</span><span class="sxs-lookup"><span data-stu-id="6b066-115">1</span></span>|<span data-ttu-id="6b066-116">总是通知。</span><span class="sxs-lookup"><span data-stu-id="6b066-116">Always notify.</span></span>|
|<span data-ttu-id="6b066-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="6b066-117">notifyOnAppChanges</span></span>|<span data-ttu-id="6b066-118">双面</span><span class="sxs-lookup"><span data-stu-id="6b066-118">2</span></span>|<span data-ttu-id="6b066-119">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="6b066-119">Notify on app changes.</span></span>|
|<span data-ttu-id="6b066-120">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="6b066-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="6b066-121">第三章</span><span class="sxs-lookup"><span data-stu-id="6b066-121">3</span></span>|<span data-ttu-id="6b066-122">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="6b066-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="6b066-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="6b066-123">neverNotify</span></span>|<span data-ttu-id="6b066-124">4 </span><span class="sxs-lookup"><span data-stu-id="6b066-124">4</span></span>|<span data-ttu-id="6b066-125">从不通知。</span><span class="sxs-lookup"><span data-stu-id="6b066-125">Never notify.</span></span>|



