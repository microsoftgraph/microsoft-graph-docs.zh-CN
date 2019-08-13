---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5c9c5bedbb07a89b51deb25942caeb5385f60e0a
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333546"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="626da-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="626da-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="626da-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="626da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="626da-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="626da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="626da-106">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="626da-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="626da-107">成员</span><span class="sxs-lookup"><span data-stu-id="626da-107">Members</span></span>
|<span data-ttu-id="626da-108">成员</span><span class="sxs-lookup"><span data-stu-id="626da-108">Member</span></span>|<span data-ttu-id="626da-109">值</span><span class="sxs-lookup"><span data-stu-id="626da-109">Value</span></span>|<span data-ttu-id="626da-110">说明</span><span class="sxs-lookup"><span data-stu-id="626da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="626da-111">定制</span><span class="sxs-lookup"><span data-stu-id="626da-111">userDefined</span></span>|<span data-ttu-id="626da-112">0</span><span class="sxs-lookup"><span data-stu-id="626da-112">0</span></span>|<span data-ttu-id="626da-113">用户定义, 默认值, 无意向。</span><span class="sxs-lookup"><span data-stu-id="626da-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="626da-114">disable</span><span class="sxs-lookup"><span data-stu-id="626da-114">disable</span></span>|<span data-ttu-id="626da-115">1</span><span class="sxs-lookup"><span data-stu-id="626da-115">1</span></span>|<span data-ttu-id="626da-116">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="626da-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="626da-117">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="626da-117">monitorAllFiles</span></span>|<span data-ttu-id="626da-118">双面</span><span class="sxs-lookup"><span data-stu-id="626da-118">2</span></span>|<span data-ttu-id="626da-119">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="626da-119">Monitor all files.</span></span>|
|<span data-ttu-id="626da-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="626da-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="626da-121">第三章</span><span class="sxs-lookup"><span data-stu-id="626da-121">3</span></span>| <span data-ttu-id="626da-122">仅监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="626da-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="626da-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="626da-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="626da-124">4</span><span class="sxs-lookup"><span data-stu-id="626da-124">4</span></span>|<span data-ttu-id="626da-125">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="626da-125">Monitor outgoing files only.</span></span>|



