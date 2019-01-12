---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: df973c06456484263b6346b5eaa48ac466de41f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27967992"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="89dbf-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89dbf-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="89dbf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89dbf-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89dbf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89dbf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="89dbf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="89dbf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="89dbf-107">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="89dbf-107">Possible values for monitoring file activity.</span></span>
## <a name="members"></a><span data-ttu-id="89dbf-108">成员</span><span class="sxs-lookup"><span data-stu-id="89dbf-108">Members</span></span>
|<span data-ttu-id="89dbf-109">成员</span><span class="sxs-lookup"><span data-stu-id="89dbf-109">Member</span></span>|<span data-ttu-id="89dbf-110">值</span><span class="sxs-lookup"><span data-stu-id="89dbf-110">Value</span></span>|<span data-ttu-id="89dbf-111">说明</span><span class="sxs-lookup"><span data-stu-id="89dbf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89dbf-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="89dbf-112">userDefined</span></span>|<span data-ttu-id="89dbf-113">0</span><span class="sxs-lookup"><span data-stu-id="89dbf-113">0</span></span>|<span data-ttu-id="89dbf-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="89dbf-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="89dbf-115">禁用</span><span class="sxs-lookup"><span data-stu-id="89dbf-115">disable</span></span>|<span data-ttu-id="89dbf-116">1</span><span class="sxs-lookup"><span data-stu-id="89dbf-116">1</span></span>|<span data-ttu-id="89dbf-117">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="89dbf-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="89dbf-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="89dbf-118">monitorAllFiles</span></span>|<span data-ttu-id="89dbf-119">2</span><span class="sxs-lookup"><span data-stu-id="89dbf-119">2</span></span>|<span data-ttu-id="89dbf-120">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="89dbf-120">Monitor all files.</span></span>|
|<span data-ttu-id="89dbf-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="89dbf-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="89dbf-122">3</span><span class="sxs-lookup"><span data-stu-id="89dbf-122">3</span></span>| <span data-ttu-id="89dbf-123">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="89dbf-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="89dbf-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="89dbf-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="89dbf-125">4</span><span class="sxs-lookup"><span data-stu-id="89dbf-125">4</span></span>|<span data-ttu-id="89dbf-126">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="89dbf-126">Monitor outgoing files only.</span></span>|





