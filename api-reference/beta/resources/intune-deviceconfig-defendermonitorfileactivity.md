---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc43905a4fa245a497d28c8bae97724534a6470f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42794471"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="c2c38-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c2c38-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="c2c38-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2c38-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2c38-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2c38-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2c38-106">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="c2c38-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="c2c38-107">成员</span><span class="sxs-lookup"><span data-stu-id="c2c38-107">Members</span></span>
|<span data-ttu-id="c2c38-108">成员</span><span class="sxs-lookup"><span data-stu-id="c2c38-108">Member</span></span>|<span data-ttu-id="c2c38-109">值</span><span class="sxs-lookup"><span data-stu-id="c2c38-109">Value</span></span>|<span data-ttu-id="c2c38-110">说明</span><span class="sxs-lookup"><span data-stu-id="c2c38-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2c38-111">定制</span><span class="sxs-lookup"><span data-stu-id="c2c38-111">userDefined</span></span>|<span data-ttu-id="c2c38-112">0</span><span class="sxs-lookup"><span data-stu-id="c2c38-112">0</span></span>|<span data-ttu-id="c2c38-113">用户定义，默认值，无意向。</span><span class="sxs-lookup"><span data-stu-id="c2c38-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="c2c38-114">disable</span><span class="sxs-lookup"><span data-stu-id="c2c38-114">disable</span></span>|<span data-ttu-id="c2c38-115">1</span><span class="sxs-lookup"><span data-stu-id="c2c38-115">1</span></span>|<span data-ttu-id="c2c38-116">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="c2c38-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="c2c38-117">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="c2c38-117">monitorAllFiles</span></span>|<span data-ttu-id="c2c38-118">双面</span><span class="sxs-lookup"><span data-stu-id="c2c38-118">2</span></span>|<span data-ttu-id="c2c38-119">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="c2c38-119">Monitor all files.</span></span>|
|<span data-ttu-id="c2c38-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="c2c38-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="c2c38-121">第三章</span><span class="sxs-lookup"><span data-stu-id="c2c38-121">3</span></span>| <span data-ttu-id="c2c38-122">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="c2c38-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="c2c38-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="c2c38-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="c2c38-124">4 </span><span class="sxs-lookup"><span data-stu-id="c2c38-124">4</span></span>|<span data-ttu-id="c2c38-125">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="c2c38-125">Monitor outgoing files only.</span></span>|



