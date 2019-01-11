---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 07449df53aa65036ae55e63c514c1687fbbab86a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888513"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="5b17d-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5b17d-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="5b17d-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5b17d-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b17d-105">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="5b17d-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="5b17d-106">成员</span><span class="sxs-lookup"><span data-stu-id="5b17d-106">Members</span></span>
|<span data-ttu-id="5b17d-107">成员</span><span class="sxs-lookup"><span data-stu-id="5b17d-107">Member</span></span>|<span data-ttu-id="5b17d-108">值</span><span class="sxs-lookup"><span data-stu-id="5b17d-108">Value</span></span>|<span data-ttu-id="5b17d-109">Description</span><span class="sxs-lookup"><span data-stu-id="5b17d-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b17d-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="5b17d-110">onPremises</span></span>|<span data-ttu-id="5b17d-111">0</span><span class="sxs-lookup"><span data-stu-id="5b17d-111">0</span></span>|<span data-ttu-id="5b17d-112">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="5b17d-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="5b17d-113">承载</span><span class="sxs-lookup"><span data-stu-id="5b17d-113">hosted</span></span>|<span data-ttu-id="5b17d-114">1</span><span class="sxs-lookup"><span data-stu-id="5b17d-114">1</span></span>|<span data-ttu-id="5b17d-115">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="5b17d-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="5b17d-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="5b17d-116">serviceToService</span></span>|<span data-ttu-id="5b17d-117">2</span><span class="sxs-lookup"><span data-stu-id="5b17d-117">2</span></span>|<span data-ttu-id="5b17d-118">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="5b17d-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="5b17d-119">专用</span><span class="sxs-lookup"><span data-stu-id="5b17d-119">dedicated</span></span>|<span data-ttu-id="5b17d-120">3</span><span class="sxs-lookup"><span data-stu-id="5b17d-120">3</span></span>|<span data-ttu-id="5b17d-121">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="5b17d-121">Connects to O365 Dedicated Exchange environment.</span></span>|



