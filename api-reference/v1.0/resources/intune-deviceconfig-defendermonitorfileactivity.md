---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 39c53847d270639d11b5014291e62dde2668a4d5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32534379"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="946b7-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="946b7-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="946b7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="946b7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="946b7-105">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="946b7-105">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="946b7-106">成员</span><span class="sxs-lookup"><span data-stu-id="946b7-106">Members</span></span>
|<span data-ttu-id="946b7-107">成员</span><span class="sxs-lookup"><span data-stu-id="946b7-107">Member</span></span>|<span data-ttu-id="946b7-108">值</span><span class="sxs-lookup"><span data-stu-id="946b7-108">Value</span></span>|<span data-ttu-id="946b7-109">说明</span><span class="sxs-lookup"><span data-stu-id="946b7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="946b7-110">定制</span><span class="sxs-lookup"><span data-stu-id="946b7-110">userDefined</span></span>|<span data-ttu-id="946b7-111">0</span><span class="sxs-lookup"><span data-stu-id="946b7-111">0</span></span>|<span data-ttu-id="946b7-112">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="946b7-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="946b7-113">disable</span><span class="sxs-lookup"><span data-stu-id="946b7-113">disable</span></span>|<span data-ttu-id="946b7-114">1</span><span class="sxs-lookup"><span data-stu-id="946b7-114">1</span></span>|<span data-ttu-id="946b7-115">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="946b7-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="946b7-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="946b7-116">monitorAllFiles</span></span>|<span data-ttu-id="946b7-117">2 </span><span class="sxs-lookup"><span data-stu-id="946b7-117">2</span></span>|<span data-ttu-id="946b7-118">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="946b7-118">Monitor all files.</span></span>|
|<span data-ttu-id="946b7-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="946b7-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="946b7-120">3 </span><span class="sxs-lookup"><span data-stu-id="946b7-120">3</span></span>| <span data-ttu-id="946b7-121">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="946b7-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="946b7-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="946b7-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="946b7-123">4 </span><span class="sxs-lookup"><span data-stu-id="946b7-123">4</span></span>|<span data-ttu-id="946b7-124">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="946b7-124">Monitor outgoing files only.</span></span>|



