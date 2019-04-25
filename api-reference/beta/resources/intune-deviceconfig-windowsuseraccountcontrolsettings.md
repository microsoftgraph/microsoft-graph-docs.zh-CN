---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6b63fe44abfb0a06e5978d78e49c392c08122e38
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523558"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="7f6f5-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7f6f5-103">windowsUserAccountControlSettings enum type</span></span>

> <span data-ttu-id="7f6f5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7f6f5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f6f5-106">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-106">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="7f6f5-107">成员</span><span class="sxs-lookup"><span data-stu-id="7f6f5-107">Members</span></span>
|<span data-ttu-id="7f6f5-108">成员</span><span class="sxs-lookup"><span data-stu-id="7f6f5-108">Member</span></span>|<span data-ttu-id="7f6f5-109">值</span><span class="sxs-lookup"><span data-stu-id="7f6f5-109">Value</span></span>|<span data-ttu-id="7f6f5-110">说明</span><span class="sxs-lookup"><span data-stu-id="7f6f5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f6f5-111">定制</span><span class="sxs-lookup"><span data-stu-id="7f6f5-111">userDefined</span></span>|<span data-ttu-id="7f6f5-112">0</span><span class="sxs-lookup"><span data-stu-id="7f6f5-112">0</span></span>|<span data-ttu-id="7f6f5-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="7f6f5-114">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="7f6f5-114">alwaysNotify</span></span>|<span data-ttu-id="7f6f5-115">1</span><span class="sxs-lookup"><span data-stu-id="7f6f5-115">1</span></span>|<span data-ttu-id="7f6f5-116">总是通知。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-116">Always notify.</span></span>|
|<span data-ttu-id="7f6f5-117">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="7f6f5-117">notifyOnAppChanges</span></span>|<span data-ttu-id="7f6f5-118">2 </span><span class="sxs-lookup"><span data-stu-id="7f6f5-118">2</span></span>|<span data-ttu-id="7f6f5-119">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-119">Notify on app changes.</span></span>|
|<span data-ttu-id="7f6f5-120">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="7f6f5-120">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="7f6f5-121">3 </span><span class="sxs-lookup"><span data-stu-id="7f6f5-121">3</span></span>|<span data-ttu-id="7f6f5-122">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-122">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="7f6f5-123">neverNotify</span><span class="sxs-lookup"><span data-stu-id="7f6f5-123">neverNotify</span></span>|<span data-ttu-id="7f6f5-124">4 </span><span class="sxs-lookup"><span data-stu-id="7f6f5-124">4</span></span>|<span data-ttu-id="7f6f5-125">从不通知。</span><span class="sxs-lookup"><span data-stu-id="7f6f5-125">Never notify.</span></span>|





