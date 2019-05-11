---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 093af5b16854bf65699e469b1afd47fe6b990375
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33939838"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="03544-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="03544-103">runState enum type</span></span>

> <span data-ttu-id="03544-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03544-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03544-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03544-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03544-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="03544-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="03544-107">成员</span><span class="sxs-lookup"><span data-stu-id="03544-107">Members</span></span>
|<span data-ttu-id="03544-108">成员</span><span class="sxs-lookup"><span data-stu-id="03544-108">Member</span></span>|<span data-ttu-id="03544-109">值</span><span class="sxs-lookup"><span data-stu-id="03544-109">Value</span></span>|<span data-ttu-id="03544-110">说明</span><span class="sxs-lookup"><span data-stu-id="03544-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03544-111">unknown</span><span class="sxs-lookup"><span data-stu-id="03544-111">unknown</span></span>|<span data-ttu-id="03544-112">0</span><span class="sxs-lookup"><span data-stu-id="03544-112">0</span></span>|<span data-ttu-id="03544-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="03544-113">Unknown result.</span></span>|
|<span data-ttu-id="03544-114">success</span><span class="sxs-lookup"><span data-stu-id="03544-114">success</span></span>|<span data-ttu-id="03544-115">1</span><span class="sxs-lookup"><span data-stu-id="03544-115">1</span></span>|<span data-ttu-id="03544-116">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="03544-116">Script is run successfully.</span></span>|
|<span data-ttu-id="03544-117">失败</span><span class="sxs-lookup"><span data-stu-id="03544-117">fail</span></span>|<span data-ttu-id="03544-118">双面</span><span class="sxs-lookup"><span data-stu-id="03544-118">2</span></span>|<span data-ttu-id="03544-119">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="03544-119">Script failed to run.</span></span>|




