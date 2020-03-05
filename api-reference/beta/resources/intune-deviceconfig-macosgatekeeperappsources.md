---
title: macOSGatekeeperAppSources 枚举类型
description: MacOS 网关的应用程序源选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7e0990d063d2f50045b3d5de7f4cce4f9f32943b
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526109"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="4ce34-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4ce34-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="4ce34-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4ce34-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4ce34-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4ce34-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4ce34-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4ce34-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4ce34-107">MacOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="4ce34-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="4ce34-108">成员</span><span class="sxs-lookup"><span data-stu-id="4ce34-108">Members</span></span>
|<span data-ttu-id="4ce34-109">成员</span><span class="sxs-lookup"><span data-stu-id="4ce34-109">Member</span></span>|<span data-ttu-id="4ce34-110">值</span><span class="sxs-lookup"><span data-stu-id="4ce34-110">Value</span></span>|<span data-ttu-id="4ce34-111">说明</span><span class="sxs-lookup"><span data-stu-id="4ce34-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4ce34-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="4ce34-112">notConfigured</span></span>|<span data-ttu-id="4ce34-113">0</span><span class="sxs-lookup"><span data-stu-id="4ce34-113">0</span></span>|<span data-ttu-id="4ce34-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="4ce34-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="4ce34-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="4ce34-115">macAppStore</span></span>|<span data-ttu-id="4ce34-116">1 </span><span class="sxs-lookup"><span data-stu-id="4ce34-116">1</span></span>|<span data-ttu-id="4ce34-117">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="4ce34-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="4ce34-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="4ce34-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="4ce34-119">2 </span><span class="sxs-lookup"><span data-stu-id="4ce34-119">2</span></span>|<span data-ttu-id="4ce34-120">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="4ce34-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="4ce34-121">无论</span><span class="sxs-lookup"><span data-stu-id="4ce34-121">anywhere</span></span>|<span data-ttu-id="4ce34-122">3 </span><span class="sxs-lookup"><span data-stu-id="4ce34-122">3</span></span>|<span data-ttu-id="4ce34-123">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="4ce34-123">Apps from anywhere can be run.</span></span>|



