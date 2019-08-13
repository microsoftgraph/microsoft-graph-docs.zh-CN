---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ede152d056c082e3b55c9142730ce61af86ae48c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36369344"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="73183-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="73183-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="73183-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="73183-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73183-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73183-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73183-106">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="73183-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="73183-107">成员</span><span class="sxs-lookup"><span data-stu-id="73183-107">Members</span></span>
|<span data-ttu-id="73183-108">成员</span><span class="sxs-lookup"><span data-stu-id="73183-108">Member</span></span>|<span data-ttu-id="73183-109">值</span><span class="sxs-lookup"><span data-stu-id="73183-109">Value</span></span>|<span data-ttu-id="73183-110">说明</span><span class="sxs-lookup"><span data-stu-id="73183-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73183-111">无</span><span class="sxs-lookup"><span data-stu-id="73183-111">none</span></span>|<span data-ttu-id="73183-112">0</span><span class="sxs-lookup"><span data-stu-id="73183-112">0</span></span>|<span data-ttu-id="73183-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="73183-113">Default status.</span></span>|
|<span data-ttu-id="73183-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="73183-114">inProgress</span></span>|<span data-ttu-id="73183-115">1</span><span class="sxs-lookup"><span data-stu-id="73183-115">1</span></span>|<span data-ttu-id="73183-116">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="73183-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="73183-117">后</span><span class="sxs-lookup"><span data-stu-id="73183-117">completed</span></span>|<span data-ttu-id="73183-118">双面</span><span class="sxs-lookup"><span data-stu-id="73183-118">2</span></span>|<span data-ttu-id="73183-119">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="73183-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="73183-120">未能</span><span class="sxs-lookup"><span data-stu-id="73183-120">failed</span></span>|<span data-ttu-id="73183-121">第三章</span><span class="sxs-lookup"><span data-stu-id="73183-121">3</span></span>|<span data-ttu-id="73183-122">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="73183-122">Last Sync failed.</span></span>|



