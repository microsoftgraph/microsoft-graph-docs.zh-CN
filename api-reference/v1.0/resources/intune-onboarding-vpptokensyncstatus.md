---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple volume purchase Program 令牌关联的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254049"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="16e32-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="16e32-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="16e32-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="16e32-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="16e32-105">可能与 Apple volume purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="16e32-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="16e32-106">成员</span><span class="sxs-lookup"><span data-stu-id="16e32-106">Members</span></span>
|<span data-ttu-id="16e32-107">成员</span><span class="sxs-lookup"><span data-stu-id="16e32-107">Member</span></span>|<span data-ttu-id="16e32-108">值</span><span class="sxs-lookup"><span data-stu-id="16e32-108">Value</span></span>|<span data-ttu-id="16e32-109">说明</span><span class="sxs-lookup"><span data-stu-id="16e32-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16e32-110">无</span><span class="sxs-lookup"><span data-stu-id="16e32-110">none</span></span>|<span data-ttu-id="16e32-111">0</span><span class="sxs-lookup"><span data-stu-id="16e32-111">0</span></span>|<span data-ttu-id="16e32-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="16e32-112">Default status.</span></span>|
|<span data-ttu-id="16e32-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="16e32-113">inProgress</span></span>|<span data-ttu-id="16e32-114">1</span><span class="sxs-lookup"><span data-stu-id="16e32-114">1</span></span>|<span data-ttu-id="16e32-115">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="16e32-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="16e32-116">后</span><span class="sxs-lookup"><span data-stu-id="16e32-116">completed</span></span>|<span data-ttu-id="16e32-117">双面</span><span class="sxs-lookup"><span data-stu-id="16e32-117">2</span></span>|<span data-ttu-id="16e32-118">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="16e32-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="16e32-119">failed</span><span class="sxs-lookup"><span data-stu-id="16e32-119">failed</span></span>|<span data-ttu-id="16e32-120">第三章</span><span class="sxs-lookup"><span data-stu-id="16e32-120">3</span></span>|<span data-ttu-id="16e32-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="16e32-121">Last Sync failed.</span></span>|



