---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备 Exchange 访问状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f66f8372b5bd087ad620fa86d8e0beff8b3eb3a0
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29401066"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="37281-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="37281-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="37281-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="37281-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="37281-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="37281-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="37281-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37281-107">设备 Exchange 访问状态。</span><span class="sxs-lookup"><span data-stu-id="37281-107">Device Exchange Access State.</span></span>

## <a name="members"></a><span data-ttu-id="37281-108">成员</span><span class="sxs-lookup"><span data-stu-id="37281-108">Members</span></span>
|<span data-ttu-id="37281-109">成员</span><span class="sxs-lookup"><span data-stu-id="37281-109">Member</span></span>|<span data-ttu-id="37281-110">值</span><span class="sxs-lookup"><span data-stu-id="37281-110">Value</span></span>|<span data-ttu-id="37281-111">说明</span><span class="sxs-lookup"><span data-stu-id="37281-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37281-112">无</span><span class="sxs-lookup"><span data-stu-id="37281-112">none</span></span>|<span data-ttu-id="37281-113">0</span><span class="sxs-lookup"><span data-stu-id="37281-113">0</span></span>|<span data-ttu-id="37281-114">从 Exchange 发现没有访问状态</span><span class="sxs-lookup"><span data-stu-id="37281-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="37281-115">unknown</span><span class="sxs-lookup"><span data-stu-id="37281-115">unknown</span></span>|<span data-ttu-id="37281-116">1</span><span class="sxs-lookup"><span data-stu-id="37281-116">1</span></span>|<span data-ttu-id="37281-117">到 Exchange 的设备访问状态是未知</span><span class="sxs-lookup"><span data-stu-id="37281-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="37281-118">允许</span><span class="sxs-lookup"><span data-stu-id="37281-118">allowed</span></span>|<span data-ttu-id="37281-119">2</span><span class="sxs-lookup"><span data-stu-id="37281-119">2</span></span>|<span data-ttu-id="37281-120">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="37281-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="37281-121">已阻止</span><span class="sxs-lookup"><span data-stu-id="37281-121">blocked</span></span>|<span data-ttu-id="37281-122">3</span><span class="sxs-lookup"><span data-stu-id="37281-122">3</span></span>|<span data-ttu-id="37281-123">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="37281-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="37281-124">隔离</span><span class="sxs-lookup"><span data-stu-id="37281-124">quarantined</span></span>|<span data-ttu-id="37281-125">4</span><span class="sxs-lookup"><span data-stu-id="37281-125">4</span></span>|<span data-ttu-id="37281-126">在 Exchange 隔离设备</span><span class="sxs-lookup"><span data-stu-id="37281-126">Device is Quarantined in Exchange</span></span>|




