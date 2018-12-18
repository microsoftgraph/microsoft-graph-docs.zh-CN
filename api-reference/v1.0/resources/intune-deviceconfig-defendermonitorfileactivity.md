---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
author: tfitzmac
ms.openlocfilehash: 87c8656c09482763b5e09f0ca746c7bddd069a21
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314761"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="69f07-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="69f07-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="69f07-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="69f07-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="69f07-105">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="69f07-105">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="69f07-106">成员</span><span class="sxs-lookup"><span data-stu-id="69f07-106">Members</span></span>
|<span data-ttu-id="69f07-107">成员</span><span class="sxs-lookup"><span data-stu-id="69f07-107">Member</span></span>|<span data-ttu-id="69f07-108">值</span><span class="sxs-lookup"><span data-stu-id="69f07-108">Value</span></span>|<span data-ttu-id="69f07-109">说明</span><span class="sxs-lookup"><span data-stu-id="69f07-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69f07-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="69f07-110">userDefined</span></span>|<span data-ttu-id="69f07-111">0</span><span class="sxs-lookup"><span data-stu-id="69f07-111">0</span></span>|<span data-ttu-id="69f07-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="69f07-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="69f07-113">禁用</span><span class="sxs-lookup"><span data-stu-id="69f07-113">disable</span></span>|<span data-ttu-id="69f07-114">1</span><span class="sxs-lookup"><span data-stu-id="69f07-114">1</span></span>|<span data-ttu-id="69f07-115">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="69f07-115">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="69f07-116">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="69f07-116">monitorAllFiles</span></span>|<span data-ttu-id="69f07-117">2</span><span class="sxs-lookup"><span data-stu-id="69f07-117">2</span></span>|<span data-ttu-id="69f07-118">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="69f07-118">Monitor all files.</span></span>|
|<span data-ttu-id="69f07-119">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="69f07-119">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="69f07-120">3</span><span class="sxs-lookup"><span data-stu-id="69f07-120">3</span></span>| <span data-ttu-id="69f07-121">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="69f07-121">Monitor incoming files only.</span></span>|
|<span data-ttu-id="69f07-122">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="69f07-122">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="69f07-123">4</span><span class="sxs-lookup"><span data-stu-id="69f07-123">4</span></span>|<span data-ttu-id="69f07-124">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="69f07-124">Monitor outgoing files only.</span></span>|



