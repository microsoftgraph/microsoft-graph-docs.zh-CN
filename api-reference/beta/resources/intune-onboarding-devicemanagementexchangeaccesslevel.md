---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ec6ddbf48d7e511a05140391937c4ce079a3bbdf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998154"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="06396-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="06396-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="06396-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="06396-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="06396-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06396-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06396-106">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="06396-106">Access Level in Exchange.</span></span>

## <a name="members"></a><span data-ttu-id="06396-107">成员</span><span class="sxs-lookup"><span data-stu-id="06396-107">Members</span></span>
|<span data-ttu-id="06396-108">成员</span><span class="sxs-lookup"><span data-stu-id="06396-108">Member</span></span>|<span data-ttu-id="06396-109">值</span><span class="sxs-lookup"><span data-stu-id="06396-109">Value</span></span>|<span data-ttu-id="06396-110">说明</span><span class="sxs-lookup"><span data-stu-id="06396-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06396-111">无</span><span class="sxs-lookup"><span data-stu-id="06396-111">none</span></span>|<span data-ttu-id="06396-112">0</span><span class="sxs-lookup"><span data-stu-id="06396-112">0</span></span>|<span data-ttu-id="06396-113">未在 Exchange 中配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="06396-113">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="06396-114">允许</span><span class="sxs-lookup"><span data-stu-id="06396-114">allow</span></span>|<span data-ttu-id="06396-115">1</span><span class="sxs-lookup"><span data-stu-id="06396-115">1</span></span>|<span data-ttu-id="06396-116">允许设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="06396-116">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="06396-117">数据</span><span class="sxs-lookup"><span data-stu-id="06396-117">block</span></span>|<span data-ttu-id="06396-118">双面</span><span class="sxs-lookup"><span data-stu-id="06396-118">2</span></span>|<span data-ttu-id="06396-119">阻止设备访问 Exchange。</span><span class="sxs-lookup"><span data-stu-id="06396-119">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="06396-120">隔离</span><span class="sxs-lookup"><span data-stu-id="06396-120">quarantine</span></span>|<span data-ttu-id="06396-121">第三章</span><span class="sxs-lookup"><span data-stu-id="06396-121">3</span></span>|<span data-ttu-id="06396-122">隔离 Exchange 中的设备。</span><span class="sxs-lookup"><span data-stu-id="06396-122">Quarantine the device in Exchange.</span></span>|





