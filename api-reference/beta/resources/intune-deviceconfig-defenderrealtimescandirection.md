---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0256c756be59b1b3661360d4c952a385fd5c6348
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526869"
---
# <a name="defenderrealtimescandirection-enum-type"></a><span data-ttu-id="4be1c-103">defenderRealtimeScanDirection 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4be1c-103">defenderRealtimeScanDirection enum type</span></span>

<span data-ttu-id="4be1c-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="4be1c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4be1c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4be1c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4be1c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4be1c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4be1c-107">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="4be1c-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="4be1c-108">成员</span><span class="sxs-lookup"><span data-stu-id="4be1c-108">Members</span></span>
|<span data-ttu-id="4be1c-109">成员</span><span class="sxs-lookup"><span data-stu-id="4be1c-109">Member</span></span>|<span data-ttu-id="4be1c-110">值</span><span class="sxs-lookup"><span data-stu-id="4be1c-110">Value</span></span>|<span data-ttu-id="4be1c-111">说明</span><span class="sxs-lookup"><span data-stu-id="4be1c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4be1c-112">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="4be1c-112">monitorAllFiles</span></span>|<span data-ttu-id="4be1c-113">0</span><span class="sxs-lookup"><span data-stu-id="4be1c-113">0</span></span>|<span data-ttu-id="4be1c-114">0（默认值）–监视所有文件（双向）</span><span class="sxs-lookup"><span data-stu-id="4be1c-114">0 (default) – Monitor all files(bi-directional)</span></span>|
|<span data-ttu-id="4be1c-115">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="4be1c-115">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="4be1c-116">1 </span><span class="sxs-lookup"><span data-stu-id="4be1c-116">1</span></span>|<span data-ttu-id="4be1c-117">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="4be1c-117">Monitor incoming files only.</span></span>|
|<span data-ttu-id="4be1c-118">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="4be1c-118">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="4be1c-119">2 </span><span class="sxs-lookup"><span data-stu-id="4be1c-119">2</span></span>|<span data-ttu-id="4be1c-120">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="4be1c-120">Monitor outgoing files only.</span></span>|



