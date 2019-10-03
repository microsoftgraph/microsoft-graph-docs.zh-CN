---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: fdb99f770e719d05ef097820ff5fff56b7f0a74d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37367964"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="9c811-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9c811-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="9c811-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9c811-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c811-105">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="9c811-105">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="9c811-106">成员</span><span class="sxs-lookup"><span data-stu-id="9c811-106">Members</span></span>
|<span data-ttu-id="9c811-107">成员</span><span class="sxs-lookup"><span data-stu-id="9c811-107">Member</span></span>|<span data-ttu-id="9c811-108">值</span><span class="sxs-lookup"><span data-stu-id="9c811-108">Value</span></span>|<span data-ttu-id="9c811-109">说明</span><span class="sxs-lookup"><span data-stu-id="9c811-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9c811-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="9c811-110">onPremises</span></span>|<span data-ttu-id="9c811-111">0</span><span class="sxs-lookup"><span data-stu-id="9c811-111">0</span></span>|<span data-ttu-id="9c811-112">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="9c811-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="9c811-113">otg</span><span class="sxs-lookup"><span data-stu-id="9c811-113">hosted</span></span>|<span data-ttu-id="9c811-114">1</span><span class="sxs-lookup"><span data-stu-id="9c811-114">1</span></span>|<span data-ttu-id="9c811-115">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="9c811-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="9c811-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="9c811-116">serviceToService</span></span>|<span data-ttu-id="9c811-117">双面</span><span class="sxs-lookup"><span data-stu-id="9c811-117">2</span></span>|<span data-ttu-id="9c811-118">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="9c811-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="9c811-119">专用</span><span class="sxs-lookup"><span data-stu-id="9c811-119">dedicated</span></span>|<span data-ttu-id="9c811-120">第三章</span><span class="sxs-lookup"><span data-stu-id="9c811-120">3</span></span>|<span data-ttu-id="9c811-121">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="9c811-121">Connects to O365 Dedicated Exchange environment.</span></span>|




