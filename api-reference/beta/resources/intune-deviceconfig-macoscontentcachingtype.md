---
title: macOSContentCachingType 枚举类型
description: 指示 Apple 的内容缓存服务允许缓存的内容类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a79cd14a6bd765f260439a259c63106e6211cacc
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49268732"
---
# <a name="macoscontentcachingtype-enum-type"></a><span data-ttu-id="fbc66-103">macOSContentCachingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fbc66-103">macOSContentCachingType enum type</span></span>

<span data-ttu-id="fbc66-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbc66-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fbc66-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fbc66-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fbc66-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fbc66-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fbc66-107">指示 Apple 的内容缓存服务允许缓存的内容类型。</span><span class="sxs-lookup"><span data-stu-id="fbc66-107">Indicates the type of content allowed to be cached by Apple's content caching service.</span></span>

## <a name="members"></a><span data-ttu-id="fbc66-108">成员</span><span class="sxs-lookup"><span data-stu-id="fbc66-108">Members</span></span>
|<span data-ttu-id="fbc66-109">成员</span><span class="sxs-lookup"><span data-stu-id="fbc66-109">Member</span></span>|<span data-ttu-id="fbc66-110">值</span><span class="sxs-lookup"><span data-stu-id="fbc66-110">Value</span></span>|<span data-ttu-id="fbc66-111">说明</span><span class="sxs-lookup"><span data-stu-id="fbc66-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fbc66-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fbc66-112">notConfigured</span></span>|<span data-ttu-id="fbc66-113">0</span><span class="sxs-lookup"><span data-stu-id="fbc66-113">0</span></span>|<span data-ttu-id="fbc66-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="fbc66-114">Default.</span></span> <span data-ttu-id="fbc66-115">将缓存用户 iCloud 数据和非 iCloud 数据。</span><span class="sxs-lookup"><span data-stu-id="fbc66-115">Both user iCloud data and non-iCloud data will be cached.</span></span>|
|<span data-ttu-id="fbc66-116">userContentOnly</span><span class="sxs-lookup"><span data-stu-id="fbc66-116">userContentOnly</span></span>|<span data-ttu-id="fbc66-117">1</span><span class="sxs-lookup"><span data-stu-id="fbc66-117">1</span></span>|<span data-ttu-id="fbc66-118">允许 Apple 的内容缓存服务缓存用户 iCloud 数据。</span><span class="sxs-lookup"><span data-stu-id="fbc66-118">Allow Apple's content caching service to cache user iCloud data.</span></span>|
|<span data-ttu-id="fbc66-119">sharedContentOnly</span><span class="sxs-lookup"><span data-stu-id="fbc66-119">sharedContentOnly</span></span>|<span data-ttu-id="fbc66-120">双面</span><span class="sxs-lookup"><span data-stu-id="fbc66-120">2</span></span>|<span data-ttu-id="fbc66-121">允许 Apple 的内容缓存服务缓存非 iCloud 数据 (例如，应用程序和软件更新) 。</span><span class="sxs-lookup"><span data-stu-id="fbc66-121">Allow Apple's content caching service to cache non-iCloud data (e.g. app and software updates).</span></span>|




