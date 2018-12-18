---
title: vppTokenSyncStatus 枚举类型
description: 使用 Apple 卷购买计划令牌关联的可能的同步状态。
author: tfitzmac
ms.openlocfilehash: 18a0fcf9f4d22d7904cb76d1fc45d80b14dfc7d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344238"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="ca71a-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ca71a-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="ca71a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca71a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca71a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca71a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca71a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ca71a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca71a-107">使用 Apple 卷购买计划令牌关联的可能的同步状态。</span><span class="sxs-lookup"><span data-stu-id="ca71a-107">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>
## <a name="members"></a><span data-ttu-id="ca71a-108">成员</span><span class="sxs-lookup"><span data-stu-id="ca71a-108">Members</span></span>
|<span data-ttu-id="ca71a-109">成员</span><span class="sxs-lookup"><span data-stu-id="ca71a-109">Member</span></span>|<span data-ttu-id="ca71a-110">值</span><span class="sxs-lookup"><span data-stu-id="ca71a-110">Value</span></span>|<span data-ttu-id="ca71a-111">说明</span><span class="sxs-lookup"><span data-stu-id="ca71a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca71a-112">无</span><span class="sxs-lookup"><span data-stu-id="ca71a-112">none</span></span>|<span data-ttu-id="ca71a-113">0</span><span class="sxs-lookup"><span data-stu-id="ca71a-113">0</span></span>|<span data-ttu-id="ca71a-114">默认状态。</span><span class="sxs-lookup"><span data-stu-id="ca71a-114">Default status.</span></span>|
|<span data-ttu-id="ca71a-115">正在进行</span><span class="sxs-lookup"><span data-stu-id="ca71a-115">inProgress</span></span>|<span data-ttu-id="ca71a-116">1</span><span class="sxs-lookup"><span data-stu-id="ca71a-116">1</span></span>|<span data-ttu-id="ca71a-117">正在进行的上次同步。</span><span class="sxs-lookup"><span data-stu-id="ca71a-117">Last Sync in progress.</span></span>|
|<span data-ttu-id="ca71a-118">完成</span><span class="sxs-lookup"><span data-stu-id="ca71a-118">completed</span></span>|<span data-ttu-id="ca71a-119">2</span><span class="sxs-lookup"><span data-stu-id="ca71a-119">2</span></span>|<span data-ttu-id="ca71a-120">上次同步已成功完成。</span><span class="sxs-lookup"><span data-stu-id="ca71a-120">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="ca71a-121">failed</span><span class="sxs-lookup"><span data-stu-id="ca71a-121">failed</span></span>|<span data-ttu-id="ca71a-122">3</span><span class="sxs-lookup"><span data-stu-id="ca71a-122">3</span></span>|<span data-ttu-id="ca71a-123">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="ca71a-123">Last Sync failed.</span></span>|





