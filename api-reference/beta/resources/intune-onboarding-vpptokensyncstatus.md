---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 27d66ddf8e17072c7df27c63565e83e5d69df7c3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259394"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="7df7b-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7df7b-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="7df7b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7df7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7df7b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7df7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7df7b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7df7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7df7b-107">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="7df7b-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="7df7b-108">成员</span><span class="sxs-lookup"><span data-stu-id="7df7b-108">Members</span></span>
|<span data-ttu-id="7df7b-109">成员</span><span class="sxs-lookup"><span data-stu-id="7df7b-109">Member</span></span>|<span data-ttu-id="7df7b-110">值</span><span class="sxs-lookup"><span data-stu-id="7df7b-110">Value</span></span>|<span data-ttu-id="7df7b-111">说明</span><span class="sxs-lookup"><span data-stu-id="7df7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7df7b-112">无</span><span class="sxs-lookup"><span data-stu-id="7df7b-112">none</span></span>|<span data-ttu-id="7df7b-113">0</span><span class="sxs-lookup"><span data-stu-id="7df7b-113">0</span></span>|<span data-ttu-id="7df7b-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="7df7b-114">Default status.</span></span>|
|<span data-ttu-id="7df7b-115">inProgress</span><span class="sxs-lookup"><span data-stu-id="7df7b-115">inProgress</span></span>|<span data-ttu-id="7df7b-116">1</span><span class="sxs-lookup"><span data-stu-id="7df7b-116">1</span></span>|<span data-ttu-id="7df7b-117">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="7df7b-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="7df7b-118">后</span><span class="sxs-lookup"><span data-stu-id="7df7b-118">completed</span></span>|<span data-ttu-id="7df7b-119">双面</span><span class="sxs-lookup"><span data-stu-id="7df7b-119">2</span></span>|<span data-ttu-id="7df7b-120">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="7df7b-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="7df7b-121">未能</span><span class="sxs-lookup"><span data-stu-id="7df7b-121">failed</span></span>|<span data-ttu-id="7df7b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7df7b-122">3</span></span>|<span data-ttu-id="7df7b-123">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="7df7b-123">Last Sync failed.</span></span>|




