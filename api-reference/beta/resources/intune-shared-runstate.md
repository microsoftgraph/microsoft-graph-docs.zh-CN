---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ecf868f77bc5460af95375ef88d73e7384ef4ccf
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538698"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="b88ec-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b88ec-103">runState enum type</span></span>

> <span data-ttu-id="b88ec-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b88ec-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b88ec-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b88ec-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b88ec-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="b88ec-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="b88ec-107">成员</span><span class="sxs-lookup"><span data-stu-id="b88ec-107">Members</span></span>
|<span data-ttu-id="b88ec-108">成员</span><span class="sxs-lookup"><span data-stu-id="b88ec-108">Member</span></span>|<span data-ttu-id="b88ec-109">值</span><span class="sxs-lookup"><span data-stu-id="b88ec-109">Value</span></span>|<span data-ttu-id="b88ec-110">说明</span><span class="sxs-lookup"><span data-stu-id="b88ec-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b88ec-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b88ec-111">unknown</span></span>|<span data-ttu-id="b88ec-112">0</span><span class="sxs-lookup"><span data-stu-id="b88ec-112">0</span></span>|<span data-ttu-id="b88ec-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="b88ec-113">Unknown result.</span></span>|
|<span data-ttu-id="b88ec-114">success</span><span class="sxs-lookup"><span data-stu-id="b88ec-114">success</span></span>|<span data-ttu-id="b88ec-115">1</span><span class="sxs-lookup"><span data-stu-id="b88ec-115">1</span></span>|<span data-ttu-id="b88ec-116">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="b88ec-116">Script is run successfully.</span></span>|
|<span data-ttu-id="b88ec-117">失败</span><span class="sxs-lookup"><span data-stu-id="b88ec-117">fail</span></span>|<span data-ttu-id="b88ec-118">双面</span><span class="sxs-lookup"><span data-stu-id="b88ec-118">2</span></span>|<span data-ttu-id="b88ec-119">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="b88ec-119">Script failed to run.</span></span>|
|<span data-ttu-id="b88ec-120">scriptError</span><span class="sxs-lookup"><span data-stu-id="b88ec-120">scriptError</span></span>|<span data-ttu-id="b88ec-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b88ec-121">3</span></span>|<span data-ttu-id="b88ec-122">发现脚本命中错误。</span><span class="sxs-lookup"><span data-stu-id="b88ec-122">Discovery script hits error.</span></span>|
|<span data-ttu-id="b88ec-123">决</span><span class="sxs-lookup"><span data-stu-id="b88ec-123">pending</span></span>|<span data-ttu-id="b88ec-124">4 </span><span class="sxs-lookup"><span data-stu-id="b88ec-124">4</span></span>|<span data-ttu-id="b88ec-125">脚本正在挂起中执行。</span><span class="sxs-lookup"><span data-stu-id="b88ec-125">Script is pending to execute.</span></span>|
|<span data-ttu-id="b88ec-126">notApplicable</span><span class="sxs-lookup"><span data-stu-id="b88ec-126">notApplicable</span></span>|<span data-ttu-id="b88ec-127">5 </span><span class="sxs-lookup"><span data-stu-id="b88ec-127">5</span></span>|<span data-ttu-id="b88ec-128">脚本不适用于此设备。</span><span class="sxs-lookup"><span data-stu-id="b88ec-128">Script is not applicable for this device.</span></span>|



