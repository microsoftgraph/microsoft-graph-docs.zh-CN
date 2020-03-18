---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ba3550a494350a31a4b7dc3a2977c7b9660a51cd
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779063"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="3ac06-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3ac06-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="3ac06-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3ac06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3ac06-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3ac06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3ac06-106">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="3ac06-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="3ac06-107">成员</span><span class="sxs-lookup"><span data-stu-id="3ac06-107">Members</span></span>
|<span data-ttu-id="3ac06-108">成员</span><span class="sxs-lookup"><span data-stu-id="3ac06-108">Member</span></span>|<span data-ttu-id="3ac06-109">值</span><span class="sxs-lookup"><span data-stu-id="3ac06-109">Value</span></span>|<span data-ttu-id="3ac06-110">说明</span><span class="sxs-lookup"><span data-stu-id="3ac06-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3ac06-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="3ac06-111">onPremises</span></span>|<span data-ttu-id="3ac06-112">0</span><span class="sxs-lookup"><span data-stu-id="3ac06-112">0</span></span>|<span data-ttu-id="3ac06-113">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="3ac06-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="3ac06-114">otg</span><span class="sxs-lookup"><span data-stu-id="3ac06-114">hosted</span></span>|<span data-ttu-id="3ac06-115">1</span><span class="sxs-lookup"><span data-stu-id="3ac06-115">1</span></span>|<span data-ttu-id="3ac06-116">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="3ac06-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3ac06-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="3ac06-117">serviceToService</span></span>|<span data-ttu-id="3ac06-118">双面</span><span class="sxs-lookup"><span data-stu-id="3ac06-118">2</span></span>|<span data-ttu-id="3ac06-119">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="3ac06-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="3ac06-120">专用</span><span class="sxs-lookup"><span data-stu-id="3ac06-120">dedicated</span></span>|<span data-ttu-id="3ac06-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3ac06-121">3</span></span>|<span data-ttu-id="3ac06-122">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="3ac06-122">Connects to O365 Dedicated Exchange environment.</span></span>|



