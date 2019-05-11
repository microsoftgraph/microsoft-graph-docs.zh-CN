---
title: macOSGatekeeperAppSources 枚举类型
description: MacOS 网关的应用程序源选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b178072bd4364b2fc0df813d5b8e56423c2b29fa
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33946145"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="76078-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="76078-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="76078-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76078-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76078-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76078-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76078-106">MacOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="76078-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="76078-107">成员</span><span class="sxs-lookup"><span data-stu-id="76078-107">Members</span></span>
|<span data-ttu-id="76078-108">成员</span><span class="sxs-lookup"><span data-stu-id="76078-108">Member</span></span>|<span data-ttu-id="76078-109">值</span><span class="sxs-lookup"><span data-stu-id="76078-109">Value</span></span>|<span data-ttu-id="76078-110">说明</span><span class="sxs-lookup"><span data-stu-id="76078-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76078-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="76078-111">notConfigured</span></span>|<span data-ttu-id="76078-112">0</span><span class="sxs-lookup"><span data-stu-id="76078-112">0</span></span>|<span data-ttu-id="76078-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="76078-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="76078-114">macAppStore</span><span class="sxs-lookup"><span data-stu-id="76078-114">macAppStore</span></span>|<span data-ttu-id="76078-115">1</span><span class="sxs-lookup"><span data-stu-id="76078-115">1</span></span>|<span data-ttu-id="76078-116">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="76078-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="76078-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="76078-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="76078-118">双面</span><span class="sxs-lookup"><span data-stu-id="76078-118">2</span></span>|<span data-ttu-id="76078-119">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="76078-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="76078-120">无论</span><span class="sxs-lookup"><span data-stu-id="76078-120">anywhere</span></span>|<span data-ttu-id="76078-121">第三章</span><span class="sxs-lookup"><span data-stu-id="76078-121">3</span></span>|<span data-ttu-id="76078-122">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="76078-122">Apps from anywhere can be run.</span></span>|




