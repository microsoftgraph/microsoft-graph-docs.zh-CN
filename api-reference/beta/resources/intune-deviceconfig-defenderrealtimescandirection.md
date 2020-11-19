---
title: defenderRealtimeScanDirection 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 014602e4602c0b50f10e9b0b673767bbc41db5d0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49256396"
---
# <a name="defenderrealtimescandirection-enum-type"></a><span data-ttu-id="90702-103">defenderRealtimeScanDirection 枚举类型</span><span class="sxs-lookup"><span data-stu-id="90702-103">defenderRealtimeScanDirection enum type</span></span>

<span data-ttu-id="90702-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="90702-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="90702-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90702-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90702-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90702-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90702-107">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="90702-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="90702-108">成员</span><span class="sxs-lookup"><span data-stu-id="90702-108">Members</span></span>
|<span data-ttu-id="90702-109">成员</span><span class="sxs-lookup"><span data-stu-id="90702-109">Member</span></span>|<span data-ttu-id="90702-110">值</span><span class="sxs-lookup"><span data-stu-id="90702-110">Value</span></span>|<span data-ttu-id="90702-111">说明</span><span class="sxs-lookup"><span data-stu-id="90702-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90702-112">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="90702-112">monitorAllFiles</span></span>|<span data-ttu-id="90702-113">0</span><span class="sxs-lookup"><span data-stu-id="90702-113">0</span></span>|<span data-ttu-id="90702-114">0 (默认) –监视所有文件 (双向) </span><span class="sxs-lookup"><span data-stu-id="90702-114">0 (default) – Monitor all files(bi-directional)</span></span>|
|<span data-ttu-id="90702-115">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="90702-115">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="90702-116">1</span><span class="sxs-lookup"><span data-stu-id="90702-116">1</span></span>|<span data-ttu-id="90702-117">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="90702-117">Monitor incoming files only.</span></span>|
|<span data-ttu-id="90702-118">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="90702-118">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="90702-119">双面</span><span class="sxs-lookup"><span data-stu-id="90702-119">2</span></span>|<span data-ttu-id="90702-120">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="90702-120">Monitor outgoing files only.</span></span>|




