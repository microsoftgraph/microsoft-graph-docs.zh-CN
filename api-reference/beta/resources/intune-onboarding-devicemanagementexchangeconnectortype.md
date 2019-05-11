---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 31be5ad593b11a6344a98404b007109aa6409075
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33940370"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="22ceb-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="22ceb-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="22ceb-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22ceb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22ceb-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22ceb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22ceb-106">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="22ceb-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="22ceb-107">成员</span><span class="sxs-lookup"><span data-stu-id="22ceb-107">Members</span></span>
|<span data-ttu-id="22ceb-108">成员</span><span class="sxs-lookup"><span data-stu-id="22ceb-108">Member</span></span>|<span data-ttu-id="22ceb-109">值</span><span class="sxs-lookup"><span data-stu-id="22ceb-109">Value</span></span>|<span data-ttu-id="22ceb-110">说明</span><span class="sxs-lookup"><span data-stu-id="22ceb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22ceb-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="22ceb-111">onPremises</span></span>|<span data-ttu-id="22ceb-112">0</span><span class="sxs-lookup"><span data-stu-id="22ceb-112">0</span></span>|<span data-ttu-id="22ceb-113">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="22ceb-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="22ceb-114">otg</span><span class="sxs-lookup"><span data-stu-id="22ceb-114">hosted</span></span>|<span data-ttu-id="22ceb-115">1</span><span class="sxs-lookup"><span data-stu-id="22ceb-115">1</span></span>|<span data-ttu-id="22ceb-116">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="22ceb-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="22ceb-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="22ceb-117">serviceToService</span></span>|<span data-ttu-id="22ceb-118">双面</span><span class="sxs-lookup"><span data-stu-id="22ceb-118">2</span></span>|<span data-ttu-id="22ceb-119">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="22ceb-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="22ceb-120">专用</span><span class="sxs-lookup"><span data-stu-id="22ceb-120">dedicated</span></span>|<span data-ttu-id="22ceb-121">第三章</span><span class="sxs-lookup"><span data-stu-id="22ceb-121">3</span></span>|<span data-ttu-id="22ceb-122">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="22ceb-122">Connects to O365 Dedicated Exchange environment.</span></span>|




