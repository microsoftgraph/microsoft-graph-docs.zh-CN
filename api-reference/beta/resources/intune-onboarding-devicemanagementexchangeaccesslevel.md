---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 1d9654e526aec7263f12d0fdcb3af8c68f7ba20e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950030"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="3ce2b-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3ce2b-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="3ce2b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3ce2b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3ce2b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3ce2b-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-107">Access Level in Exchange.</span></span>
## <a name="members"></a><span data-ttu-id="3ce2b-108">成员</span><span class="sxs-lookup"><span data-stu-id="3ce2b-108">Members</span></span>
|<span data-ttu-id="3ce2b-109">成员</span><span class="sxs-lookup"><span data-stu-id="3ce2b-109">Member</span></span>|<span data-ttu-id="3ce2b-110">值</span><span class="sxs-lookup"><span data-stu-id="3ce2b-110">Value</span></span>|<span data-ttu-id="3ce2b-111">Description</span><span class="sxs-lookup"><span data-stu-id="3ce2b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ce2b-112">无</span><span class="sxs-lookup"><span data-stu-id="3ce2b-112">none</span></span>|<span data-ttu-id="3ce2b-113">0</span><span class="sxs-lookup"><span data-stu-id="3ce2b-113">0</span></span>|<span data-ttu-id="3ce2b-114">已在 Exchange 中不配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="3ce2b-115">允许</span><span class="sxs-lookup"><span data-stu-id="3ce2b-115">allow</span></span>|<span data-ttu-id="3ce2b-116">1</span><span class="sxs-lookup"><span data-stu-id="3ce2b-116">1</span></span>|<span data-ttu-id="3ce2b-117">允许 Exchange 设备访问。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="3ce2b-118">阻止</span><span class="sxs-lookup"><span data-stu-id="3ce2b-118">block</span></span>|<span data-ttu-id="3ce2b-119">2</span><span class="sxs-lookup"><span data-stu-id="3ce2b-119">2</span></span>|<span data-ttu-id="3ce2b-120">阻止访问 Exchange 的设备。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="3ce2b-121">隔离</span><span class="sxs-lookup"><span data-stu-id="3ce2b-121">quarantine</span></span>|<span data-ttu-id="3ce2b-122">3</span><span class="sxs-lookup"><span data-stu-id="3ce2b-122">3</span></span>|<span data-ttu-id="3ce2b-123">在 Exchange 隔离设备。</span><span class="sxs-lookup"><span data-stu-id="3ce2b-123">Quarantine the device in Exchange.</span></span>|





