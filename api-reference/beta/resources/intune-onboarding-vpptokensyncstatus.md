---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple volume purchase Program 令牌关联的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59653a8df6c0fd08ffd0d8aa3081d58e56447a95
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31772095"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="984b7-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="984b7-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="984b7-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="984b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="984b7-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="984b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="984b7-106">可能与 Apple volume purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="984b7-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="984b7-107">成员</span><span class="sxs-lookup"><span data-stu-id="984b7-107">Members</span></span>
|<span data-ttu-id="984b7-108">成员</span><span class="sxs-lookup"><span data-stu-id="984b7-108">Member</span></span>|<span data-ttu-id="984b7-109">值</span><span class="sxs-lookup"><span data-stu-id="984b7-109">Value</span></span>|<span data-ttu-id="984b7-110">说明</span><span class="sxs-lookup"><span data-stu-id="984b7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="984b7-111">无</span><span class="sxs-lookup"><span data-stu-id="984b7-111">none</span></span>|<span data-ttu-id="984b7-112">0</span><span class="sxs-lookup"><span data-stu-id="984b7-112">0</span></span>|<span data-ttu-id="984b7-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="984b7-113">Default status.</span></span>|
|<span data-ttu-id="984b7-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="984b7-114">inProgress</span></span>|<span data-ttu-id="984b7-115">1</span><span class="sxs-lookup"><span data-stu-id="984b7-115">1</span></span>|<span data-ttu-id="984b7-116">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="984b7-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="984b7-117">后</span><span class="sxs-lookup"><span data-stu-id="984b7-117">completed</span></span>|<span data-ttu-id="984b7-118">双面</span><span class="sxs-lookup"><span data-stu-id="984b7-118">2</span></span>|<span data-ttu-id="984b7-119">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="984b7-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="984b7-120">未能</span><span class="sxs-lookup"><span data-stu-id="984b7-120">failed</span></span>|<span data-ttu-id="984b7-121">第三章</span><span class="sxs-lookup"><span data-stu-id="984b7-121">3</span></span>|<span data-ttu-id="984b7-122">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="984b7-122">Last Sync failed.</span></span>|





