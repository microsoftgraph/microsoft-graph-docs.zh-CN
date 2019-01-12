---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4101f1338513787b27ce530579ffd42c7756366a
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931284"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="67f95-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="67f95-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="67f95-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="67f95-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="67f95-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="67f95-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="67f95-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="67f95-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="67f95-107">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="67f95-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="67f95-108">成员</span><span class="sxs-lookup"><span data-stu-id="67f95-108">Members</span></span>
|<span data-ttu-id="67f95-109">成员</span><span class="sxs-lookup"><span data-stu-id="67f95-109">Member</span></span>|<span data-ttu-id="67f95-110">值</span><span class="sxs-lookup"><span data-stu-id="67f95-110">Value</span></span>|<span data-ttu-id="67f95-111">说明</span><span class="sxs-lookup"><span data-stu-id="67f95-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67f95-112">无</span><span class="sxs-lookup"><span data-stu-id="67f95-112">none</span></span>|<span data-ttu-id="67f95-113">0</span><span class="sxs-lookup"><span data-stu-id="67f95-113">0</span></span>|<span data-ttu-id="67f95-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="67f95-114">Default status.</span></span>|
|<span data-ttu-id="67f95-115">正在进行</span><span class="sxs-lookup"><span data-stu-id="67f95-115">inProgress</span></span>|<span data-ttu-id="67f95-116">1</span><span class="sxs-lookup"><span data-stu-id="67f95-116">1</span></span>|<span data-ttu-id="67f95-117">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="67f95-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="67f95-118">完成</span><span class="sxs-lookup"><span data-stu-id="67f95-118">completed</span></span>|<span data-ttu-id="67f95-119">2</span><span class="sxs-lookup"><span data-stu-id="67f95-119">2</span></span>|<span data-ttu-id="67f95-120">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="67f95-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="67f95-121">failed</span><span class="sxs-lookup"><span data-stu-id="67f95-121">failed</span></span>|<span data-ttu-id="67f95-122">3</span><span class="sxs-lookup"><span data-stu-id="67f95-122">3</span></span>|<span data-ttu-id="67f95-123">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="67f95-123">Last Sync failed.</span></span>|





