---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 43912d24663f21281058636d3eb8a3811b6dbfa0
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34986268"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="c9cd1-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c9cd1-103">runState enum type</span></span>

> <span data-ttu-id="c9cd1-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c9cd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9cd1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c9cd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9cd1-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="c9cd1-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="c9cd1-107">成员</span><span class="sxs-lookup"><span data-stu-id="c9cd1-107">Members</span></span>
|<span data-ttu-id="c9cd1-108">成员</span><span class="sxs-lookup"><span data-stu-id="c9cd1-108">Member</span></span>|<span data-ttu-id="c9cd1-109">值</span><span class="sxs-lookup"><span data-stu-id="c9cd1-109">Value</span></span>|<span data-ttu-id="c9cd1-110">说明</span><span class="sxs-lookup"><span data-stu-id="c9cd1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9cd1-111">unknown</span><span class="sxs-lookup"><span data-stu-id="c9cd1-111">unknown</span></span>|<span data-ttu-id="c9cd1-112">0</span><span class="sxs-lookup"><span data-stu-id="c9cd1-112">0</span></span>|<span data-ttu-id="c9cd1-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="c9cd1-113">Unknown result.</span></span>|
|<span data-ttu-id="c9cd1-114">success</span><span class="sxs-lookup"><span data-stu-id="c9cd1-114">success</span></span>|<span data-ttu-id="c9cd1-115">1</span><span class="sxs-lookup"><span data-stu-id="c9cd1-115">1</span></span>|<span data-ttu-id="c9cd1-116">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="c9cd1-116">Script is run successfully.</span></span>|
|<span data-ttu-id="c9cd1-117">失败</span><span class="sxs-lookup"><span data-stu-id="c9cd1-117">fail</span></span>|<span data-ttu-id="c9cd1-118">双面</span><span class="sxs-lookup"><span data-stu-id="c9cd1-118">2</span></span>|<span data-ttu-id="c9cd1-119">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="c9cd1-119">Script failed to run.</span></span>|





