---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: af90d5f3fd461fbc7888cabec66959f385a4dc3e
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029622"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="3e43e-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3e43e-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="3e43e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3e43e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3e43e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3e43e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3e43e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3e43e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3e43e-107">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="3e43e-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="3e43e-108">成员</span><span class="sxs-lookup"><span data-stu-id="3e43e-108">Members</span></span>
|<span data-ttu-id="3e43e-109">成员</span><span class="sxs-lookup"><span data-stu-id="3e43e-109">Member</span></span>|<span data-ttu-id="3e43e-110">值</span><span class="sxs-lookup"><span data-stu-id="3e43e-110">Value</span></span>|<span data-ttu-id="3e43e-111">说明</span><span class="sxs-lookup"><span data-stu-id="3e43e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3e43e-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="3e43e-112">onPremises</span></span>|<span data-ttu-id="3e43e-113">0</span><span class="sxs-lookup"><span data-stu-id="3e43e-113">0</span></span>|<span data-ttu-id="3e43e-114">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="3e43e-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="3e43e-115">otg</span><span class="sxs-lookup"><span data-stu-id="3e43e-115">hosted</span></span>|<span data-ttu-id="3e43e-116">1 </span><span class="sxs-lookup"><span data-stu-id="3e43e-116">1</span></span>|<span data-ttu-id="3e43e-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="3e43e-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3e43e-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="3e43e-118">serviceToService</span></span>|<span data-ttu-id="3e43e-119">2 </span><span class="sxs-lookup"><span data-stu-id="3e43e-119">2</span></span>|<span data-ttu-id="3e43e-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="3e43e-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3e43e-121">专用</span><span class="sxs-lookup"><span data-stu-id="3e43e-121">dedicated</span></span>|<span data-ttu-id="3e43e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="3e43e-122">3</span></span>|<span data-ttu-id="3e43e-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="3e43e-123">Connects to O365 Dedicated Exchange environment.</span></span>|






