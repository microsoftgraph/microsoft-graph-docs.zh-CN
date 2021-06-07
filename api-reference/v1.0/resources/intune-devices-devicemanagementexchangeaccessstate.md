---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备Exchange访问状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 897b2e7783b0df6ba286491079d11b18131a4fcd
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751683"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="51b45-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="51b45-103">deviceManagementExchangeAccessState enum type</span></span>

<span data-ttu-id="51b45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51b45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="51b45-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="51b45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51b45-106">设备Exchange访问状态。</span><span class="sxs-lookup"><span data-stu-id="51b45-106">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="51b45-107">成员</span><span class="sxs-lookup"><span data-stu-id="51b45-107">Members</span></span>
|<span data-ttu-id="51b45-108">成员</span><span class="sxs-lookup"><span data-stu-id="51b45-108">Member</span></span>|<span data-ttu-id="51b45-109">值</span><span class="sxs-lookup"><span data-stu-id="51b45-109">Value</span></span>|<span data-ttu-id="51b45-110">Description</span><span class="sxs-lookup"><span data-stu-id="51b45-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51b45-111">无</span><span class="sxs-lookup"><span data-stu-id="51b45-111">none</span></span>|<span data-ttu-id="51b45-112">0</span><span class="sxs-lookup"><span data-stu-id="51b45-112">0</span></span>|<span data-ttu-id="51b45-113">未从用户发现任何Exchange</span><span class="sxs-lookup"><span data-stu-id="51b45-113">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="51b45-114">unknown</span><span class="sxs-lookup"><span data-stu-id="51b45-114">unknown</span></span>|<span data-ttu-id="51b45-115">1</span><span class="sxs-lookup"><span data-stu-id="51b45-115">1</span></span>|<span data-ttu-id="51b45-116">设备访问状态Exchange未知</span><span class="sxs-lookup"><span data-stu-id="51b45-116">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="51b45-117">allowed</span><span class="sxs-lookup"><span data-stu-id="51b45-117">allowed</span></span>|<span data-ttu-id="51b45-118">2</span><span class="sxs-lookup"><span data-stu-id="51b45-118">2</span></span>|<span data-ttu-id="51b45-119">设备有权访问Exchange</span><span class="sxs-lookup"><span data-stu-id="51b45-119">Device has access to Exchange</span></span>|
|<span data-ttu-id="51b45-120">blocked</span><span class="sxs-lookup"><span data-stu-id="51b45-120">blocked</span></span>|<span data-ttu-id="51b45-121">3</span><span class="sxs-lookup"><span data-stu-id="51b45-121">3</span></span>|<span data-ttu-id="51b45-122">设备在设备Exchange</span><span class="sxs-lookup"><span data-stu-id="51b45-122">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="51b45-123">quarantined</span><span class="sxs-lookup"><span data-stu-id="51b45-123">quarantined</span></span>|<span data-ttu-id="51b45-124">4 </span><span class="sxs-lookup"><span data-stu-id="51b45-124">4</span></span>|<span data-ttu-id="51b45-125">设备已隔离Exchange</span><span class="sxs-lookup"><span data-stu-id="51b45-125">Device is Quarantined in Exchange</span></span>|




