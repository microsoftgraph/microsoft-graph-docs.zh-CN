---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备 Exchange 访问状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 73559bf01cfc619e38a30b0393a7d7f3a8754321
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889087"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="9ee92-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9ee92-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="9ee92-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9ee92-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9ee92-105">设备 Exchange 访问状态。</span><span class="sxs-lookup"><span data-stu-id="9ee92-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="9ee92-106">成员</span><span class="sxs-lookup"><span data-stu-id="9ee92-106">Members</span></span>
|<span data-ttu-id="9ee92-107">成员</span><span class="sxs-lookup"><span data-stu-id="9ee92-107">Member</span></span>|<span data-ttu-id="9ee92-108">值</span><span class="sxs-lookup"><span data-stu-id="9ee92-108">Value</span></span>|<span data-ttu-id="9ee92-109">Description</span><span class="sxs-lookup"><span data-stu-id="9ee92-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ee92-110">无</span><span class="sxs-lookup"><span data-stu-id="9ee92-110">none</span></span>|<span data-ttu-id="9ee92-111">0</span><span class="sxs-lookup"><span data-stu-id="9ee92-111">0</span></span>|<span data-ttu-id="9ee92-112">从 Exchange 发现没有访问状态</span><span class="sxs-lookup"><span data-stu-id="9ee92-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="9ee92-113">unknown</span><span class="sxs-lookup"><span data-stu-id="9ee92-113">unknown</span></span>|<span data-ttu-id="9ee92-114">1</span><span class="sxs-lookup"><span data-stu-id="9ee92-114">1</span></span>|<span data-ttu-id="9ee92-115">到 Exchange 的设备访问状态是未知</span><span class="sxs-lookup"><span data-stu-id="9ee92-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="9ee92-116">允许</span><span class="sxs-lookup"><span data-stu-id="9ee92-116">allowed</span></span>|<span data-ttu-id="9ee92-117">2</span><span class="sxs-lookup"><span data-stu-id="9ee92-117">2</span></span>|<span data-ttu-id="9ee92-118">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="9ee92-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="9ee92-119">已阻止</span><span class="sxs-lookup"><span data-stu-id="9ee92-119">blocked</span></span>|<span data-ttu-id="9ee92-120">3</span><span class="sxs-lookup"><span data-stu-id="9ee92-120">3</span></span>|<span data-ttu-id="9ee92-121">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="9ee92-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="9ee92-122">隔离</span><span class="sxs-lookup"><span data-stu-id="9ee92-122">quarantined</span></span>|<span data-ttu-id="9ee92-123">4</span><span class="sxs-lookup"><span data-stu-id="9ee92-123">4</span></span>|<span data-ttu-id="9ee92-124">在 Exchange 隔离设备</span><span class="sxs-lookup"><span data-stu-id="9ee92-124">Device is Quarantined in Exchange</span></span>|



