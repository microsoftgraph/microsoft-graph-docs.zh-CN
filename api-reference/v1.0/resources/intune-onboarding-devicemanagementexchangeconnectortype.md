---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
author: tfitzmac
ms.openlocfilehash: 333a5a7c6f73fead263edbdf3edafeefc3514ed1
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27306732"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="0b464-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0b464-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="0b464-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0b464-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0b464-105">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="0b464-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="0b464-106">成员</span><span class="sxs-lookup"><span data-stu-id="0b464-106">Members</span></span>
|<span data-ttu-id="0b464-107">成员</span><span class="sxs-lookup"><span data-stu-id="0b464-107">Member</span></span>|<span data-ttu-id="0b464-108">值</span><span class="sxs-lookup"><span data-stu-id="0b464-108">Value</span></span>|<span data-ttu-id="0b464-109">说明</span><span class="sxs-lookup"><span data-stu-id="0b464-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b464-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="0b464-110">onPremises</span></span>|<span data-ttu-id="0b464-111">0</span><span class="sxs-lookup"><span data-stu-id="0b464-111">0</span></span>|<span data-ttu-id="0b464-112">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="0b464-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="0b464-113">承载</span><span class="sxs-lookup"><span data-stu-id="0b464-113">hosted</span></span>|<span data-ttu-id="0b464-114">1</span><span class="sxs-lookup"><span data-stu-id="0b464-114">1</span></span>|<span data-ttu-id="0b464-115">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="0b464-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="0b464-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="0b464-116">serviceToService</span></span>|<span data-ttu-id="0b464-117">2</span><span class="sxs-lookup"><span data-stu-id="0b464-117">2</span></span>|<span data-ttu-id="0b464-118">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="0b464-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="0b464-119">专用</span><span class="sxs-lookup"><span data-stu-id="0b464-119">dedicated</span></span>|<span data-ttu-id="0b464-120">3</span><span class="sxs-lookup"><span data-stu-id="0b464-120">3</span></span>|<span data-ttu-id="0b464-121">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="0b464-121">Connects to O365 Dedicated Exchange environment.</span></span>|



