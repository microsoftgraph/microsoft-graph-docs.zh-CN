---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 03588e51a301bfcc4aac5eb3f9c0bfe0fbba9ea9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27889549"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="4968a-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4968a-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="4968a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="4968a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4968a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="4968a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4968a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="4968a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4968a-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="4968a-107">Access Level in Exchange.</span></span>
## <a name="members"></a><span data-ttu-id="4968a-108">成员</span><span class="sxs-lookup"><span data-stu-id="4968a-108">Members</span></span>
|<span data-ttu-id="4968a-109">成员</span><span class="sxs-lookup"><span data-stu-id="4968a-109">Member</span></span>|<span data-ttu-id="4968a-110">值</span><span class="sxs-lookup"><span data-stu-id="4968a-110">Value</span></span>|<span data-ttu-id="4968a-111">Description</span><span class="sxs-lookup"><span data-stu-id="4968a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4968a-112">无</span><span class="sxs-lookup"><span data-stu-id="4968a-112">none</span></span>|<span data-ttu-id="4968a-113">0</span><span class="sxs-lookup"><span data-stu-id="4968a-113">0</span></span>|<span data-ttu-id="4968a-114">已在 Exchange 中不配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="4968a-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="4968a-115">允许</span><span class="sxs-lookup"><span data-stu-id="4968a-115">allow</span></span>|<span data-ttu-id="4968a-116">1</span><span class="sxs-lookup"><span data-stu-id="4968a-116">1</span></span>|<span data-ttu-id="4968a-117">允许 Exchange 设备访问。</span><span class="sxs-lookup"><span data-stu-id="4968a-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="4968a-118">阻止</span><span class="sxs-lookup"><span data-stu-id="4968a-118">block</span></span>|<span data-ttu-id="4968a-119">2</span><span class="sxs-lookup"><span data-stu-id="4968a-119">2</span></span>|<span data-ttu-id="4968a-120">阻止访问 Exchange 的设备。</span><span class="sxs-lookup"><span data-stu-id="4968a-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="4968a-121">隔离</span><span class="sxs-lookup"><span data-stu-id="4968a-121">quarantine</span></span>|<span data-ttu-id="4968a-122">3</span><span class="sxs-lookup"><span data-stu-id="4968a-122">3</span></span>|<span data-ttu-id="4968a-123">在 Exchange 隔离设备。</span><span class="sxs-lookup"><span data-stu-id="4968a-123">Quarantine the device in Exchange.</span></span>|





