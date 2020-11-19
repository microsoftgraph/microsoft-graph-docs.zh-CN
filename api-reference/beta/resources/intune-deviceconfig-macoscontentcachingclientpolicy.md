---
title: macOSContentCachingClientPolicy 枚举类型
description: 确定内容缓存将服务的客户端。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b8b2baeb66173b8e09f46bd570aa799ca9d2845e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268781"
---
# <a name="macoscontentcachingclientpolicy-enum-type"></a><span data-ttu-id="f02c3-103">macOSContentCachingClientPolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f02c3-103">macOSContentCachingClientPolicy enum type</span></span>

<span data-ttu-id="f02c3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f02c3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f02c3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f02c3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f02c3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f02c3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f02c3-107">确定内容缓存将服务的客户端。</span><span class="sxs-lookup"><span data-stu-id="f02c3-107">Determines which clients a content cache will serve.</span></span>

## <a name="members"></a><span data-ttu-id="f02c3-108">成员</span><span class="sxs-lookup"><span data-stu-id="f02c3-108">Members</span></span>
|<span data-ttu-id="f02c3-109">成员</span><span class="sxs-lookup"><span data-stu-id="f02c3-109">Member</span></span>|<span data-ttu-id="f02c3-110">值</span><span class="sxs-lookup"><span data-stu-id="f02c3-110">Value</span></span>|<span data-ttu-id="f02c3-111">说明</span><span class="sxs-lookup"><span data-stu-id="f02c3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f02c3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f02c3-112">notConfigured</span></span>|<span data-ttu-id="f02c3-113">0</span><span class="sxs-lookup"><span data-stu-id="f02c3-113">0</span></span>|<span data-ttu-id="f02c3-114">默认值为本地网络中的客户端。</span><span class="sxs-lookup"><span data-stu-id="f02c3-114">Defaults to clients in local network.</span></span>|
|<span data-ttu-id="f02c3-115">clientsInLocalNetwork</span><span class="sxs-lookup"><span data-stu-id="f02c3-115">clientsInLocalNetwork</span></span>|<span data-ttu-id="f02c3-116">1</span><span class="sxs-lookup"><span data-stu-id="f02c3-116">1</span></span>|<span data-ttu-id="f02c3-117">内容缓存将仅在其直接本地网络中向设备提供内容。</span><span class="sxs-lookup"><span data-stu-id="f02c3-117">Content caches will provide content to devices only in their immediate local network.</span></span>|
|<span data-ttu-id="f02c3-118">clientsWithSamePublicIpAddress</span><span class="sxs-lookup"><span data-stu-id="f02c3-118">clientsWithSamePublicIpAddress</span></span>|<span data-ttu-id="f02c3-119">双面</span><span class="sxs-lookup"><span data-stu-id="f02c3-119">2</span></span>|<span data-ttu-id="f02c3-120">内容缓存将向共享相同公用 IP 地址的设备提供内容。</span><span class="sxs-lookup"><span data-stu-id="f02c3-120">Content caches will provide content to devices that share the same public IP address.</span></span>|
|<span data-ttu-id="f02c3-121">clientsInCustomLocalNetworks</span><span class="sxs-lookup"><span data-stu-id="f02c3-121">clientsInCustomLocalNetworks</span></span>|<span data-ttu-id="f02c3-122">第三章</span><span class="sxs-lookup"><span data-stu-id="f02c3-122">3</span></span>|<span data-ttu-id="f02c3-123">内容缓存将向 contentCachingClientListenRanges 中的设备提供内容。</span><span class="sxs-lookup"><span data-stu-id="f02c3-123">Content caches will provide content to devices in contentCachingClientListenRanges.</span></span>|
|<span data-ttu-id="f02c3-124">clientsInCustomLocalNetworksWithFallback</span><span class="sxs-lookup"><span data-stu-id="f02c3-124">clientsInCustomLocalNetworksWithFallback</span></span>|<span data-ttu-id="f02c3-125">4 </span><span class="sxs-lookup"><span data-stu-id="f02c3-125">4</span></span>|<span data-ttu-id="f02c3-126">内容缓存将向 contentCachingClientListenRanges、contentCachingPeerListenRanges 和 contentCachingParents 中的设备提供内容。</span><span class="sxs-lookup"><span data-stu-id="f02c3-126">Content caches will provide content to devices in contentCachingClientListenRanges, contentCachingPeerListenRanges, and contentCachingParents.</span></span>|




