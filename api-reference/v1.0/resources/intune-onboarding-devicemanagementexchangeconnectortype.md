---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c358832db83e5f5b3e1fb0f5457f480d21ded996
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30263558"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="8a7bd-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8a7bd-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="8a7bd-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8a7bd-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8a7bd-105">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="8a7bd-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="8a7bd-106">成员</span><span class="sxs-lookup"><span data-stu-id="8a7bd-106">Members</span></span>
|<span data-ttu-id="8a7bd-107">成员</span><span class="sxs-lookup"><span data-stu-id="8a7bd-107">Member</span></span>|<span data-ttu-id="8a7bd-108">值</span><span class="sxs-lookup"><span data-stu-id="8a7bd-108">Value</span></span>|<span data-ttu-id="8a7bd-109">说明</span><span class="sxs-lookup"><span data-stu-id="8a7bd-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a7bd-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="8a7bd-110">onPremises</span></span>|<span data-ttu-id="8a7bd-111">0</span><span class="sxs-lookup"><span data-stu-id="8a7bd-111">0</span></span>|<span data-ttu-id="8a7bd-112">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="8a7bd-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="8a7bd-113">otg</span><span class="sxs-lookup"><span data-stu-id="8a7bd-113">hosted</span></span>|<span data-ttu-id="8a7bd-114">1</span><span class="sxs-lookup"><span data-stu-id="8a7bd-114">1</span></span>|<span data-ttu-id="8a7bd-115">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="8a7bd-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="8a7bd-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="8a7bd-116">serviceToService</span></span>|<span data-ttu-id="8a7bd-117">双面</span><span class="sxs-lookup"><span data-stu-id="8a7bd-117">2</span></span>|<span data-ttu-id="8a7bd-118">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="8a7bd-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="8a7bd-119">专用</span><span class="sxs-lookup"><span data-stu-id="8a7bd-119">dedicated</span></span>|<span data-ttu-id="8a7bd-120">第三章</span><span class="sxs-lookup"><span data-stu-id="8a7bd-120">3</span></span>|<span data-ttu-id="8a7bd-121">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="8a7bd-121">Connects to O365 Dedicated Exchange environment.</span></span>|



