---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dfdb80ae40abcc505927b94a33330bc09454e790
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27965080"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="9220d-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9220d-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="9220d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9220d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9220d-105">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="9220d-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="9220d-106">成员</span><span class="sxs-lookup"><span data-stu-id="9220d-106">Members</span></span>
|<span data-ttu-id="9220d-107">成员</span><span class="sxs-lookup"><span data-stu-id="9220d-107">Member</span></span>|<span data-ttu-id="9220d-108">值</span><span class="sxs-lookup"><span data-stu-id="9220d-108">Value</span></span>|<span data-ttu-id="9220d-109">Description</span><span class="sxs-lookup"><span data-stu-id="9220d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9220d-110">无</span><span class="sxs-lookup"><span data-stu-id="9220d-110">none</span></span>|<span data-ttu-id="9220d-111">0</span><span class="sxs-lookup"><span data-stu-id="9220d-111">0</span></span>|<span data-ttu-id="9220d-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="9220d-112">Default status.</span></span>|
|<span data-ttu-id="9220d-113">正在进行</span><span class="sxs-lookup"><span data-stu-id="9220d-113">inProgress</span></span>|<span data-ttu-id="9220d-114">1</span><span class="sxs-lookup"><span data-stu-id="9220d-114">1</span></span>|<span data-ttu-id="9220d-115">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="9220d-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="9220d-116">完成</span><span class="sxs-lookup"><span data-stu-id="9220d-116">completed</span></span>|<span data-ttu-id="9220d-117">2</span><span class="sxs-lookup"><span data-stu-id="9220d-117">2</span></span>|<span data-ttu-id="9220d-118">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="9220d-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="9220d-119">failed</span><span class="sxs-lookup"><span data-stu-id="9220d-119">failed</span></span>|<span data-ttu-id="9220d-120">3</span><span class="sxs-lookup"><span data-stu-id="9220d-120">3</span></span>|<span data-ttu-id="9220d-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="9220d-121">Last Sync failed.</span></span>|



