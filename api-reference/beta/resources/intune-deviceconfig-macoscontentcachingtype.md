---
title: macOSContentCachingType 枚举类型
description: 指示 Apple 的内容缓存服务允许缓存的内容类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9022b320507cc10455e2eeb3ebd3a3ca58d52f71
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47993838"
---
# <a name="macoscontentcachingtype-enum-type"></a><span data-ttu-id="30d59-103">macOSContentCachingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="30d59-103">macOSContentCachingType enum type</span></span>

<span data-ttu-id="30d59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="30d59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="30d59-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="30d59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="30d59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="30d59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="30d59-107">指示 Apple 的内容缓存服务允许缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="30d59-107">Indicates the type of content allowed to be cached by Apple's content caching service.</span></span>

## <a name="members"></a><span data-ttu-id="30d59-108">成员</span><span class="sxs-lookup"><span data-stu-id="30d59-108">Members</span></span>
|<span data-ttu-id="30d59-109">成员</span><span class="sxs-lookup"><span data-stu-id="30d59-109">Member</span></span>|<span data-ttu-id="30d59-110">值</span><span class="sxs-lookup"><span data-stu-id="30d59-110">Value</span></span>|<span data-ttu-id="30d59-111">说明</span><span class="sxs-lookup"><span data-stu-id="30d59-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="30d59-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="30d59-112">notConfigured</span></span>|<span data-ttu-id="30d59-113">0</span><span class="sxs-lookup"><span data-stu-id="30d59-113">0</span></span>|<span data-ttu-id="30d59-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="30d59-114">Default.</span></span> <span data-ttu-id="30d59-115">将缓存用户 iCloud 数据和非 iCloud 数据。</span><span class="sxs-lookup"><span data-stu-id="30d59-115">Both user iCloud data and non-iCloud data will be cached.</span></span>|
|<span data-ttu-id="30d59-116">userContentOnly</span><span class="sxs-lookup"><span data-stu-id="30d59-116">userContentOnly</span></span>|<span data-ttu-id="30d59-117">1 </span><span class="sxs-lookup"><span data-stu-id="30d59-117">1</span></span>|<span data-ttu-id="30d59-118">允许 Apple 的内容缓存服务缓存用户 iCloud 数据。</span><span class="sxs-lookup"><span data-stu-id="30d59-118">Allow Apple's content caching service to cache user iCloud data.</span></span>|
|<span data-ttu-id="30d59-119">sharedContentOnly</span><span class="sxs-lookup"><span data-stu-id="30d59-119">sharedContentOnly</span></span>|<span data-ttu-id="30d59-120">2 </span><span class="sxs-lookup"><span data-stu-id="30d59-120">2</span></span>|<span data-ttu-id="30d59-121">允许 Apple 的内容缓存服务缓存非 iCloud 数据 (例如，应用程序和软件更新) 。</span><span class="sxs-lookup"><span data-stu-id="30d59-121">Allow Apple's content caching service to cache non-iCloud data (e.g. app and software updates).</span></span>|






