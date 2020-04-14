---
title: windowsUserAccountControlSettings 枚举类型
description: Windows 用户帐户控制设置的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8e2523949829f858064c9dc7bceca2cd55cf9b2a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43456936"
---
# <a name="windowsuseraccountcontrolsettings-enum-type"></a><span data-ttu-id="f0759-103">windowsUserAccountControlSettings 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f0759-103">windowsUserAccountControlSettings enum type</span></span>

<span data-ttu-id="f0759-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f0759-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f0759-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f0759-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f0759-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f0759-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f0759-107">Windows 用户帐户控制设置的可能值。</span><span class="sxs-lookup"><span data-stu-id="f0759-107">Possible values for Windows user account control settings.</span></span>

## <a name="members"></a><span data-ttu-id="f0759-108">成员</span><span class="sxs-lookup"><span data-stu-id="f0759-108">Members</span></span>
|<span data-ttu-id="f0759-109">成员</span><span class="sxs-lookup"><span data-stu-id="f0759-109">Member</span></span>|<span data-ttu-id="f0759-110">值</span><span class="sxs-lookup"><span data-stu-id="f0759-110">Value</span></span>|<span data-ttu-id="f0759-111">说明</span><span class="sxs-lookup"><span data-stu-id="f0759-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f0759-112">定制</span><span class="sxs-lookup"><span data-stu-id="f0759-112">userDefined</span></span>|<span data-ttu-id="f0759-113">0</span><span class="sxs-lookup"><span data-stu-id="f0759-113">0</span></span>|<span data-ttu-id="f0759-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="f0759-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f0759-115">alwaysNotify</span><span class="sxs-lookup"><span data-stu-id="f0759-115">alwaysNotify</span></span>|<span data-ttu-id="f0759-116">1</span><span class="sxs-lookup"><span data-stu-id="f0759-116">1</span></span>|<span data-ttu-id="f0759-117">总是通知。</span><span class="sxs-lookup"><span data-stu-id="f0759-117">Always notify.</span></span>|
|<span data-ttu-id="f0759-118">notifyOnAppChanges</span><span class="sxs-lookup"><span data-stu-id="f0759-118">notifyOnAppChanges</span></span>|<span data-ttu-id="f0759-119">双面</span><span class="sxs-lookup"><span data-stu-id="f0759-119">2</span></span>|<span data-ttu-id="f0759-120">通知应用更改。</span><span class="sxs-lookup"><span data-stu-id="f0759-120">Notify on app changes.</span></span>|
|<span data-ttu-id="f0759-121">notifyOnAppChangesWithoutDimming</span><span class="sxs-lookup"><span data-stu-id="f0759-121">notifyOnAppChangesWithoutDimming</span></span>|<span data-ttu-id="f0759-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f0759-122">3</span></span>|<span data-ttu-id="f0759-123">在应用程序发生更改时通知桌面不变暗。</span><span class="sxs-lookup"><span data-stu-id="f0759-123">Notify on app changes without dimming desktop.</span></span>|
|<span data-ttu-id="f0759-124">neverNotify</span><span class="sxs-lookup"><span data-stu-id="f0759-124">neverNotify</span></span>|<span data-ttu-id="f0759-125">4 </span><span class="sxs-lookup"><span data-stu-id="f0759-125">4</span></span>|<span data-ttu-id="f0759-126">从不通知。</span><span class="sxs-lookup"><span data-stu-id="f0759-126">Never notify.</span></span>|



