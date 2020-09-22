---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 93a9bcd2d76008f1113c755e904e1141003ee553
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48024310"
---
# <a name="defenderrealtimescandirection-enum-type"></a><span data-ttu-id="f491f-103">defenderRealtimeScanDirection 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f491f-103">defenderRealtimeScanDirection enum type</span></span>

<span data-ttu-id="f491f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f491f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f491f-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f491f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f491f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f491f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f491f-107">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="f491f-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="f491f-108">成员</span><span class="sxs-lookup"><span data-stu-id="f491f-108">Members</span></span>
|<span data-ttu-id="f491f-109">成员</span><span class="sxs-lookup"><span data-stu-id="f491f-109">Member</span></span>|<span data-ttu-id="f491f-110">值</span><span class="sxs-lookup"><span data-stu-id="f491f-110">Value</span></span>|<span data-ttu-id="f491f-111">说明</span><span class="sxs-lookup"><span data-stu-id="f491f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f491f-112">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="f491f-112">monitorAllFiles</span></span>|<span data-ttu-id="f491f-113">0</span><span class="sxs-lookup"><span data-stu-id="f491f-113">0</span></span>|<span data-ttu-id="f491f-114">0 (默认) –监视所有文件 (双向) </span><span class="sxs-lookup"><span data-stu-id="f491f-114">0 (default) – Monitor all files(bi-directional)</span></span>|
|<span data-ttu-id="f491f-115">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="f491f-115">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="f491f-116">1 </span><span class="sxs-lookup"><span data-stu-id="f491f-116">1</span></span>|<span data-ttu-id="f491f-117">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="f491f-117">Monitor incoming files only.</span></span>|
|<span data-ttu-id="f491f-118">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="f491f-118">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="f491f-119">2 </span><span class="sxs-lookup"><span data-stu-id="f491f-119">2</span></span>|<span data-ttu-id="f491f-120">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="f491f-120">Monitor outgoing files only.</span></span>|






