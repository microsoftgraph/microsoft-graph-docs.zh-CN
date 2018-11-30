---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
ms.openlocfilehash: e038f15a3c58928ebb066c0fbf5aac320bf574a9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010247"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="1ff59-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1ff59-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="1ff59-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1ff59-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1ff59-105">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="1ff59-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="1ff59-106">成员</span><span class="sxs-lookup"><span data-stu-id="1ff59-106">Members</span></span>
|<span data-ttu-id="1ff59-107">成员</span><span class="sxs-lookup"><span data-stu-id="1ff59-107">Member</span></span>|<span data-ttu-id="1ff59-108">值</span><span class="sxs-lookup"><span data-stu-id="1ff59-108">Value</span></span>|<span data-ttu-id="1ff59-109">说明</span><span class="sxs-lookup"><span data-stu-id="1ff59-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ff59-110">无</span><span class="sxs-lookup"><span data-stu-id="1ff59-110">none</span></span>|<span data-ttu-id="1ff59-111">0</span><span class="sxs-lookup"><span data-stu-id="1ff59-111">0</span></span>|<span data-ttu-id="1ff59-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="1ff59-112">Default status.</span></span>|
|<span data-ttu-id="1ff59-113">正在进行</span><span class="sxs-lookup"><span data-stu-id="1ff59-113">inProgress</span></span>|<span data-ttu-id="1ff59-114">1</span><span class="sxs-lookup"><span data-stu-id="1ff59-114">1</span></span>|<span data-ttu-id="1ff59-115">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="1ff59-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="1ff59-116">完成</span><span class="sxs-lookup"><span data-stu-id="1ff59-116">completed</span></span>|<span data-ttu-id="1ff59-117">2</span><span class="sxs-lookup"><span data-stu-id="1ff59-117">2</span></span>|<span data-ttu-id="1ff59-118">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="1ff59-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="1ff59-119">failed</span><span class="sxs-lookup"><span data-stu-id="1ff59-119">failed</span></span>|<span data-ttu-id="1ff59-120">3</span><span class="sxs-lookup"><span data-stu-id="1ff59-120">3</span></span>|<span data-ttu-id="1ff59-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="1ff59-121">Last Sync failed.</span></span>|



