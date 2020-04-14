---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 28ec478d33ddeb5c56963bf6c750a98ab217cc75
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446806"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="ff3fa-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ff3fa-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="ff3fa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff3fa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff3fa-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff3fa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff3fa-107">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="ff3fa-108">成员</span><span class="sxs-lookup"><span data-stu-id="ff3fa-108">Members</span></span>
|<span data-ttu-id="ff3fa-109">成员</span><span class="sxs-lookup"><span data-stu-id="ff3fa-109">Member</span></span>|<span data-ttu-id="ff3fa-110">值</span><span class="sxs-lookup"><span data-stu-id="ff3fa-110">Value</span></span>|<span data-ttu-id="ff3fa-111">说明</span><span class="sxs-lookup"><span data-stu-id="ff3fa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff3fa-112">无</span><span class="sxs-lookup"><span data-stu-id="ff3fa-112">none</span></span>|<span data-ttu-id="ff3fa-113">0</span><span class="sxs-lookup"><span data-stu-id="ff3fa-113">0</span></span>|<span data-ttu-id="ff3fa-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-114">Default status.</span></span>|
|<span data-ttu-id="ff3fa-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="ff3fa-115">inProgress</span></span>|<span data-ttu-id="ff3fa-116">1</span><span class="sxs-lookup"><span data-stu-id="ff3fa-116">1</span></span>|<span data-ttu-id="ff3fa-117">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="ff3fa-118">后</span><span class="sxs-lookup"><span data-stu-id="ff3fa-118">completed</span></span>|<span data-ttu-id="ff3fa-119">双面</span><span class="sxs-lookup"><span data-stu-id="ff3fa-119">2</span></span>|<span data-ttu-id="ff3fa-120">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="ff3fa-121">未能</span><span class="sxs-lookup"><span data-stu-id="ff3fa-121">failed</span></span>|<span data-ttu-id="ff3fa-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ff3fa-122">3</span></span>|<span data-ttu-id="ff3fa-123">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="ff3fa-123">Last Sync failed.</span></span>|



