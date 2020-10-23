---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0ce4a0db405ece59222360557d24fa655e76d998
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48707652"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="84e12-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="84e12-103">deviceManagementExchangeAccessLevel enum type</span></span>

<span data-ttu-id="84e12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84e12-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84e12-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84e12-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84e12-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84e12-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84e12-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="84e12-107">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="84e12-108">成员</span><span class="sxs-lookup"><span data-stu-id="84e12-108">Members</span></span>
|<span data-ttu-id="84e12-109">成员</span><span class="sxs-lookup"><span data-stu-id="84e12-109">Member</span></span>|<span data-ttu-id="84e12-110">值</span><span class="sxs-lookup"><span data-stu-id="84e12-110">Value</span></span>|<span data-ttu-id="84e12-111">说明</span><span class="sxs-lookup"><span data-stu-id="84e12-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84e12-112">无</span><span class="sxs-lookup"><span data-stu-id="84e12-112">none</span></span>|<span data-ttu-id="84e12-113">0</span><span class="sxs-lookup"><span data-stu-id="84e12-113">0</span></span>|<span data-ttu-id="84e12-114">未在 Exchange 中配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="84e12-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="84e12-115">允许</span><span class="sxs-lookup"><span data-stu-id="84e12-115">allow</span></span>|<span data-ttu-id="84e12-116">1</span><span class="sxs-lookup"><span data-stu-id="84e12-116">1</span></span>|<span data-ttu-id="84e12-117">允许设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="84e12-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="84e12-118">数据</span><span class="sxs-lookup"><span data-stu-id="84e12-118">block</span></span>|<span data-ttu-id="84e12-119">双面</span><span class="sxs-lookup"><span data-stu-id="84e12-119">2</span></span>|<span data-ttu-id="84e12-120">阻止设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="84e12-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="84e12-121">隔离</span><span class="sxs-lookup"><span data-stu-id="84e12-121">quarantine</span></span>|<span data-ttu-id="84e12-122">第三章</span><span class="sxs-lookup"><span data-stu-id="84e12-122">3</span></span>|<span data-ttu-id="84e12-123">隔离 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="84e12-123">Quarantine the device in Exchange.</span></span>|





