---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e8719fd5f07efa9d09dcf88ae02566f331904734
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871685"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="09036-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="09036-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="09036-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="09036-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09036-105">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="09036-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="09036-106">成员</span><span class="sxs-lookup"><span data-stu-id="09036-106">Members</span></span>
|<span data-ttu-id="09036-107">成员</span><span class="sxs-lookup"><span data-stu-id="09036-107">Member</span></span>|<span data-ttu-id="09036-108">值</span><span class="sxs-lookup"><span data-stu-id="09036-108">Value</span></span>|<span data-ttu-id="09036-109">Description</span><span class="sxs-lookup"><span data-stu-id="09036-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09036-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="09036-110">userDefined</span></span>|<span data-ttu-id="09036-111">0</span><span class="sxs-lookup"><span data-stu-id="09036-111">0</span></span>|<span data-ttu-id="09036-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="09036-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="09036-113">禁用</span><span class="sxs-lookup"><span data-stu-id="09036-113">disable</span></span>|<span data-ttu-id="09036-114">1</span><span class="sxs-lookup"><span data-stu-id="09036-114">1</span></span>|<span data-ttu-id="09036-115">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="09036-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="09036-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="09036-116">monitorAllFiles</span></span>|<span data-ttu-id="09036-117">2</span><span class="sxs-lookup"><span data-stu-id="09036-117">2</span></span>|<span data-ttu-id="09036-118">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="09036-118">Monitor all files.</span></span>|
|<span data-ttu-id="09036-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="09036-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="09036-120">3</span><span class="sxs-lookup"><span data-stu-id="09036-120">3</span></span>| <span data-ttu-id="09036-121">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="09036-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="09036-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="09036-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="09036-123">4</span><span class="sxs-lookup"><span data-stu-id="09036-123">4</span></span>|<span data-ttu-id="09036-124">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="09036-124">Monitor outgoing files only.</span></span>|



