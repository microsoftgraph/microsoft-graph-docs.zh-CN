---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c53847d270639d11b5014291e62dde2668a4d5
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255998"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="f54ea-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f54ea-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="f54ea-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f54ea-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f54ea-105">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="f54ea-105">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="f54ea-106">成员</span><span class="sxs-lookup"><span data-stu-id="f54ea-106">Members</span></span>
|<span data-ttu-id="f54ea-107">成员</span><span class="sxs-lookup"><span data-stu-id="f54ea-107">Member</span></span>|<span data-ttu-id="f54ea-108">值</span><span class="sxs-lookup"><span data-stu-id="f54ea-108">Value</span></span>|<span data-ttu-id="f54ea-109">说明</span><span class="sxs-lookup"><span data-stu-id="f54ea-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f54ea-110">定制</span><span class="sxs-lookup"><span data-stu-id="f54ea-110">userDefined</span></span>|<span data-ttu-id="f54ea-111">0</span><span class="sxs-lookup"><span data-stu-id="f54ea-111">0</span></span>|<span data-ttu-id="f54ea-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="f54ea-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="f54ea-113">启用</span><span class="sxs-lookup"><span data-stu-id="f54ea-113">disable</span></span>|<span data-ttu-id="f54ea-114">1</span><span class="sxs-lookup"><span data-stu-id="f54ea-114">1</span></span>|<span data-ttu-id="f54ea-115">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="f54ea-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="f54ea-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="f54ea-116">monitorAllFiles</span></span>|<span data-ttu-id="f54ea-117">双面</span><span class="sxs-lookup"><span data-stu-id="f54ea-117">2</span></span>|<span data-ttu-id="f54ea-118">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="f54ea-118">Monitor all files.</span></span>|
|<span data-ttu-id="f54ea-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="f54ea-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="f54ea-120">第三章</span><span class="sxs-lookup"><span data-stu-id="f54ea-120">3</span></span>| <span data-ttu-id="f54ea-121">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="f54ea-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="f54ea-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="f54ea-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="f54ea-123">4</span><span class="sxs-lookup"><span data-stu-id="f54ea-123">4</span></span>|<span data-ttu-id="f54ea-124">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="f54ea-124">Monitor outgoing files only.</span></span>|



