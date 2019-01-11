---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 1d7b6c921ec40b53339646b2b3b0a91e2d4e8a84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837903"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="88090-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="88090-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="88090-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="88090-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="88090-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88090-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88090-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="88090-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="88090-107">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="88090-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="88090-108">成员</span><span class="sxs-lookup"><span data-stu-id="88090-108">Members</span></span>
|<span data-ttu-id="88090-109">成员</span><span class="sxs-lookup"><span data-stu-id="88090-109">Member</span></span>|<span data-ttu-id="88090-110">值</span><span class="sxs-lookup"><span data-stu-id="88090-110">Value</span></span>|<span data-ttu-id="88090-111">Description</span><span class="sxs-lookup"><span data-stu-id="88090-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88090-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="88090-112">userDefined</span></span>|<span data-ttu-id="88090-113">0</span><span class="sxs-lookup"><span data-stu-id="88090-113">0</span></span>|<span data-ttu-id="88090-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="88090-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="88090-115">禁用</span><span class="sxs-lookup"><span data-stu-id="88090-115">disable</span></span>|<span data-ttu-id="88090-116">1</span><span class="sxs-lookup"><span data-stu-id="88090-116">1</span></span>|<span data-ttu-id="88090-117">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="88090-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="88090-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="88090-118">monitorAllFiles</span></span>|<span data-ttu-id="88090-119">2</span><span class="sxs-lookup"><span data-stu-id="88090-119">2</span></span>|<span data-ttu-id="88090-120">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="88090-120">Monitor all files.</span></span>|
|<span data-ttu-id="88090-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="88090-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="88090-122">3</span><span class="sxs-lookup"><span data-stu-id="88090-122">3</span></span>| <span data-ttu-id="88090-123">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="88090-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="88090-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="88090-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="88090-125">4</span><span class="sxs-lookup"><span data-stu-id="88090-125">4</span></span>|<span data-ttu-id="88090-126">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="88090-126">Monitor outgoing files only.</span></span>|





