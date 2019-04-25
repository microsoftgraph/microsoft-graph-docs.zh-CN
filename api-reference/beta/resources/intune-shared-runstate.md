---
title: runState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 706ef0d5ea87796c951d2fcb8c7357643fba7afb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522585"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="b4c7d-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4c7d-103">runState enum type</span></span>

> <span data-ttu-id="b4c7d-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4c7d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4c7d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4c7d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4c7d-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="b4c7d-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="b4c7d-107">成员</span><span class="sxs-lookup"><span data-stu-id="b4c7d-107">Members</span></span>
|<span data-ttu-id="b4c7d-108">成员</span><span class="sxs-lookup"><span data-stu-id="b4c7d-108">Member</span></span>|<span data-ttu-id="b4c7d-109">值</span><span class="sxs-lookup"><span data-stu-id="b4c7d-109">Value</span></span>|<span data-ttu-id="b4c7d-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4c7d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4c7d-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b4c7d-111">unknown</span></span>|<span data-ttu-id="b4c7d-112">0</span><span class="sxs-lookup"><span data-stu-id="b4c7d-112">0</span></span>|<span data-ttu-id="b4c7d-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="b4c7d-113">Unknown result.</span></span>|
|<span data-ttu-id="b4c7d-114">success</span><span class="sxs-lookup"><span data-stu-id="b4c7d-114">success</span></span>|<span data-ttu-id="b4c7d-115">1</span><span class="sxs-lookup"><span data-stu-id="b4c7d-115">1</span></span>|<span data-ttu-id="b4c7d-116">脚本成功运行。</span><span class="sxs-lookup"><span data-stu-id="b4c7d-116">Script is run successfully.</span></span>|
|<span data-ttu-id="b4c7d-117">失败</span><span class="sxs-lookup"><span data-stu-id="b4c7d-117">fail</span></span>|<span data-ttu-id="b4c7d-118">2 </span><span class="sxs-lookup"><span data-stu-id="b4c7d-118">2</span></span>|<span data-ttu-id="b4c7d-119">脚本运行失败。</span><span class="sxs-lookup"><span data-stu-id="b4c7d-119">Script failed to run.</span></span>|




