---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2d24aedcd5c09de6e56b3870f8c5b111fbb39513
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29414331"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="a8272-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a8272-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="a8272-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a8272-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a8272-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a8272-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a8272-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a8272-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a8272-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="a8272-107">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="a8272-108">成员</span><span class="sxs-lookup"><span data-stu-id="a8272-108">Members</span></span>
|<span data-ttu-id="a8272-109">成员</span><span class="sxs-lookup"><span data-stu-id="a8272-109">Member</span></span>|<span data-ttu-id="a8272-110">值</span><span class="sxs-lookup"><span data-stu-id="a8272-110">Value</span></span>|<span data-ttu-id="a8272-111">说明</span><span class="sxs-lookup"><span data-stu-id="a8272-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a8272-112">无</span><span class="sxs-lookup"><span data-stu-id="a8272-112">none</span></span>|<span data-ttu-id="a8272-113">0</span><span class="sxs-lookup"><span data-stu-id="a8272-113">0</span></span>|<span data-ttu-id="a8272-114">已在 Exchange 中不配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="a8272-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="a8272-115">允许</span><span class="sxs-lookup"><span data-stu-id="a8272-115">allow</span></span>|<span data-ttu-id="a8272-116">1</span><span class="sxs-lookup"><span data-stu-id="a8272-116">1</span></span>|<span data-ttu-id="a8272-117">允许 Exchange 设备访问。</span><span class="sxs-lookup"><span data-stu-id="a8272-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="a8272-118">阻止</span><span class="sxs-lookup"><span data-stu-id="a8272-118">block</span></span>|<span data-ttu-id="a8272-119">2</span><span class="sxs-lookup"><span data-stu-id="a8272-119">2</span></span>|<span data-ttu-id="a8272-120">阻止访问 Exchange 的设备。</span><span class="sxs-lookup"><span data-stu-id="a8272-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="a8272-121">隔离</span><span class="sxs-lookup"><span data-stu-id="a8272-121">quarantine</span></span>|<span data-ttu-id="a8272-122">3</span><span class="sxs-lookup"><span data-stu-id="a8272-122">3</span></span>|<span data-ttu-id="a8272-123">在 Exchange 隔离设备。</span><span class="sxs-lookup"><span data-stu-id="a8272-123">Quarantine the device in Exchange.</span></span>|




