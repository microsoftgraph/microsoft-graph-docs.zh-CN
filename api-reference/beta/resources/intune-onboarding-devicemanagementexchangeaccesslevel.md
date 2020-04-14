---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e0132fde18857d9e8adc5d6ddfd2bd13f4b5188d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43455048"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="89b16-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="89b16-103">deviceManagementExchangeAccessLevel enum type</span></span>

<span data-ttu-id="89b16-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89b16-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="89b16-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="89b16-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="89b16-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="89b16-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="89b16-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="89b16-107">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="89b16-108">成员</span><span class="sxs-lookup"><span data-stu-id="89b16-108">Members</span></span>
|<span data-ttu-id="89b16-109">成员</span><span class="sxs-lookup"><span data-stu-id="89b16-109">Member</span></span>|<span data-ttu-id="89b16-110">值</span><span class="sxs-lookup"><span data-stu-id="89b16-110">Value</span></span>|<span data-ttu-id="89b16-111">说明</span><span class="sxs-lookup"><span data-stu-id="89b16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="89b16-112">无</span><span class="sxs-lookup"><span data-stu-id="89b16-112">none</span></span>|<span data-ttu-id="89b16-113">0</span><span class="sxs-lookup"><span data-stu-id="89b16-113">0</span></span>|<span data-ttu-id="89b16-114">未在 Exchange 中配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="89b16-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="89b16-115">允许</span><span class="sxs-lookup"><span data-stu-id="89b16-115">allow</span></span>|<span data-ttu-id="89b16-116">1</span><span class="sxs-lookup"><span data-stu-id="89b16-116">1</span></span>|<span data-ttu-id="89b16-117">允许设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="89b16-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="89b16-118">数据</span><span class="sxs-lookup"><span data-stu-id="89b16-118">block</span></span>|<span data-ttu-id="89b16-119">双面</span><span class="sxs-lookup"><span data-stu-id="89b16-119">2</span></span>|<span data-ttu-id="89b16-120">阻止设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="89b16-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="89b16-121">隔离</span><span class="sxs-lookup"><span data-stu-id="89b16-121">quarantine</span></span>|<span data-ttu-id="89b16-122">第三章</span><span class="sxs-lookup"><span data-stu-id="89b16-122">3</span></span>|<span data-ttu-id="89b16-123">隔离 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="89b16-123">Quarantine the device in Exchange.</span></span>|



