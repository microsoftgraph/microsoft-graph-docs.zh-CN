---
title: appListType 枚举类型
description: 合规性应用程序列表的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5df56b14d3c5416a04245ffbccd0b3b887266bde
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987787"
---
# <a name="applisttype-enum-type"></a><span data-ttu-id="c6ab6-103">appListType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c6ab6-103">appListType enum type</span></span>

> <span data-ttu-id="c6ab6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c6ab6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c6ab6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c6ab6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c6ab6-106">合规性应用程序列表的可能值。</span><span class="sxs-lookup"><span data-stu-id="c6ab6-106">Possible values of the compliance app list.</span></span>

## <a name="members"></a><span data-ttu-id="c6ab6-107">成员</span><span class="sxs-lookup"><span data-stu-id="c6ab6-107">Members</span></span>
|<span data-ttu-id="c6ab6-108">成员</span><span class="sxs-lookup"><span data-stu-id="c6ab6-108">Member</span></span>|<span data-ttu-id="c6ab6-109">值</span><span class="sxs-lookup"><span data-stu-id="c6ab6-109">Value</span></span>|<span data-ttu-id="c6ab6-110">说明</span><span class="sxs-lookup"><span data-stu-id="c6ab6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c6ab6-111">无</span><span class="sxs-lookup"><span data-stu-id="c6ab6-111">none</span></span>|<span data-ttu-id="c6ab6-112">0</span><span class="sxs-lookup"><span data-stu-id="c6ab6-112">0</span></span>|<span data-ttu-id="c6ab6-113">默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="c6ab6-113">Default value, no intent.</span></span>|
|<span data-ttu-id="c6ab6-114">appsInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c6ab6-114">appsInListCompliant</span></span>|<span data-ttu-id="c6ab6-115">1</span><span class="sxs-lookup"><span data-stu-id="c6ab6-115">1</span></span>|<span data-ttu-id="c6ab6-116">此列表表示将被视为合规性的应用程序 (仅符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="c6ab6-116">The list represents the apps that will be considered compliant (only apps on the list are compliant).</span></span>|
|<span data-ttu-id="c6ab6-117">appsNotInListCompliant</span><span class="sxs-lookup"><span data-stu-id="c6ab6-117">appsNotInListCompliant</span></span>|<span data-ttu-id="c6ab6-118">双面</span><span class="sxs-lookup"><span data-stu-id="c6ab6-118">2</span></span>|<span data-ttu-id="c6ab6-119">此列表表示将被视为不合规的应用程序 (所有应用程序都符合列表中的应用程序)。</span><span class="sxs-lookup"><span data-stu-id="c6ab6-119">The list represents the apps that will be considered non compliant (all apps are compliant except apps on the list).</span></span>|





