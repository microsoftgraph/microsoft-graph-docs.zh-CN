---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: tfitzmac
ms.openlocfilehash: 8f163c5186c1fc8dac13a22d730870c52df66a06
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320795"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="ed819-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ed819-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="ed819-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ed819-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ed819-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ed819-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ed819-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ed819-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ed819-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="ed819-107">Access Level in Exchange.</span></span>
## <a name="members"></a><span data-ttu-id="ed819-108">成员</span><span class="sxs-lookup"><span data-stu-id="ed819-108">Members</span></span>
|<span data-ttu-id="ed819-109">成员</span><span class="sxs-lookup"><span data-stu-id="ed819-109">Member</span></span>|<span data-ttu-id="ed819-110">值</span><span class="sxs-lookup"><span data-stu-id="ed819-110">Value</span></span>|<span data-ttu-id="ed819-111">说明</span><span class="sxs-lookup"><span data-stu-id="ed819-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed819-112">无</span><span class="sxs-lookup"><span data-stu-id="ed819-112">none</span></span>|<span data-ttu-id="ed819-113">0</span><span class="sxs-lookup"><span data-stu-id="ed819-113">0</span></span>|<span data-ttu-id="ed819-114">已在 Exchange 中不配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="ed819-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="ed819-115">允许</span><span class="sxs-lookup"><span data-stu-id="ed819-115">allow</span></span>|<span data-ttu-id="ed819-116">1</span><span class="sxs-lookup"><span data-stu-id="ed819-116">1</span></span>|<span data-ttu-id="ed819-117">允许 Exchange 设备访问。</span><span class="sxs-lookup"><span data-stu-id="ed819-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="ed819-118">阻止</span><span class="sxs-lookup"><span data-stu-id="ed819-118">block</span></span>|<span data-ttu-id="ed819-119">2</span><span class="sxs-lookup"><span data-stu-id="ed819-119">2</span></span>|<span data-ttu-id="ed819-120">阻止访问 Exchange 的设备。</span><span class="sxs-lookup"><span data-stu-id="ed819-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="ed819-121">隔离</span><span class="sxs-lookup"><span data-stu-id="ed819-121">quarantine</span></span>|<span data-ttu-id="ed819-122">3</span><span class="sxs-lookup"><span data-stu-id="ed819-122">3</span></span>|<span data-ttu-id="ed819-123">在 Exchange 隔离设备。</span><span class="sxs-lookup"><span data-stu-id="ed819-123">Quarantine the device in Exchange.</span></span>|





