---
title: defenderMonitorFileActivity 枚举类型
description: 用于监控文件活动的可能值。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d9b0f91d0a2d802fd573d7825da016dc8850e941
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414954"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="8d0a2-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8d0a2-103">defenderMonitorFileActivity enum type</span></span>

> <span data-ttu-id="8d0a2-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8d0a2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d0a2-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8d0a2-107">用于监控文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-107">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="8d0a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="8d0a2-108">Members</span></span>
|<span data-ttu-id="8d0a2-109">成员</span><span class="sxs-lookup"><span data-stu-id="8d0a2-109">Member</span></span>|<span data-ttu-id="8d0a2-110">值</span><span class="sxs-lookup"><span data-stu-id="8d0a2-110">Value</span></span>|<span data-ttu-id="8d0a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="8d0a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d0a2-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="8d0a2-112">userDefined</span></span>|<span data-ttu-id="8d0a2-113">0</span><span class="sxs-lookup"><span data-stu-id="8d0a2-113">0</span></span>|<span data-ttu-id="8d0a2-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="8d0a2-115">禁用</span><span class="sxs-lookup"><span data-stu-id="8d0a2-115">disable</span></span>|<span data-ttu-id="8d0a2-116">1</span><span class="sxs-lookup"><span data-stu-id="8d0a2-116">1</span></span>|<span data-ttu-id="8d0a2-117">禁用监控文件活动。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-117">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="8d0a2-118">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="8d0a2-118">monitorAllFiles</span></span>|<span data-ttu-id="8d0a2-119">2</span><span class="sxs-lookup"><span data-stu-id="8d0a2-119">2</span></span>|<span data-ttu-id="8d0a2-120">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-120">Monitor all files.</span></span>|
|<span data-ttu-id="8d0a2-121">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="8d0a2-121">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="8d0a2-122">3</span><span class="sxs-lookup"><span data-stu-id="8d0a2-122">3</span></span>| <span data-ttu-id="8d0a2-123">监视传入的文件。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-123">Monitor incoming files only.</span></span>|
|<span data-ttu-id="8d0a2-124">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="8d0a2-124">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="8d0a2-125">4</span><span class="sxs-lookup"><span data-stu-id="8d0a2-125">4</span></span>|<span data-ttu-id="8d0a2-126">监视传出的文件。</span><span class="sxs-lookup"><span data-stu-id="8d0a2-126">Monitor outgoing files only.</span></span>|




