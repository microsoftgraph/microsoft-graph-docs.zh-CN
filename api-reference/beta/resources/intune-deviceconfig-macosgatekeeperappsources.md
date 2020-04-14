---
title: macOSGatekeeperAppSources 枚举类型
description: MacOS 网关的应用程序源选项。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 53e98d727f2c90d830b66106d3376564e6c89116
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43464133"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="6cb6a-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6cb6a-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="6cb6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6cb6a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6cb6a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6cb6a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6cb6a-107">MacOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="6cb6a-108">成员</span><span class="sxs-lookup"><span data-stu-id="6cb6a-108">Members</span></span>
|<span data-ttu-id="6cb6a-109">成员</span><span class="sxs-lookup"><span data-stu-id="6cb6a-109">Member</span></span>|<span data-ttu-id="6cb6a-110">值</span><span class="sxs-lookup"><span data-stu-id="6cb6a-110">Value</span></span>|<span data-ttu-id="6cb6a-111">说明</span><span class="sxs-lookup"><span data-stu-id="6cb6a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cb6a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="6cb6a-112">notConfigured</span></span>|<span data-ttu-id="6cb6a-113">0</span><span class="sxs-lookup"><span data-stu-id="6cb6a-113">0</span></span>|<span data-ttu-id="6cb6a-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="6cb6a-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="6cb6a-115">macAppStore</span></span>|<span data-ttu-id="6cb6a-116">1</span><span class="sxs-lookup"><span data-stu-id="6cb6a-116">1</span></span>|<span data-ttu-id="6cb6a-117">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="6cb6a-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="6cb6a-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="6cb6a-119">双面</span><span class="sxs-lookup"><span data-stu-id="6cb6a-119">2</span></span>|<span data-ttu-id="6cb6a-120">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="6cb6a-121">无论</span><span class="sxs-lookup"><span data-stu-id="6cb6a-121">anywhere</span></span>|<span data-ttu-id="6cb6a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="6cb6a-122">3</span></span>|<span data-ttu-id="6cb6a-123">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="6cb6a-123">Apps from anywhere can be run.</span></span>|



