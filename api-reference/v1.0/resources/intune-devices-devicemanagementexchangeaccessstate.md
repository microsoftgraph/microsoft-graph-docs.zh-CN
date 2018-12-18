---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备 Exchange 访问状态。
author: tfitzmac
ms.openlocfilehash: 37db054314375411dc237746ca6ca3bdb99e9016
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27328719"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="18715-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="18715-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="18715-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="18715-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="18715-105">设备 Exchange 访问状态。</span><span class="sxs-lookup"><span data-stu-id="18715-105">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="18715-106">成员</span><span class="sxs-lookup"><span data-stu-id="18715-106">Members</span></span>
|<span data-ttu-id="18715-107">成员</span><span class="sxs-lookup"><span data-stu-id="18715-107">Member</span></span>|<span data-ttu-id="18715-108">值</span><span class="sxs-lookup"><span data-stu-id="18715-108">Value</span></span>|<span data-ttu-id="18715-109">说明</span><span class="sxs-lookup"><span data-stu-id="18715-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="18715-110">无</span><span class="sxs-lookup"><span data-stu-id="18715-110">none</span></span>|<span data-ttu-id="18715-111">0</span><span class="sxs-lookup"><span data-stu-id="18715-111">0</span></span>|<span data-ttu-id="18715-112">从 Exchange 发现没有访问状态</span><span class="sxs-lookup"><span data-stu-id="18715-112">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="18715-113">unknown</span><span class="sxs-lookup"><span data-stu-id="18715-113">unknown</span></span>|<span data-ttu-id="18715-114">1</span><span class="sxs-lookup"><span data-stu-id="18715-114">1</span></span>|<span data-ttu-id="18715-115">到 Exchange 的设备访问状态是未知</span><span class="sxs-lookup"><span data-stu-id="18715-115">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="18715-116">允许</span><span class="sxs-lookup"><span data-stu-id="18715-116">allowed</span></span>|<span data-ttu-id="18715-117">2</span><span class="sxs-lookup"><span data-stu-id="18715-117">2</span></span>|<span data-ttu-id="18715-118">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="18715-118">Device has access to Exchange</span></span>|
|<span data-ttu-id="18715-119">已阻止</span><span class="sxs-lookup"><span data-stu-id="18715-119">blocked</span></span>|<span data-ttu-id="18715-120">3</span><span class="sxs-lookup"><span data-stu-id="18715-120">3</span></span>|<span data-ttu-id="18715-121">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="18715-121">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="18715-122">隔离</span><span class="sxs-lookup"><span data-stu-id="18715-122">quarantined</span></span>|<span data-ttu-id="18715-123">4</span><span class="sxs-lookup"><span data-stu-id="18715-123">4</span></span>|<span data-ttu-id="18715-124">在 Exchange 隔离设备</span><span class="sxs-lookup"><span data-stu-id="18715-124">Device is Quarantined in Exchange</span></span>|



