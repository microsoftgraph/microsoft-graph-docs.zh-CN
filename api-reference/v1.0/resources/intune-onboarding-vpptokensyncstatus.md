---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple volume purchase Program 令牌关联的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6938fd41b6cd7c089b08edb629bc1197ec47c2d7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548087"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="547bc-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="547bc-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="547bc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="547bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="547bc-105">可能与 Apple volume purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="547bc-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="547bc-106">成员</span><span class="sxs-lookup"><span data-stu-id="547bc-106">Members</span></span>
|<span data-ttu-id="547bc-107">成员</span><span class="sxs-lookup"><span data-stu-id="547bc-107">Member</span></span>|<span data-ttu-id="547bc-108">值</span><span class="sxs-lookup"><span data-stu-id="547bc-108">Value</span></span>|<span data-ttu-id="547bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="547bc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="547bc-110">无</span><span class="sxs-lookup"><span data-stu-id="547bc-110">none</span></span>|<span data-ttu-id="547bc-111">0</span><span class="sxs-lookup"><span data-stu-id="547bc-111">0</span></span>|<span data-ttu-id="547bc-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="547bc-112">Default status.</span></span>|
|<span data-ttu-id="547bc-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="547bc-113">inProgress</span></span>|<span data-ttu-id="547bc-114">1</span><span class="sxs-lookup"><span data-stu-id="547bc-114">1</span></span>|<span data-ttu-id="547bc-115">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="547bc-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="547bc-116">后</span><span class="sxs-lookup"><span data-stu-id="547bc-116">completed</span></span>|<span data-ttu-id="547bc-117">2 </span><span class="sxs-lookup"><span data-stu-id="547bc-117">2</span></span>|<span data-ttu-id="547bc-118">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="547bc-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="547bc-119">未能</span><span class="sxs-lookup"><span data-stu-id="547bc-119">failed</span></span>|<span data-ttu-id="547bc-120">3 </span><span class="sxs-lookup"><span data-stu-id="547bc-120">3</span></span>|<span data-ttu-id="547bc-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="547bc-121">Last Sync failed.</span></span>|



