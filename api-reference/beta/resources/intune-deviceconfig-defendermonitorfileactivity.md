---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
ms.openlocfilehash: ec10458cbb76a45caff8d64f6c4047d5645094b4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047071"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="ad1b5-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ad1b5-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="ad1b5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad1b5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad1b5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad1b5-107">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="ad1b5-108">成员</span><span class="sxs-lookup"><span data-stu-id="ad1b5-108">Members</span></span>
|<span data-ttu-id="ad1b5-109">成员</span><span class="sxs-lookup"><span data-stu-id="ad1b5-109">Member</span></span>|<span data-ttu-id="ad1b5-110">值</span><span class="sxs-lookup"><span data-stu-id="ad1b5-110">Value</span></span>|<span data-ttu-id="ad1b5-111">说明</span><span class="sxs-lookup"><span data-stu-id="ad1b5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad1b5-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="ad1b5-112">userDefined</span></span>|<span data-ttu-id="ad1b5-113">0</span><span class="sxs-lookup"><span data-stu-id="ad1b5-113">0</span></span>|<span data-ttu-id="ad1b5-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="ad1b5-115">禁用</span><span class="sxs-lookup"><span data-stu-id="ad1b5-115">disable</span></span>|<span data-ttu-id="ad1b5-116">1</span><span class="sxs-lookup"><span data-stu-id="ad1b5-116">1</span></span>|<span data-ttu-id="ad1b5-117">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="ad1b5-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="ad1b5-118">monitorAllFiles</span></span>|<span data-ttu-id="ad1b5-119">2</span><span class="sxs-lookup"><span data-stu-id="ad1b5-119">2</span></span>|<span data-ttu-id="ad1b5-120">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-120">Monitor all files.</span></span>|
|<span data-ttu-id="ad1b5-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="ad1b5-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="ad1b5-122">3</span><span class="sxs-lookup"><span data-stu-id="ad1b5-122">3</span></span>| <span data-ttu-id="ad1b5-123">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="ad1b5-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="ad1b5-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="ad1b5-125">4</span><span class="sxs-lookup"><span data-stu-id="ad1b5-125">4</span></span>|<span data-ttu-id="ad1b5-126">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="ad1b5-126">Monitor outgoing files only.</span></span>|





