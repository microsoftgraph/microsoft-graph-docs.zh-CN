---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8f4c1605734afef3caefc4b51e2c8a826d2f2cd4
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42767818"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="3cace-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3cace-103">runState enum type</span></span>

> <span data-ttu-id="3cace-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3cace-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3cace-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3cace-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3cace-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="3cace-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="3cace-107">成员</span><span class="sxs-lookup"><span data-stu-id="3cace-107">Members</span></span>
|<span data-ttu-id="3cace-108">成员</span><span class="sxs-lookup"><span data-stu-id="3cace-108">Member</span></span>|<span data-ttu-id="3cace-109">值</span><span class="sxs-lookup"><span data-stu-id="3cace-109">Value</span></span>|<span data-ttu-id="3cace-110">说明</span><span class="sxs-lookup"><span data-stu-id="3cace-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3cace-111">unknown</span><span class="sxs-lookup"><span data-stu-id="3cace-111">unknown</span></span>|<span data-ttu-id="3cace-112">0</span><span class="sxs-lookup"><span data-stu-id="3cace-112">0</span></span>|<span data-ttu-id="3cace-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="3cace-113">Unknown result.</span></span>|
|<span data-ttu-id="3cace-114">success</span><span class="sxs-lookup"><span data-stu-id="3cace-114">success</span></span>|<span data-ttu-id="3cace-115">1</span><span class="sxs-lookup"><span data-stu-id="3cace-115">1</span></span>|<span data-ttu-id="3cace-116">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="3cace-116">Script is run successfully.</span></span>|
|<span data-ttu-id="3cace-117">失败</span><span class="sxs-lookup"><span data-stu-id="3cace-117">fail</span></span>|<span data-ttu-id="3cace-118">双面</span><span class="sxs-lookup"><span data-stu-id="3cace-118">2</span></span>|<span data-ttu-id="3cace-119">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="3cace-119">Script failed to run.</span></span>|
|<span data-ttu-id="3cace-120">scriptError</span><span class="sxs-lookup"><span data-stu-id="3cace-120">scriptError</span></span>|<span data-ttu-id="3cace-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3cace-121">3</span></span>|<span data-ttu-id="3cace-122">发现脚本命中错误。</span><span class="sxs-lookup"><span data-stu-id="3cace-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="3cace-123">决</span><span class="sxs-lookup"><span data-stu-id="3cace-123">pending</span></span>|<span data-ttu-id="3cace-124">4 </span><span class="sxs-lookup"><span data-stu-id="3cace-124">4</span></span>|<span data-ttu-id="3cace-125">脚本正在挂起中执行。</span><span class="sxs-lookup"><span data-stu-id="3cace-125">Script is pending to execute.</span></span>|
|<span data-ttu-id="3cace-126">notApplicable</span><span class="sxs-lookup"><span data-stu-id="3cace-126">notApplicable</span></span>|<span data-ttu-id="3cace-127">5 </span><span class="sxs-lookup"><span data-stu-id="3cace-127">5</span></span>|<span data-ttu-id="3cace-128">脚本不适用于此设备。</span><span class="sxs-lookup"><span data-stu-id="3cace-128">Script is not applicable for this device.</span></span>|



