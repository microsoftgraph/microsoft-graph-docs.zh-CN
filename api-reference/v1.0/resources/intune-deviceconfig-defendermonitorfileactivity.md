---
title: defenderMonitorFileActivity 枚举类型
description: 监视文件活动的可能值。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a50ee70da2a36e8bdd773235ccd5e9b227a0d01f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758881"
---
# <a name="defendermonitorfileactivity-enum-type"></a><span data-ttu-id="e94cc-103">defenderMonitorFileActivity 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e94cc-103">defenderMonitorFileActivity enum type</span></span>

<span data-ttu-id="e94cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e94cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e94cc-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e94cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e94cc-106">监视文件活动的可能值。</span><span class="sxs-lookup"><span data-stu-id="e94cc-106">Possible values for monitoring file activity.</span></span>

## <a name="members"></a><span data-ttu-id="e94cc-107">成员</span><span class="sxs-lookup"><span data-stu-id="e94cc-107">Members</span></span>
|<span data-ttu-id="e94cc-108">成员</span><span class="sxs-lookup"><span data-stu-id="e94cc-108">Member</span></span>|<span data-ttu-id="e94cc-109">值</span><span class="sxs-lookup"><span data-stu-id="e94cc-109">Value</span></span>|<span data-ttu-id="e94cc-110">说明</span><span class="sxs-lookup"><span data-stu-id="e94cc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e94cc-111">userDefined</span><span class="sxs-lookup"><span data-stu-id="e94cc-111">userDefined</span></span>|<span data-ttu-id="e94cc-112">0</span><span class="sxs-lookup"><span data-stu-id="e94cc-112">0</span></span>|<span data-ttu-id="e94cc-113">用户定义，默认值，无意图。</span><span class="sxs-lookup"><span data-stu-id="e94cc-113">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="e94cc-114">disable</span><span class="sxs-lookup"><span data-stu-id="e94cc-114">disable</span></span>|<span data-ttu-id="e94cc-115">1</span><span class="sxs-lookup"><span data-stu-id="e94cc-115">1</span></span>|<span data-ttu-id="e94cc-116">禁用监视文件活动。</span><span class="sxs-lookup"><span data-stu-id="e94cc-116">Disable monitoring file activity.</span></span>|
|<span data-ttu-id="e94cc-117">monitorAllFiles</span><span class="sxs-lookup"><span data-stu-id="e94cc-117">monitorAllFiles</span></span>|<span data-ttu-id="e94cc-118">2</span><span class="sxs-lookup"><span data-stu-id="e94cc-118">2</span></span>|<span data-ttu-id="e94cc-119">监视所有文件。</span><span class="sxs-lookup"><span data-stu-id="e94cc-119">Monitor all files.</span></span>|
|<span data-ttu-id="e94cc-120">monitorIncomingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="e94cc-120">monitorIncomingFilesOnly</span></span>|<span data-ttu-id="e94cc-121">3</span><span class="sxs-lookup"><span data-stu-id="e94cc-121">3</span></span>| <span data-ttu-id="e94cc-122">仅监视传入文件。</span><span class="sxs-lookup"><span data-stu-id="e94cc-122">Monitor incoming files only.</span></span>|
|<span data-ttu-id="e94cc-123">monitorOutgoingFilesOnly</span><span class="sxs-lookup"><span data-stu-id="e94cc-123">monitorOutgoingFilesOnly</span></span>|<span data-ttu-id="e94cc-124">4 </span><span class="sxs-lookup"><span data-stu-id="e94cc-124">4</span></span>|<span data-ttu-id="e94cc-125">仅监视传出文件。</span><span class="sxs-lookup"><span data-stu-id="e94cc-125">Monitor outgoing files only.</span></span>|




