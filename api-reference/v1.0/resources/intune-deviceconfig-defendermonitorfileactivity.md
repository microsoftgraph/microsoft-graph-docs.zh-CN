---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
ms.openlocfilehash: 7784671f69712ce06a5aefa75048391cb097a89c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011373"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="5e962-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5e962-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="5e962-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5e962-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e962-105">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="5e962-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="5e962-106">成员</span><span class="sxs-lookup"><span data-stu-id="5e962-106">Members</span></span>
|<span data-ttu-id="5e962-107">成员</span><span class="sxs-lookup"><span data-stu-id="5e962-107">Member</span></span>|<span data-ttu-id="5e962-108">值</span><span class="sxs-lookup"><span data-stu-id="5e962-108">Value</span></span>|<span data-ttu-id="5e962-109">说明</span><span class="sxs-lookup"><span data-stu-id="5e962-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e962-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="5e962-110">userDefined</span></span>|<span data-ttu-id="5e962-111">0</span><span class="sxs-lookup"><span data-stu-id="5e962-111">0</span></span>|<span data-ttu-id="5e962-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="5e962-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="5e962-113">禁用</span><span class="sxs-lookup"><span data-stu-id="5e962-113">disable</span></span>|<span data-ttu-id="5e962-114">1</span><span class="sxs-lookup"><span data-stu-id="5e962-114">1</span></span>|<span data-ttu-id="5e962-115">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="5e962-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="5e962-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="5e962-116">monitorAllFiles</span></span>|<span data-ttu-id="5e962-117">2</span><span class="sxs-lookup"><span data-stu-id="5e962-117">2</span></span>|<span data-ttu-id="5e962-118">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="5e962-118">Monitor all files.</span></span>|
|<span data-ttu-id="5e962-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="5e962-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="5e962-120">3</span><span class="sxs-lookup"><span data-stu-id="5e962-120">3</span></span>| <span data-ttu-id="5e962-121">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="5e962-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="5e962-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="5e962-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="5e962-123">4</span><span class="sxs-lookup"><span data-stu-id="5e962-123">4</span></span>|<span data-ttu-id="5e962-124">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="5e962-124">Monitor outgoing files only.</span></span>|



