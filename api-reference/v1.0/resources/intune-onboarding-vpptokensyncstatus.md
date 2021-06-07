---
title: vppTokenSyncStatus 枚举类型
description: 与 Apple Volume Purchase Program 令牌关联的可能同步状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1468240f5d83002d21336299486bceca259a207f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755691"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="aebdd-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aebdd-103">vppTokenSyncStatus enum type</span></span>

<span data-ttu-id="aebdd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aebdd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aebdd-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aebdd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aebdd-106">与 Apple Volume Purchase Program 令牌关联的可能同步状态。</span><span class="sxs-lookup"><span data-stu-id="aebdd-106">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="aebdd-107">成员</span><span class="sxs-lookup"><span data-stu-id="aebdd-107">Members</span></span>
|<span data-ttu-id="aebdd-108">成员</span><span class="sxs-lookup"><span data-stu-id="aebdd-108">Member</span></span>|<span data-ttu-id="aebdd-109">值</span><span class="sxs-lookup"><span data-stu-id="aebdd-109">Value</span></span>|<span data-ttu-id="aebdd-110">Description</span><span class="sxs-lookup"><span data-stu-id="aebdd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aebdd-111">无</span><span class="sxs-lookup"><span data-stu-id="aebdd-111">none</span></span>|<span data-ttu-id="aebdd-112">0</span><span class="sxs-lookup"><span data-stu-id="aebdd-112">0</span></span>|<span data-ttu-id="aebdd-113">默认状态。</span><span class="sxs-lookup"><span data-stu-id="aebdd-113">Default status.</span></span>|
|<span data-ttu-id="aebdd-114">inProgress</span><span class="sxs-lookup"><span data-stu-id="aebdd-114">inProgress</span></span>|<span data-ttu-id="aebdd-115">1</span><span class="sxs-lookup"><span data-stu-id="aebdd-115">1</span></span>|<span data-ttu-id="aebdd-116">正在同步的最后一个同步。</span><span class="sxs-lookup"><span data-stu-id="aebdd-116">Last Sync in progress.</span></span>|
|<span data-ttu-id="aebdd-117">已完成</span><span class="sxs-lookup"><span data-stu-id="aebdd-117">completed</span></span>|<span data-ttu-id="aebdd-118">2</span><span class="sxs-lookup"><span data-stu-id="aebdd-118">2</span></span>|<span data-ttu-id="aebdd-119">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="aebdd-119">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="aebdd-120">failed</span><span class="sxs-lookup"><span data-stu-id="aebdd-120">failed</span></span>|<span data-ttu-id="aebdd-121">3</span><span class="sxs-lookup"><span data-stu-id="aebdd-121">3</span></span>|<span data-ttu-id="aebdd-122">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="aebdd-122">Last Sync failed.</span></span>|




