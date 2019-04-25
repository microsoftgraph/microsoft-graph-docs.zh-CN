---
title: healthState 枚举类型
description: 指示 Windows management 应用的运行状况状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6192b7785f751521ebcee676905cf3426ad4145
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32522186"
---
# <a name="healthstate-enum-type"></a><span data-ttu-id="b4d53-103">healthState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b4d53-103">healthState enum type</span></span>

> <span data-ttu-id="b4d53-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4d53-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4d53-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4d53-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4d53-106">指示 Windows management 应用的运行状况状态。</span><span class="sxs-lookup"><span data-stu-id="b4d53-106">Indicates health state of the Windows management app.</span></span>

## <a name="members"></a><span data-ttu-id="b4d53-107">成员</span><span class="sxs-lookup"><span data-stu-id="b4d53-107">Members</span></span>
|<span data-ttu-id="b4d53-108">成员</span><span class="sxs-lookup"><span data-stu-id="b4d53-108">Member</span></span>|<span data-ttu-id="b4d53-109">值</span><span class="sxs-lookup"><span data-stu-id="b4d53-109">Value</span></span>|<span data-ttu-id="b4d53-110">说明</span><span class="sxs-lookup"><span data-stu-id="b4d53-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b4d53-111">unknown</span><span class="sxs-lookup"><span data-stu-id="b4d53-111">unknown</span></span>|<span data-ttu-id="b4d53-112">0</span><span class="sxs-lookup"><span data-stu-id="b4d53-112">0</span></span>|<span data-ttu-id="b4d53-113">未知状态。</span><span class="sxs-lookup"><span data-stu-id="b4d53-113">Unknown state.</span></span>|
|<span data-ttu-id="b4d53-114">运转</span><span class="sxs-lookup"><span data-stu-id="b4d53-114">healthy</span></span>|<span data-ttu-id="b4d53-115">1</span><span class="sxs-lookup"><span data-stu-id="b4d53-115">1</span></span>|<span data-ttu-id="b4d53-116">正常状态。</span><span class="sxs-lookup"><span data-stu-id="b4d53-116">Healthy state.</span></span>|
|<span data-ttu-id="b4d53-117">正常</span><span class="sxs-lookup"><span data-stu-id="b4d53-117">unhealthy</span></span>|<span data-ttu-id="b4d53-118">2 </span><span class="sxs-lookup"><span data-stu-id="b4d53-118">2</span></span>|<span data-ttu-id="b4d53-119">不正常状态。</span><span class="sxs-lookup"><span data-stu-id="b4d53-119">Unhealthy state.</span></span>|





