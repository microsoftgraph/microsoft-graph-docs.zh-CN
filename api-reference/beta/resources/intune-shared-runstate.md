---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ec8d3f9333393b946539d639c9cc9eeb30c6b027
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725153"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="f45f0-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f45f0-103">runState enum type</span></span>

<span data-ttu-id="f45f0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f45f0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f45f0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f45f0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f45f0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f45f0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f45f0-107">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="f45f0-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="f45f0-108">成员</span><span class="sxs-lookup"><span data-stu-id="f45f0-108">Members</span></span>
|<span data-ttu-id="f45f0-109">成员</span><span class="sxs-lookup"><span data-stu-id="f45f0-109">Member</span></span>|<span data-ttu-id="f45f0-110">值</span><span class="sxs-lookup"><span data-stu-id="f45f0-110">Value</span></span>|<span data-ttu-id="f45f0-111">说明</span><span class="sxs-lookup"><span data-stu-id="f45f0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f45f0-112">unknown</span><span class="sxs-lookup"><span data-stu-id="f45f0-112">unknown</span></span>|<span data-ttu-id="f45f0-113">0</span><span class="sxs-lookup"><span data-stu-id="f45f0-113">0</span></span>|<span data-ttu-id="f45f0-114">未知结果。</span><span class="sxs-lookup"><span data-stu-id="f45f0-114">Unknown result.</span></span>|
|<span data-ttu-id="f45f0-115">success</span><span class="sxs-lookup"><span data-stu-id="f45f0-115">success</span></span>|<span data-ttu-id="f45f0-116">1</span><span class="sxs-lookup"><span data-stu-id="f45f0-116">1</span></span>|<span data-ttu-id="f45f0-117">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="f45f0-117">Script is run successfully.</span></span>|
|<span data-ttu-id="f45f0-118">失败</span><span class="sxs-lookup"><span data-stu-id="f45f0-118">fail</span></span>|<span data-ttu-id="f45f0-119">双面</span><span class="sxs-lookup"><span data-stu-id="f45f0-119">2</span></span>|<span data-ttu-id="f45f0-120">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="f45f0-120">Script failed to run.</span></span>|
|<span data-ttu-id="f45f0-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="f45f0-121">scriptError</span></span>|<span data-ttu-id="f45f0-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f45f0-122">3</span></span>|<span data-ttu-id="f45f0-123">发现脚本命中错误。</span><span class="sxs-lookup"><span data-stu-id="f45f0-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="f45f0-124">决</span><span class="sxs-lookup"><span data-stu-id="f45f0-124">pending</span></span>|<span data-ttu-id="f45f0-125">4 </span><span class="sxs-lookup"><span data-stu-id="f45f0-125">4</span></span>|<span data-ttu-id="f45f0-126">脚本正在挂起中执行。</span><span class="sxs-lookup"><span data-stu-id="f45f0-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="f45f0-127">notApplicable</span><span class="sxs-lookup"><span data-stu-id="f45f0-127">notApplicable</span></span>|<span data-ttu-id="f45f0-128">5 </span><span class="sxs-lookup"><span data-stu-id="f45f0-128">5</span></span>|<span data-ttu-id="f45f0-129">脚本不适用于此设备。</span><span class="sxs-lookup"><span data-stu-id="f45f0-129">Script is not applicable for this device.</span></span>|





