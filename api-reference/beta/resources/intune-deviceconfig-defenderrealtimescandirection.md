---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b4df7541cc1c3822ddd659d266d152d0edfe67b6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43413079"
---
# <a name="defenderrealtimescandirection-enum-type"></a><span data-ttu-id="82d10-103">defenderRealtimeScanDirection 枚举类型</span><span class="sxs-lookup"><span data-stu-id="82d10-103">defenderRealtimeScanDirection enum type</span></span>

<span data-ttu-id="82d10-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82d10-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82d10-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="82d10-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82d10-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82d10-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82d10-107">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="82d10-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="82d10-108">成员</span><span class="sxs-lookup"><span data-stu-id="82d10-108">Members</span></span>
|<span data-ttu-id="82d10-109">成员</span><span class="sxs-lookup"><span data-stu-id="82d10-109">Member</span></span>|<span data-ttu-id="82d10-110">值</span><span class="sxs-lookup"><span data-stu-id="82d10-110">Value</span></span>|<span data-ttu-id="82d10-111">说明</span><span class="sxs-lookup"><span data-stu-id="82d10-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82d10-112">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="82d10-112">monitorAllFiles</span></span>|<span data-ttu-id="82d10-113">0</span><span class="sxs-lookup"><span data-stu-id="82d10-113">0</span></span>|<span data-ttu-id="82d10-114">0（默认值）–监视所有文件（双向）</span><span class="sxs-lookup"><span data-stu-id="82d10-114">0 (default) – Monitor all files(bi-directional)</span></span>|
|<span data-ttu-id="82d10-115">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="82d10-115">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="82d10-116">1</span><span class="sxs-lookup"><span data-stu-id="82d10-116">1</span></span>|<span data-ttu-id="82d10-117">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="82d10-117">Monitor incoming files only.</span></span>|
|<span data-ttu-id="82d10-118">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="82d10-118">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="82d10-119">双面</span><span class="sxs-lookup"><span data-stu-id="82d10-119">2</span></span>|<span data-ttu-id="82d10-120">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="82d10-120">Monitor outgoing files only.</span></span>|



