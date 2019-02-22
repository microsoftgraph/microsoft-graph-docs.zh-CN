---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3b7d11107ca3ea2b698e28cd288f163ec190b0a6
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30172672"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="c911a-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c911a-103">appListType enum type</span></span>

> <span data-ttu-id="c911a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c911a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c911a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c911a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c911a-106">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="c911a-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="c911a-107">成员</span><span class="sxs-lookup"><span data-stu-id="c911a-107">Members</span></span>
|<span data-ttu-id="c911a-108">成员</span><span class="sxs-lookup"><span data-stu-id="c911a-108">Member</span></span>|<span data-ttu-id="c911a-109">值</span><span class="sxs-lookup"><span data-stu-id="c911a-109">Value</span></span>|<span data-ttu-id="c911a-110">说明</span><span class="sxs-lookup"><span data-stu-id="c911a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c911a-111">无</span><span class="sxs-lookup"><span data-stu-id="c911a-111">none</span></span>|<span data-ttu-id="c911a-112">0</span><span class="sxs-lookup"><span data-stu-id="c911a-112">0</span></span>|<span data-ttu-id="c911a-113">默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="c911a-113">Default value, no intent.</span></span>|
|<span data-ttu-id="c911a-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c911a-114">appsInListCompliant</span></span>|<span data-ttu-id="c911a-115">1</span><span class="sxs-lookup"><span data-stu-id="c911a-115">1</span></span>|<span data-ttu-id="c911a-116">此列表表示将被视为合规性的应用程序 (仅符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="c911a-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="c911a-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c911a-117">appsNotInListCompliant</span></span>|<span data-ttu-id="c911a-118">双面</span><span class="sxs-lookup"><span data-stu-id="c911a-118">2</span></span>|<span data-ttu-id="c911a-119">此列表表示将被视为不合规的应用程序 (所有应用程序都符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="c911a-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|




