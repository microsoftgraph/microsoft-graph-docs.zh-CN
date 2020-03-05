---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a9955b825fffab7837cb2c77ffa443ad3f9c9fa1
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524060"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="c489e-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c489e-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="c489e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c489e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c489e-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c489e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c489e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c489e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c489e-107">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="c489e-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="c489e-108">成员</span><span class="sxs-lookup"><span data-stu-id="c489e-108">Members</span></span>
|<span data-ttu-id="c489e-109">成员</span><span class="sxs-lookup"><span data-stu-id="c489e-109">Member</span></span>|<span data-ttu-id="c489e-110">值</span><span class="sxs-lookup"><span data-stu-id="c489e-110">Value</span></span>|<span data-ttu-id="c489e-111">说明</span><span class="sxs-lookup"><span data-stu-id="c489e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c489e-112">无</span><span class="sxs-lookup"><span data-stu-id="c489e-112">none</span></span>|<span data-ttu-id="c489e-113">0</span><span class="sxs-lookup"><span data-stu-id="c489e-113">0</span></span>|<span data-ttu-id="c489e-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="c489e-114">Default status.</span></span>|
|<span data-ttu-id="c489e-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="c489e-115">inProgress</span></span>|<span data-ttu-id="c489e-116">1 </span><span class="sxs-lookup"><span data-stu-id="c489e-116">1</span></span>|<span data-ttu-id="c489e-117">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="c489e-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="c489e-118">后</span><span class="sxs-lookup"><span data-stu-id="c489e-118">completed</span></span>|<span data-ttu-id="c489e-119">2 </span><span class="sxs-lookup"><span data-stu-id="c489e-119">2</span></span>|<span data-ttu-id="c489e-120">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="c489e-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="c489e-121">未能</span><span class="sxs-lookup"><span data-stu-id="c489e-121">failed</span></span>|<span data-ttu-id="c489e-122">3 </span><span class="sxs-lookup"><span data-stu-id="c489e-122">3</span></span>|<span data-ttu-id="c489e-123">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="c489e-123">Last Sync failed.</span></span>|



