---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 36cdb3ff0490ea1b2d446beb587ef3a828e638ed
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34993051"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="01538-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="01538-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="01538-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="01538-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01538-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="01538-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01538-106">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="01538-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="01538-107">成员</span><span class="sxs-lookup"><span data-stu-id="01538-107">Members</span></span>
|<span data-ttu-id="01538-108">成员</span><span class="sxs-lookup"><span data-stu-id="01538-108">Member</span></span>|<span data-ttu-id="01538-109">值</span><span class="sxs-lookup"><span data-stu-id="01538-109">Value</span></span>|<span data-ttu-id="01538-110">说明</span><span class="sxs-lookup"><span data-stu-id="01538-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01538-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="01538-111">onPremises</span></span>|<span data-ttu-id="01538-112">0</span><span class="sxs-lookup"><span data-stu-id="01538-112">0</span></span>|<span data-ttu-id="01538-113">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="01538-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="01538-114">otg</span><span class="sxs-lookup"><span data-stu-id="01538-114">hosted</span></span>|<span data-ttu-id="01538-115">1</span><span class="sxs-lookup"><span data-stu-id="01538-115">1</span></span>|<span data-ttu-id="01538-116">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="01538-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="01538-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="01538-117">serviceToService</span></span>|<span data-ttu-id="01538-118">双面</span><span class="sxs-lookup"><span data-stu-id="01538-118">2</span></span>|<span data-ttu-id="01538-119">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="01538-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="01538-120">专用</span><span class="sxs-lookup"><span data-stu-id="01538-120">dedicated</span></span>|<span data-ttu-id="01538-121">第三章</span><span class="sxs-lookup"><span data-stu-id="01538-121">3</span></span>|<span data-ttu-id="01538-122">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="01538-122">Connects to O365 Dedicated Exchange environment.</span></span>|





