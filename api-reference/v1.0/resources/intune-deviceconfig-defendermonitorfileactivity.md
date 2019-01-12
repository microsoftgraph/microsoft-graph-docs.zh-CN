---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: d818264470543d077384f055cf2ef4004e019b26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937115"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="49df7-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49df7-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="49df7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49df7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49df7-105">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="49df7-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="49df7-106">成员</span><span class="sxs-lookup"><span data-stu-id="49df7-106">Members</span></span>
|<span data-ttu-id="49df7-107">成员</span><span class="sxs-lookup"><span data-stu-id="49df7-107">Member</span></span>|<span data-ttu-id="49df7-108">值</span><span class="sxs-lookup"><span data-stu-id="49df7-108">Value</span></span>|<span data-ttu-id="49df7-109">说明</span><span class="sxs-lookup"><span data-stu-id="49df7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49df7-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="49df7-110">userDefined</span></span>|<span data-ttu-id="49df7-111">0</span><span class="sxs-lookup"><span data-stu-id="49df7-111">0</span></span>|<span data-ttu-id="49df7-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="49df7-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="49df7-113">禁用</span><span class="sxs-lookup"><span data-stu-id="49df7-113">disable</span></span>|<span data-ttu-id="49df7-114">1</span><span class="sxs-lookup"><span data-stu-id="49df7-114">1</span></span>|<span data-ttu-id="49df7-115">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="49df7-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="49df7-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="49df7-116">monitorAllFiles</span></span>|<span data-ttu-id="49df7-117">2</span><span class="sxs-lookup"><span data-stu-id="49df7-117">2</span></span>|<span data-ttu-id="49df7-118">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="49df7-118">Monitor all files.</span></span>|
|<span data-ttu-id="49df7-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="49df7-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="49df7-120">3</span><span class="sxs-lookup"><span data-stu-id="49df7-120">3</span></span>| <span data-ttu-id="49df7-121">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="49df7-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="49df7-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="49df7-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="49df7-123">4</span><span class="sxs-lookup"><span data-stu-id="49df7-123">4</span></span>|<span data-ttu-id="49df7-124">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="49df7-124">Monitor outgoing files only.</span></span>|



