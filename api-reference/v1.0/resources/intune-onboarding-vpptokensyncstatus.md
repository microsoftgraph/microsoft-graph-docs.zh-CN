---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5475a49341005b3c5d8037cc1697b84ce9be57f6
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37360683"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="b57f8-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b57f8-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="b57f8-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b57f8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b57f8-105">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="b57f8-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="b57f8-106">成员</span><span class="sxs-lookup"><span data-stu-id="b57f8-106">Members</span></span>
|<span data-ttu-id="b57f8-107">成员</span><span class="sxs-lookup"><span data-stu-id="b57f8-107">Member</span></span>|<span data-ttu-id="b57f8-108">值</span><span class="sxs-lookup"><span data-stu-id="b57f8-108">Value</span></span>|<span data-ttu-id="b57f8-109">说明</span><span class="sxs-lookup"><span data-stu-id="b57f8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b57f8-110">无</span><span class="sxs-lookup"><span data-stu-id="b57f8-110">none</span></span>|<span data-ttu-id="b57f8-111">0</span><span class="sxs-lookup"><span data-stu-id="b57f8-111">0</span></span>|<span data-ttu-id="b57f8-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="b57f8-112">Default status.</span></span>|
|<span data-ttu-id="b57f8-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="b57f8-113">inProgress</span></span>|<span data-ttu-id="b57f8-114">1</span><span class="sxs-lookup"><span data-stu-id="b57f8-114">1</span></span>|<span data-ttu-id="b57f8-115">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="b57f8-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="b57f8-116">后</span><span class="sxs-lookup"><span data-stu-id="b57f8-116">completed</span></span>|<span data-ttu-id="b57f8-117">双面</span><span class="sxs-lookup"><span data-stu-id="b57f8-117">2</span></span>|<span data-ttu-id="b57f8-118">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="b57f8-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="b57f8-119">未能</span><span class="sxs-lookup"><span data-stu-id="b57f8-119">failed</span></span>|<span data-ttu-id="b57f8-120">第三章</span><span class="sxs-lookup"><span data-stu-id="b57f8-120">3</span></span>|<span data-ttu-id="b57f8-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="b57f8-121">Last Sync failed.</span></span>|




