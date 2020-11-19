---
title: macOSGatekeeperAppSources 枚举类型
description: MacOS 网关的应用程序源选项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9a886155056a8ef689f37497f735ada345316a70
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49279862"
---
# <a name="macosgatekeeperappsources-enum-type"></a><span data-ttu-id="c57f4-103">macOSGatekeeperAppSources 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c57f4-103">macOSGatekeeperAppSources enum type</span></span>

<span data-ttu-id="c57f4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c57f4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c57f4-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c57f4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c57f4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c57f4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c57f4-107">MacOS 网关的应用程序源选项。</span><span class="sxs-lookup"><span data-stu-id="c57f4-107">App source options for macOS Gatekeeper.</span></span>

## <a name="members"></a><span data-ttu-id="c57f4-108">成员</span><span class="sxs-lookup"><span data-stu-id="c57f4-108">Members</span></span>
|<span data-ttu-id="c57f4-109">成员</span><span class="sxs-lookup"><span data-stu-id="c57f4-109">Member</span></span>|<span data-ttu-id="c57f4-110">值</span><span class="sxs-lookup"><span data-stu-id="c57f4-110">Value</span></span>|<span data-ttu-id="c57f4-111">说明</span><span class="sxs-lookup"><span data-stu-id="c57f4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c57f4-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c57f4-112">notConfigured</span></span>|<span data-ttu-id="c57f4-113">0</span><span class="sxs-lookup"><span data-stu-id="c57f4-113">0</span></span>|<span data-ttu-id="c57f4-114">设备默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="c57f4-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="c57f4-115">macAppStore</span><span class="sxs-lookup"><span data-stu-id="c57f4-115">macAppStore</span></span>|<span data-ttu-id="c57f4-116">1</span><span class="sxs-lookup"><span data-stu-id="c57f4-116">1</span></span>|<span data-ttu-id="c57f4-117">只有 Mac AppStore 中的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="c57f4-117">Only apps from the Mac AppStore can be run.</span></span>|
|<span data-ttu-id="c57f4-118">macAppStoreAndIdentifiedDevelopers</span><span class="sxs-lookup"><span data-stu-id="c57f4-118">macAppStoreAndIdentifiedDevelopers</span></span>|<span data-ttu-id="c57f4-119">双面</span><span class="sxs-lookup"><span data-stu-id="c57f4-119">2</span></span>|<span data-ttu-id="c57f4-120">只有 Mac AppStore 和已确定的开发人员的应用可以运行。</span><span class="sxs-lookup"><span data-stu-id="c57f4-120">Only apps from the Mac AppStore and identified developers can be run.</span></span>|
|<span data-ttu-id="c57f4-121">无论</span><span class="sxs-lookup"><span data-stu-id="c57f4-121">anywhere</span></span>|<span data-ttu-id="c57f4-122">第三章</span><span class="sxs-lookup"><span data-stu-id="c57f4-122">3</span></span>|<span data-ttu-id="c57f4-123">可以从任意位置运行应用程序。</span><span class="sxs-lookup"><span data-stu-id="c57f4-123">Apps from anywhere can be run.</span></span>|




