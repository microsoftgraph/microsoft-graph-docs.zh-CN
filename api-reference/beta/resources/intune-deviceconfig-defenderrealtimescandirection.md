---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c7568470ec57e25ab3f8562629273d26f2ee0381
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794443"
---
# <a name="defenderrealtimescandirection-enum-type"></a><span data-ttu-id="1993a-103">defenderRealtimeScanDirection 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1993a-103">defenderRealtimeScanDirection enum type</span></span>

> <span data-ttu-id="1993a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1993a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1993a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1993a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1993a-106">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="1993a-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="1993a-107">成员</span><span class="sxs-lookup"><span data-stu-id="1993a-107">Members</span></span>
|<span data-ttu-id="1993a-108">成员</span><span class="sxs-lookup"><span data-stu-id="1993a-108">Member</span></span>|<span data-ttu-id="1993a-109">值</span><span class="sxs-lookup"><span data-stu-id="1993a-109">Value</span></span>|<span data-ttu-id="1993a-110">说明</span><span class="sxs-lookup"><span data-stu-id="1993a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1993a-111">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="1993a-111">monitorAllFiles</span></span>|<span data-ttu-id="1993a-112">0</span><span class="sxs-lookup"><span data-stu-id="1993a-112">0</span></span>|<span data-ttu-id="1993a-113">0（默认值）–监视所有文件（双向）</span><span class="sxs-lookup"><span data-stu-id="1993a-113">0 (default) – Monitor all files(bi-directional)</span></span>|
|<span data-ttu-id="1993a-114">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="1993a-114">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="1993a-115">1</span><span class="sxs-lookup"><span data-stu-id="1993a-115">1</span></span>|<span data-ttu-id="1993a-116">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="1993a-116">Monitor incoming files only.</span></span>|
|<span data-ttu-id="1993a-117">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="1993a-117">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="1993a-118">双面</span><span class="sxs-lookup"><span data-stu-id="1993a-118">2</span></span>|<span data-ttu-id="1993a-119">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="1993a-119">Monitor outgoing files only.</span></span>|



