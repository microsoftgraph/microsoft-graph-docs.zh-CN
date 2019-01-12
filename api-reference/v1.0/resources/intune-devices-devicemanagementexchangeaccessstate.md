---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备 Exchange 访问状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: dbfa7b9396a1100f2e3c7e4e78cf697233d840cc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27947013"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="ffac2-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ffac2-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="ffac2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ffac2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffac2-105">设备 Exchange 访问状态。</span><span class="sxs-lookup"><span data-stu-id="ffac2-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="ffac2-106">成员</span><span class="sxs-lookup"><span data-stu-id="ffac2-106">Members</span></span>
|<span data-ttu-id="ffac2-107">成员</span><span class="sxs-lookup"><span data-stu-id="ffac2-107">Member</span></span>|<span data-ttu-id="ffac2-108">值</span><span class="sxs-lookup"><span data-stu-id="ffac2-108">Value</span></span>|<span data-ttu-id="ffac2-109">Description</span><span class="sxs-lookup"><span data-stu-id="ffac2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffac2-110">无</span><span class="sxs-lookup"><span data-stu-id="ffac2-110">none</span></span>|<span data-ttu-id="ffac2-111">0</span><span class="sxs-lookup"><span data-stu-id="ffac2-111">0</span></span>|<span data-ttu-id="ffac2-112">从 Exchange 发现没有访问状态</span><span class="sxs-lookup"><span data-stu-id="ffac2-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="ffac2-113">unknown</span><span class="sxs-lookup"><span data-stu-id="ffac2-113">unknown</span></span>|<span data-ttu-id="ffac2-114">1</span><span class="sxs-lookup"><span data-stu-id="ffac2-114">1</span></span>|<span data-ttu-id="ffac2-115">到 Exchange 的设备访问状态是未知</span><span class="sxs-lookup"><span data-stu-id="ffac2-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="ffac2-116">允许</span><span class="sxs-lookup"><span data-stu-id="ffac2-116">allowed</span></span>|<span data-ttu-id="ffac2-117">2</span><span class="sxs-lookup"><span data-stu-id="ffac2-117">2</span></span>|<span data-ttu-id="ffac2-118">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="ffac2-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="ffac2-119">已阻止</span><span class="sxs-lookup"><span data-stu-id="ffac2-119">blocked</span></span>|<span data-ttu-id="ffac2-120">3</span><span class="sxs-lookup"><span data-stu-id="ffac2-120">3</span></span>|<span data-ttu-id="ffac2-121">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="ffac2-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="ffac2-122">隔离</span><span class="sxs-lookup"><span data-stu-id="ffac2-122">quarantined</span></span>|<span data-ttu-id="ffac2-123">4</span><span class="sxs-lookup"><span data-stu-id="ffac2-123">4</span></span>|<span data-ttu-id="ffac2-124">在 Exchange 隔离设备</span><span class="sxs-lookup"><span data-stu-id="ffac2-124">Device is Quarantined in Exchange</span></span>|



