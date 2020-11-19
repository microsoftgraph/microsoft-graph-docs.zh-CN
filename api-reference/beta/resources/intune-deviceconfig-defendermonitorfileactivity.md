---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 61a8c80f0e3c01c213e1dacb625b58f854756673
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256517"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="5d312-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5d312-103">defenderMonitorFileActivity enum type</span></span>

<span data-ttu-id="5d312-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5d312-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5d312-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5d312-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5d312-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5d312-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5d312-107">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="5d312-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="5d312-108">成员</span><span class="sxs-lookup"><span data-stu-id="5d312-108">Members</span></span>
|<span data-ttu-id="5d312-109">成员</span><span class="sxs-lookup"><span data-stu-id="5d312-109">Member</span></span>|<span data-ttu-id="5d312-110">值</span><span class="sxs-lookup"><span data-stu-id="5d312-110">Value</span></span>|<span data-ttu-id="5d312-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d312-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d312-112">定制</span><span class="sxs-lookup"><span data-stu-id="5d312-112">userDefined</span></span>|<span data-ttu-id="5d312-113">0</span><span class="sxs-lookup"><span data-stu-id="5d312-113">0</span></span>|<span data-ttu-id="5d312-114">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="5d312-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5d312-115">disable</span><span class="sxs-lookup"><span data-stu-id="5d312-115">disable</span></span>|<span data-ttu-id="5d312-116">1</span><span class="sxs-lookup"><span data-stu-id="5d312-116">1</span></span>|<span data-ttu-id="5d312-117">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="5d312-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="5d312-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="5d312-118">monitorAllFiles</span></span>|<span data-ttu-id="5d312-119">双面</span><span class="sxs-lookup"><span data-stu-id="5d312-119">2</span></span>|<span data-ttu-id="5d312-120">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="5d312-120">Monitor all files.</span></span>|
|<span data-ttu-id="5d312-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="5d312-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="5d312-122">第三章</span><span class="sxs-lookup"><span data-stu-id="5d312-122">3</span></span>| <span data-ttu-id="5d312-123">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="5d312-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="5d312-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="5d312-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="5d312-125">4 </span><span class="sxs-lookup"><span data-stu-id="5d312-125">4</span></span>|<span data-ttu-id="5d312-126">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="5d312-126">Monitor outgoing files only.</span></span>|




