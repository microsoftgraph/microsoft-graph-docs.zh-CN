---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 10fc00b5d3135535c557cd179d32029a6aef2f6b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48736105"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="ba990-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ba990-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="ba990-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ba990-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ba990-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ba990-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba990-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ba990-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba990-107">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="ba990-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="ba990-108">成员</span><span class="sxs-lookup"><span data-stu-id="ba990-108">Members</span></span>
|<span data-ttu-id="ba990-109">成员</span><span class="sxs-lookup"><span data-stu-id="ba990-109">Member</span></span>|<span data-ttu-id="ba990-110">值</span><span class="sxs-lookup"><span data-stu-id="ba990-110">Value</span></span>|<span data-ttu-id="ba990-111">说明</span><span class="sxs-lookup"><span data-stu-id="ba990-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba990-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="ba990-112">onPremises</span></span>|<span data-ttu-id="ba990-113">0</span><span class="sxs-lookup"><span data-stu-id="ba990-113">0</span></span>|<span data-ttu-id="ba990-114">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="ba990-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="ba990-115">otg</span><span class="sxs-lookup"><span data-stu-id="ba990-115">hosted</span></span>|<span data-ttu-id="ba990-116">1</span><span class="sxs-lookup"><span data-stu-id="ba990-116">1</span></span>|<span data-ttu-id="ba990-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="ba990-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ba990-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="ba990-118">serviceToService</span></span>|<span data-ttu-id="ba990-119">双面</span><span class="sxs-lookup"><span data-stu-id="ba990-119">2</span></span>|<span data-ttu-id="ba990-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="ba990-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="ba990-121">专用</span><span class="sxs-lookup"><span data-stu-id="ba990-121">dedicated</span></span>|<span data-ttu-id="ba990-122">第三章</span><span class="sxs-lookup"><span data-stu-id="ba990-122">3</span></span>|<span data-ttu-id="ba990-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="ba990-123">Connects to O365 Dedicated Exchange environment.</span></span>|





