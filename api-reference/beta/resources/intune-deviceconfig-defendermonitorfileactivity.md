---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
author: tfitzmac
ms.openlocfilehash: 32b3972f6c4c09117f3b8001038c0316235ea222
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338106"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="cf09b-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cf09b-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="cf09b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cf09b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf09b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cf09b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cf09b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf09b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf09b-107">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="cf09b-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="cf09b-108">成员</span><span class="sxs-lookup"><span data-stu-id="cf09b-108">Members</span></span>
|<span data-ttu-id="cf09b-109">成员</span><span class="sxs-lookup"><span data-stu-id="cf09b-109">Member</span></span>|<span data-ttu-id="cf09b-110">值</span><span class="sxs-lookup"><span data-stu-id="cf09b-110">Value</span></span>|<span data-ttu-id="cf09b-111">说明</span><span class="sxs-lookup"><span data-stu-id="cf09b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf09b-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="cf09b-112">userDefined</span></span>|<span data-ttu-id="cf09b-113">0</span><span class="sxs-lookup"><span data-stu-id="cf09b-113">0</span></span>|<span data-ttu-id="cf09b-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="cf09b-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="cf09b-115">禁用</span><span class="sxs-lookup"><span data-stu-id="cf09b-115">disable</span></span>|<span data-ttu-id="cf09b-116">1</span><span class="sxs-lookup"><span data-stu-id="cf09b-116">1</span></span>|<span data-ttu-id="cf09b-117">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="cf09b-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="cf09b-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="cf09b-118">monitorAllFiles</span></span>|<span data-ttu-id="cf09b-119">2</span><span class="sxs-lookup"><span data-stu-id="cf09b-119">2</span></span>|<span data-ttu-id="cf09b-120">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="cf09b-120">Monitor all files.</span></span>|
|<span data-ttu-id="cf09b-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="cf09b-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="cf09b-122">3</span><span class="sxs-lookup"><span data-stu-id="cf09b-122">3</span></span>| <span data-ttu-id="cf09b-123">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="cf09b-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="cf09b-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="cf09b-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="cf09b-125">4</span><span class="sxs-lookup"><span data-stu-id="cf09b-125">4</span></span>|<span data-ttu-id="cf09b-126">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="cf09b-126">Monitor outgoing files only.</span></span>|





