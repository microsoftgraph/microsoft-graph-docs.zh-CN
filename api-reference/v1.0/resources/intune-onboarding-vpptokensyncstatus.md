---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
author: tfitzmac
ms.openlocfilehash: c6612c86911fd3d43128a8a7a441db8093ad3656
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316651"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="49f8e-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49f8e-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="49f8e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49f8e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49f8e-105">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="49f8e-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="49f8e-106">成员</span><span class="sxs-lookup"><span data-stu-id="49f8e-106">Members</span></span>
|<span data-ttu-id="49f8e-107">成员</span><span class="sxs-lookup"><span data-stu-id="49f8e-107">Member</span></span>|<span data-ttu-id="49f8e-108">值</span><span class="sxs-lookup"><span data-stu-id="49f8e-108">Value</span></span>|<span data-ttu-id="49f8e-109">说明</span><span class="sxs-lookup"><span data-stu-id="49f8e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49f8e-110">无</span><span class="sxs-lookup"><span data-stu-id="49f8e-110">none</span></span>|<span data-ttu-id="49f8e-111">0</span><span class="sxs-lookup"><span data-stu-id="49f8e-111">0</span></span>|<span data-ttu-id="49f8e-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="49f8e-112">Default status.</span></span>|
|<span data-ttu-id="49f8e-113">正在进行</span><span class="sxs-lookup"><span data-stu-id="49f8e-113">inProgress</span></span>|<span data-ttu-id="49f8e-114">1</span><span class="sxs-lookup"><span data-stu-id="49f8e-114">1</span></span>|<span data-ttu-id="49f8e-115">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="49f8e-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="49f8e-116">完成</span><span class="sxs-lookup"><span data-stu-id="49f8e-116">completed</span></span>|<span data-ttu-id="49f8e-117">2</span><span class="sxs-lookup"><span data-stu-id="49f8e-117">2</span></span>|<span data-ttu-id="49f8e-118">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="49f8e-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="49f8e-119">failed</span><span class="sxs-lookup"><span data-stu-id="49f8e-119">failed</span></span>|<span data-ttu-id="49f8e-120">3</span><span class="sxs-lookup"><span data-stu-id="49f8e-120">3</span></span>|<span data-ttu-id="49f8e-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="49f8e-121">Last Sync failed.</span></span>|



