---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0d17b599460a5d7b6a7e37f7255f050df8350ccd
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447988"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="9fc28-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9fc28-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="9fc28-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9fc28-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9fc28-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9fc28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9fc28-106">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="9fc28-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="9fc28-107">成员</span><span class="sxs-lookup"><span data-stu-id="9fc28-107">Members</span></span>
|<span data-ttu-id="9fc28-108">成员</span><span class="sxs-lookup"><span data-stu-id="9fc28-108">Member</span></span>|<span data-ttu-id="9fc28-109">值</span><span class="sxs-lookup"><span data-stu-id="9fc28-109">Value</span></span>|<span data-ttu-id="9fc28-110">说明</span><span class="sxs-lookup"><span data-stu-id="9fc28-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9fc28-111">无</span><span class="sxs-lookup"><span data-stu-id="9fc28-111">none</span></span>|<span data-ttu-id="9fc28-112">0</span><span class="sxs-lookup"><span data-stu-id="9fc28-112">0</span></span>|<span data-ttu-id="9fc28-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="9fc28-113">Default status.</span></span>|
|<span data-ttu-id="9fc28-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="9fc28-114">inProgress</span></span>|<span data-ttu-id="9fc28-115">1 </span><span class="sxs-lookup"><span data-stu-id="9fc28-115">1</span></span>|<span data-ttu-id="9fc28-116">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="9fc28-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="9fc28-117">后</span><span class="sxs-lookup"><span data-stu-id="9fc28-117">completed</span></span>|<span data-ttu-id="9fc28-118">2 </span><span class="sxs-lookup"><span data-stu-id="9fc28-118">2</span></span>|<span data-ttu-id="9fc28-119">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="9fc28-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="9fc28-120">未能</span><span class="sxs-lookup"><span data-stu-id="9fc28-120">failed</span></span>|<span data-ttu-id="9fc28-121">3 </span><span class="sxs-lookup"><span data-stu-id="9fc28-121">3</span></span>|<span data-ttu-id="9fc28-122">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="9fc28-122">Last Sync failed.</span></span>|




