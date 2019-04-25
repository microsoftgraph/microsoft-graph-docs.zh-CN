---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple volume purchase Program 令牌关联的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 59653a8df6c0fd08ffd0d8aa3081d58e56447a95
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566372"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="dc568-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dc568-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="dc568-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dc568-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dc568-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dc568-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dc568-106">可能与 Apple volume purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="dc568-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="dc568-107">成员</span><span class="sxs-lookup"><span data-stu-id="dc568-107">Members</span></span>
|<span data-ttu-id="dc568-108">成员</span><span class="sxs-lookup"><span data-stu-id="dc568-108">Member</span></span>|<span data-ttu-id="dc568-109">值</span><span class="sxs-lookup"><span data-stu-id="dc568-109">Value</span></span>|<span data-ttu-id="dc568-110">说明</span><span class="sxs-lookup"><span data-stu-id="dc568-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc568-111">无</span><span class="sxs-lookup"><span data-stu-id="dc568-111">none</span></span>|<span data-ttu-id="dc568-112">0</span><span class="sxs-lookup"><span data-stu-id="dc568-112">0</span></span>|<span data-ttu-id="dc568-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="dc568-113">Default status.</span></span>|
|<span data-ttu-id="dc568-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="dc568-114">inProgress</span></span>|<span data-ttu-id="dc568-115">1</span><span class="sxs-lookup"><span data-stu-id="dc568-115">1</span></span>|<span data-ttu-id="dc568-116">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="dc568-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="dc568-117">后</span><span class="sxs-lookup"><span data-stu-id="dc568-117">completed</span></span>|<span data-ttu-id="dc568-118">2 </span><span class="sxs-lookup"><span data-stu-id="dc568-118">2</span></span>|<span data-ttu-id="dc568-119">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="dc568-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="dc568-120">未能</span><span class="sxs-lookup"><span data-stu-id="dc568-120">failed</span></span>|<span data-ttu-id="dc568-121">3 </span><span class="sxs-lookup"><span data-stu-id="dc568-121">3</span></span>|<span data-ttu-id="dc568-122">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="dc568-122">Last Sync failed.</span></span>|





