---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: db458423a00fd7b38bddea1b1954cda1ec6ec83b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888681"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="e91bd-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e91bd-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="e91bd-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e91bd-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e91bd-105">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="e91bd-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="e91bd-106">成员</span><span class="sxs-lookup"><span data-stu-id="e91bd-106">Members</span></span>
|<span data-ttu-id="e91bd-107">成员</span><span class="sxs-lookup"><span data-stu-id="e91bd-107">Member</span></span>|<span data-ttu-id="e91bd-108">值</span><span class="sxs-lookup"><span data-stu-id="e91bd-108">Value</span></span>|<span data-ttu-id="e91bd-109">Description</span><span class="sxs-lookup"><span data-stu-id="e91bd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e91bd-110">无</span><span class="sxs-lookup"><span data-stu-id="e91bd-110">none</span></span>|<span data-ttu-id="e91bd-111">0</span><span class="sxs-lookup"><span data-stu-id="e91bd-111">0</span></span>|<span data-ttu-id="e91bd-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="e91bd-112">Default status.</span></span>|
|<span data-ttu-id="e91bd-113">正在进行</span><span class="sxs-lookup"><span data-stu-id="e91bd-113">inProgress</span></span>|<span data-ttu-id="e91bd-114">1</span><span class="sxs-lookup"><span data-stu-id="e91bd-114">1</span></span>|<span data-ttu-id="e91bd-115">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="e91bd-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="e91bd-116">完成</span><span class="sxs-lookup"><span data-stu-id="e91bd-116">completed</span></span>|<span data-ttu-id="e91bd-117">2</span><span class="sxs-lookup"><span data-stu-id="e91bd-117">2</span></span>|<span data-ttu-id="e91bd-118">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="e91bd-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="e91bd-119">failed</span><span class="sxs-lookup"><span data-stu-id="e91bd-119">failed</span></span>|<span data-ttu-id="e91bd-120">3</span><span class="sxs-lookup"><span data-stu-id="e91bd-120">3</span></span>|<span data-ttu-id="e91bd-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="e91bd-121">Last Sync failed.</span></span>|



