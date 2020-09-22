---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: ba530475e03a2aef3b34d5387fc61d500fc94585
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025246"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="46905-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="46905-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="46905-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46905-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="46905-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="46905-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46905-106">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="46905-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="46905-107">成员</span><span class="sxs-lookup"><span data-stu-id="46905-107">Members</span></span>
|<span data-ttu-id="46905-108">成员</span><span class="sxs-lookup"><span data-stu-id="46905-108">Member</span></span>|<span data-ttu-id="46905-109">值</span><span class="sxs-lookup"><span data-stu-id="46905-109">Value</span></span>|<span data-ttu-id="46905-110">说明</span><span class="sxs-lookup"><span data-stu-id="46905-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46905-111">无</span><span class="sxs-lookup"><span data-stu-id="46905-111">none</span></span>|<span data-ttu-id="46905-112">0</span><span class="sxs-lookup"><span data-stu-id="46905-112">0</span></span>|<span data-ttu-id="46905-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="46905-113">Default status.</span></span>|
|<span data-ttu-id="46905-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="46905-114">inProgress</span></span>|<span data-ttu-id="46905-115">1 </span><span class="sxs-lookup"><span data-stu-id="46905-115">1</span></span>|<span data-ttu-id="46905-116">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="46905-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="46905-117">后</span><span class="sxs-lookup"><span data-stu-id="46905-117">completed</span></span>|<span data-ttu-id="46905-118">2 </span><span class="sxs-lookup"><span data-stu-id="46905-118">2</span></span>|<span data-ttu-id="46905-119">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="46905-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="46905-120">未能</span><span class="sxs-lookup"><span data-stu-id="46905-120">failed</span></span>|<span data-ttu-id="46905-121">第三章</span><span class="sxs-lookup"><span data-stu-id="46905-121">3</span></span>|<span data-ttu-id="46905-122">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="46905-122">Last Sync failed.</span></span>|









