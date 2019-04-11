---
title: macOSGatekeeperAppSources 枚举类型
description: macOS 网关的应用程序源选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2dbe261b223a180f64016d41495a0f4fcec22868
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31771066"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="f26ca-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f26ca-103">macOSGatekeeperAppSources enum type</span></span>

> <span data-ttu-id="f26ca-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f26ca-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f26ca-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f26ca-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f26ca-106">macOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="f26ca-106">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="f26ca-107">成员</span><span class="sxs-lookup"><span data-stu-id="f26ca-107">Members</span></span>
|<span data-ttu-id="f26ca-108">成员</span><span class="sxs-lookup"><span data-stu-id="f26ca-108">Member</span></span>|<span data-ttu-id="f26ca-109">值</span><span class="sxs-lookup"><span data-stu-id="f26ca-109">Value</span></span>|<span data-ttu-id="f26ca-110">说明</span><span class="sxs-lookup"><span data-stu-id="f26ca-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f26ca-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f26ca-111">notConfigured</span></span>|<span data-ttu-id="f26ca-112">0</span><span class="sxs-lookup"><span data-stu-id="f26ca-112">0</span></span>|<span data-ttu-id="f26ca-113">设备默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f26ca-113">Device default value, no intent.</span></span>|
|<span data-ttu-id="f26ca-114">macAppStore</span><span class="sxs-lookup"><span data-stu-id="f26ca-114">macAppStore</span></span>|<span data-ttu-id="f26ca-115">1</span><span class="sxs-lookup"><span data-stu-id="f26ca-115">1</span></span>|<span data-ttu-id="f26ca-116">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="f26ca-116">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="f26ca-117">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="f26ca-117">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="f26ca-118">双面</span><span class="sxs-lookup"><span data-stu-id="f26ca-118">2</span></span>|<span data-ttu-id="f26ca-119">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="f26ca-119">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="f26ca-120">无论</span><span class="sxs-lookup"><span data-stu-id="f26ca-120">anywhere</span></span>|<span data-ttu-id="f26ca-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f26ca-121">3</span></span>|<span data-ttu-id="f26ca-122">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="f26ca-122">Apps from anywhere can be run.</span></span>|





