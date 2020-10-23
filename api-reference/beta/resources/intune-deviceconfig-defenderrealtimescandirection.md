---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1fe80eb0df800cb0439497a6603448e942c8dc27
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48696326"
---
# <a name="defenderrealtimescandirection-enum-type"></a><span data-ttu-id="65ec7-103">defenderRealtimeScanDirection 枚举类型</span><span class="sxs-lookup"><span data-stu-id="65ec7-103">defenderRealtimeScanDirection enum type</span></span>

<span data-ttu-id="65ec7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65ec7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65ec7-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65ec7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65ec7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65ec7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65ec7-107">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="65ec7-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="65ec7-108">成员</span><span class="sxs-lookup"><span data-stu-id="65ec7-108">Members</span></span>
|<span data-ttu-id="65ec7-109">成员</span><span class="sxs-lookup"><span data-stu-id="65ec7-109">Member</span></span>|<span data-ttu-id="65ec7-110">值</span><span class="sxs-lookup"><span data-stu-id="65ec7-110">Value</span></span>|<span data-ttu-id="65ec7-111">说明</span><span class="sxs-lookup"><span data-stu-id="65ec7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65ec7-112">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="65ec7-112">monitorAllFiles</span></span>|<span data-ttu-id="65ec7-113">0</span><span class="sxs-lookup"><span data-stu-id="65ec7-113">0</span></span>|<span data-ttu-id="65ec7-114">0 (默认) –监视所有文件 (双向) </span><span class="sxs-lookup"><span data-stu-id="65ec7-114">0 (default) – Monitor all files(bi-directional)</span></span>|
|<span data-ttu-id="65ec7-115">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="65ec7-115">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="65ec7-116">1</span><span class="sxs-lookup"><span data-stu-id="65ec7-116">1</span></span>|<span data-ttu-id="65ec7-117">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="65ec7-117">Monitor incoming files only.</span></span>|
|<span data-ttu-id="65ec7-118">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="65ec7-118">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="65ec7-119">双面</span><span class="sxs-lookup"><span data-stu-id="65ec7-119">2</span></span>|<span data-ttu-id="65ec7-120">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="65ec7-120">Monitor outgoing files only.</span></span>|





