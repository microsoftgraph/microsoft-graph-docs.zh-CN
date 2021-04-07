---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1785f433c604c441072b953a3efae94978d449f4
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51612183"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="13ad4-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="13ad4-103">runState enum type</span></span>

<span data-ttu-id="13ad4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13ad4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13ad4-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="13ad4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="13ad4-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13ad4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13ad4-107">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="13ad4-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="13ad4-108">成员</span><span class="sxs-lookup"><span data-stu-id="13ad4-108">Members</span></span>
|<span data-ttu-id="13ad4-109">成员</span><span class="sxs-lookup"><span data-stu-id="13ad4-109">Member</span></span>|<span data-ttu-id="13ad4-110">值</span><span class="sxs-lookup"><span data-stu-id="13ad4-110">Value</span></span>|<span data-ttu-id="13ad4-111">Description</span><span class="sxs-lookup"><span data-stu-id="13ad4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13ad4-112">unknown</span><span class="sxs-lookup"><span data-stu-id="13ad4-112">unknown</span></span>|<span data-ttu-id="13ad4-113">0</span><span class="sxs-lookup"><span data-stu-id="13ad4-113">0</span></span>|<span data-ttu-id="13ad4-114">结果未知。</span><span class="sxs-lookup"><span data-stu-id="13ad4-114">Unknown result.</span></span>|
|<span data-ttu-id="13ad4-115">success</span><span class="sxs-lookup"><span data-stu-id="13ad4-115">success</span></span>|<span data-ttu-id="13ad4-116">1</span><span class="sxs-lookup"><span data-stu-id="13ad4-116">1</span></span>|<span data-ttu-id="13ad4-117">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="13ad4-117">Script is run successfully.</span></span>|
|<span data-ttu-id="13ad4-118">失败</span><span class="sxs-lookup"><span data-stu-id="13ad4-118">fail</span></span>|<span data-ttu-id="13ad4-119">2</span><span class="sxs-lookup"><span data-stu-id="13ad4-119">2</span></span>|<span data-ttu-id="13ad4-120">脚本无法运行。</span><span class="sxs-lookup"><span data-stu-id="13ad4-120">Script failed to run.</span></span>|
|<span data-ttu-id="13ad4-121">scriptError</span><span class="sxs-lookup"><span data-stu-id="13ad4-121">scriptError</span></span>|<span data-ttu-id="13ad4-122">3</span><span class="sxs-lookup"><span data-stu-id="13ad4-122">3</span></span>|<span data-ttu-id="13ad4-123">发现脚本命中错误。</span><span class="sxs-lookup"><span data-stu-id="13ad4-123">Discovery script hits error.</span></span>|
|<span data-ttu-id="13ad4-124">pending</span><span class="sxs-lookup"><span data-stu-id="13ad4-124">pending</span></span>|<span data-ttu-id="13ad4-125">4 </span><span class="sxs-lookup"><span data-stu-id="13ad4-125">4</span></span>|<span data-ttu-id="13ad4-126">脚本正在等待执行。</span><span class="sxs-lookup"><span data-stu-id="13ad4-126">Script is pending to execute.</span></span>|
|<span data-ttu-id="13ad4-127">notApplicable</span><span class="sxs-lookup"><span data-stu-id="13ad4-127">notApplicable</span></span>|<span data-ttu-id="13ad4-128">5 </span><span class="sxs-lookup"><span data-stu-id="13ad4-128">5</span></span>|<span data-ttu-id="13ad4-129">脚本不适用于此设备。</span><span class="sxs-lookup"><span data-stu-id="13ad4-129">Script is not applicable for this device.</span></span>|




