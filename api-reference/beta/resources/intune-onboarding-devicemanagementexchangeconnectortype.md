---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8ee6b98f668035f16f65ce366159d7d455ea6ae3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49288185"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="d5e2a-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d5e2a-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="d5e2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d5e2a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d5e2a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d5e2a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d5e2a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5e2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5e2a-107">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="d5e2a-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="d5e2a-108">成员</span><span class="sxs-lookup"><span data-stu-id="d5e2a-108">Members</span></span>
|<span data-ttu-id="d5e2a-109">成员</span><span class="sxs-lookup"><span data-stu-id="d5e2a-109">Member</span></span>|<span data-ttu-id="d5e2a-110">值</span><span class="sxs-lookup"><span data-stu-id="d5e2a-110">Value</span></span>|<span data-ttu-id="d5e2a-111">Description</span><span class="sxs-lookup"><span data-stu-id="d5e2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d5e2a-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="d5e2a-112">onPremises</span></span>|<span data-ttu-id="d5e2a-113">0</span><span class="sxs-lookup"><span data-stu-id="d5e2a-113">0</span></span>|<span data-ttu-id="d5e2a-114">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="d5e2a-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="d5e2a-115">otg</span><span class="sxs-lookup"><span data-stu-id="d5e2a-115">hosted</span></span>|<span data-ttu-id="d5e2a-116">1</span><span class="sxs-lookup"><span data-stu-id="d5e2a-116">1</span></span>|<span data-ttu-id="d5e2a-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="d5e2a-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="d5e2a-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="d5e2a-118">serviceToService</span></span>|<span data-ttu-id="d5e2a-119">双面</span><span class="sxs-lookup"><span data-stu-id="d5e2a-119">2</span></span>|<span data-ttu-id="d5e2a-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="d5e2a-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="d5e2a-121">专用</span><span class="sxs-lookup"><span data-stu-id="d5e2a-121">dedicated</span></span>|<span data-ttu-id="d5e2a-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d5e2a-122">3</span></span>|<span data-ttu-id="d5e2a-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="d5e2a-123">Connects to O365 Dedicated Exchange environment.</span></span>|




