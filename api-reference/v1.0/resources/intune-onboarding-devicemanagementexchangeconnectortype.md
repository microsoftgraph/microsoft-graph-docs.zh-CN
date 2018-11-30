---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
ms.openlocfilehash: 694b211afeaaaabb997f03dfc64618fc0301f0ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27010836"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="2413c-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2413c-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="2413c-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2413c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2413c-105">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="2413c-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="2413c-106">成员</span><span class="sxs-lookup"><span data-stu-id="2413c-106">Members</span></span>
|<span data-ttu-id="2413c-107">成员</span><span class="sxs-lookup"><span data-stu-id="2413c-107">Member</span></span>|<span data-ttu-id="2413c-108">值</span><span class="sxs-lookup"><span data-stu-id="2413c-108">Value</span></span>|<span data-ttu-id="2413c-109">说明</span><span class="sxs-lookup"><span data-stu-id="2413c-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2413c-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="2413c-110">onPremises</span></span>|<span data-ttu-id="2413c-111">0</span><span class="sxs-lookup"><span data-stu-id="2413c-111">0</span></span>|<span data-ttu-id="2413c-112">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="2413c-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="2413c-113">承载</span><span class="sxs-lookup"><span data-stu-id="2413c-113">hosted</span></span>|<span data-ttu-id="2413c-114">1</span><span class="sxs-lookup"><span data-stu-id="2413c-114">1</span></span>|<span data-ttu-id="2413c-115">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="2413c-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="2413c-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="2413c-116">serviceToService</span></span>|<span data-ttu-id="2413c-117">2</span><span class="sxs-lookup"><span data-stu-id="2413c-117">2</span></span>|<span data-ttu-id="2413c-118">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="2413c-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="2413c-119">专用</span><span class="sxs-lookup"><span data-stu-id="2413c-119">dedicated</span></span>|<span data-ttu-id="2413c-120">3</span><span class="sxs-lookup"><span data-stu-id="2413c-120">3</span></span>|<span data-ttu-id="2413c-121">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="2413c-121">Connects to O365 Dedicated Exchange environment.</span></span>|



