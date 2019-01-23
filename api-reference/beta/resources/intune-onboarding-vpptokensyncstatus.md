---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1a53906018d45181bd16750e4ed3f0dac9dcb0d1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398812"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="87ae4-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="87ae4-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="87ae4-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="87ae4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="87ae4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87ae4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87ae4-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="87ae4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="87ae4-107">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="87ae4-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="87ae4-108">成员</span><span class="sxs-lookup"><span data-stu-id="87ae4-108">Members</span></span>
|<span data-ttu-id="87ae4-109">成员</span><span class="sxs-lookup"><span data-stu-id="87ae4-109">Member</span></span>|<span data-ttu-id="87ae4-110">值</span><span class="sxs-lookup"><span data-stu-id="87ae4-110">Value</span></span>|<span data-ttu-id="87ae4-111">说明</span><span class="sxs-lookup"><span data-stu-id="87ae4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87ae4-112">无</span><span class="sxs-lookup"><span data-stu-id="87ae4-112">none</span></span>|<span data-ttu-id="87ae4-113">0</span><span class="sxs-lookup"><span data-stu-id="87ae4-113">0</span></span>|<span data-ttu-id="87ae4-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="87ae4-114">Default status.</span></span>|
|<span data-ttu-id="87ae4-115">正在进行</span><span class="sxs-lookup"><span data-stu-id="87ae4-115">inProgress</span></span>|<span data-ttu-id="87ae4-116">1</span><span class="sxs-lookup"><span data-stu-id="87ae4-116">1</span></span>|<span data-ttu-id="87ae4-117">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="87ae4-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="87ae4-118">完成</span><span class="sxs-lookup"><span data-stu-id="87ae4-118">completed</span></span>|<span data-ttu-id="87ae4-119">2</span><span class="sxs-lookup"><span data-stu-id="87ae4-119">2</span></span>|<span data-ttu-id="87ae4-120">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="87ae4-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="87ae4-121">failed</span><span class="sxs-lookup"><span data-stu-id="87ae4-121">failed</span></span>|<span data-ttu-id="87ae4-122">3</span><span class="sxs-lookup"><span data-stu-id="87ae4-122">3</span></span>|<span data-ttu-id="87ae4-123">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="87ae4-123">Last Sync failed.</span></span>|




