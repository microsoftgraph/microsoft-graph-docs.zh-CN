---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: aec7d3ee34f4d9cdd9a31a93db8934673bbafa7d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459474"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="ed11c-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ed11c-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="ed11c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed11c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ed11c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ed11c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ed11c-106">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="ed11c-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="ed11c-107">成员</span><span class="sxs-lookup"><span data-stu-id="ed11c-107">Members</span></span>
|<span data-ttu-id="ed11c-108">成员</span><span class="sxs-lookup"><span data-stu-id="ed11c-108">Member</span></span>|<span data-ttu-id="ed11c-109">值</span><span class="sxs-lookup"><span data-stu-id="ed11c-109">Value</span></span>|<span data-ttu-id="ed11c-110">说明</span><span class="sxs-lookup"><span data-stu-id="ed11c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ed11c-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="ed11c-111">onPremises</span></span>|<span data-ttu-id="ed11c-112">0</span><span class="sxs-lookup"><span data-stu-id="ed11c-112">0</span></span>|<span data-ttu-id="ed11c-113">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="ed11c-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="ed11c-114">otg</span><span class="sxs-lookup"><span data-stu-id="ed11c-114">hosted</span></span>|<span data-ttu-id="ed11c-115">1</span><span class="sxs-lookup"><span data-stu-id="ed11c-115">1</span></span>|<span data-ttu-id="ed11c-116">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="ed11c-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ed11c-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="ed11c-117">serviceToService</span></span>|<span data-ttu-id="ed11c-118">双面</span><span class="sxs-lookup"><span data-stu-id="ed11c-118">2</span></span>|<span data-ttu-id="ed11c-119">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="ed11c-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ed11c-120">专用</span><span class="sxs-lookup"><span data-stu-id="ed11c-120">dedicated</span></span>|<span data-ttu-id="ed11c-121">第三章</span><span class="sxs-lookup"><span data-stu-id="ed11c-121">3</span></span>|<span data-ttu-id="ed11c-122">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="ed11c-122">Connects to O365 Dedicated Exchange environment.</span></span>|







