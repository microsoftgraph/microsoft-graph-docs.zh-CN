---
title: macOSGatekeeperAppSources 枚举类型
description: MacOS 网关的应用程序源选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 550f10e1484dc0d159712a2c6fc2132c6565628c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48724563"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="dab00-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dab00-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="dab00-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dab00-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dab00-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dab00-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dab00-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dab00-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dab00-107">MacOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="dab00-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="dab00-108">成员</span><span class="sxs-lookup"><span data-stu-id="dab00-108">Members</span></span>
|<span data-ttu-id="dab00-109">成员</span><span class="sxs-lookup"><span data-stu-id="dab00-109">Member</span></span>|<span data-ttu-id="dab00-110">值</span><span class="sxs-lookup"><span data-stu-id="dab00-110">Value</span></span>|<span data-ttu-id="dab00-111">说明</span><span class="sxs-lookup"><span data-stu-id="dab00-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dab00-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="dab00-112">notConfigured</span></span>|<span data-ttu-id="dab00-113">0</span><span class="sxs-lookup"><span data-stu-id="dab00-113">0</span></span>|<span data-ttu-id="dab00-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="dab00-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="dab00-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="dab00-115">macAppStore</span></span>|<span data-ttu-id="dab00-116">1</span><span class="sxs-lookup"><span data-stu-id="dab00-116">1</span></span>|<span data-ttu-id="dab00-117">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="dab00-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="dab00-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="dab00-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="dab00-119">双面</span><span class="sxs-lookup"><span data-stu-id="dab00-119">2</span></span>|<span data-ttu-id="dab00-120">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="dab00-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="dab00-121">无论</span><span class="sxs-lookup"><span data-stu-id="dab00-121">anywhere</span></span>|<span data-ttu-id="dab00-122">第三章</span><span class="sxs-lookup"><span data-stu-id="dab00-122">3</span></span>|<span data-ttu-id="dab00-123">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="dab00-123">Apps from anywhere can be run.</span></span>|





