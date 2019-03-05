---
title: macOSGatekeeperAppSources 枚举类型
description: macOS 网关的应用程序源选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3e43505a745e87e52f2f1c12a5cc5ff08825c09
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166204"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="76b56-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="76b56-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="76b56-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="76b56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76b56-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="76b56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76b56-106">macOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="76b56-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="76b56-107">成员</span><span class="sxs-lookup"><span data-stu-id="76b56-107">Members</span></span>
|<span data-ttu-id="76b56-108">成员</span><span class="sxs-lookup"><span data-stu-id="76b56-108">Member</span></span>|<span data-ttu-id="76b56-109">值</span><span class="sxs-lookup"><span data-stu-id="76b56-109">Value</span></span>|<span data-ttu-id="76b56-110">说明</span><span class="sxs-lookup"><span data-stu-id="76b56-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76b56-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="76b56-111">notConfigured</span></span>|<span data-ttu-id="76b56-112">0</span><span class="sxs-lookup"><span data-stu-id="76b56-112">0</span></span>|<span data-ttu-id="76b56-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="76b56-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="76b56-114">macAppStore</span><span class="sxs-lookup"><span data-stu-id="76b56-114">macAppStore</span></span>|<span data-ttu-id="76b56-115">1</span><span class="sxs-lookup"><span data-stu-id="76b56-115">1</span></span>|<span data-ttu-id="76b56-116">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="76b56-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="76b56-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="76b56-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="76b56-118">双面</span><span class="sxs-lookup"><span data-stu-id="76b56-118">2</span></span>|<span data-ttu-id="76b56-119">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="76b56-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="76b56-120">无论</span><span class="sxs-lookup"><span data-stu-id="76b56-120">anywhere</span></span>|<span data-ttu-id="76b56-121">第三章</span><span class="sxs-lookup"><span data-stu-id="76b56-121">3</span></span>|<span data-ttu-id="76b56-122">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="76b56-122">Apps from anywhere can be run.</span></span>|




