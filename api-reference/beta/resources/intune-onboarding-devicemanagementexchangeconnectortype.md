---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
author: tfitzmac
ms.openlocfilehash: 31459d4053e2ba1ef22a516995796baef2407dbf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301727"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="001ef-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="001ef-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="001ef-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="001ef-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="001ef-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="001ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="001ef-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="001ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="001ef-107">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="001ef-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="001ef-108">成员</span><span class="sxs-lookup"><span data-stu-id="001ef-108">Members</span></span>
|<span data-ttu-id="001ef-109">成员</span><span class="sxs-lookup"><span data-stu-id="001ef-109">Member</span></span>|<span data-ttu-id="001ef-110">值</span><span class="sxs-lookup"><span data-stu-id="001ef-110">Value</span></span>|<span data-ttu-id="001ef-111">说明</span><span class="sxs-lookup"><span data-stu-id="001ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="001ef-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="001ef-112">onPremises</span></span>|<span data-ttu-id="001ef-113">0</span><span class="sxs-lookup"><span data-stu-id="001ef-113">0</span></span>|<span data-ttu-id="001ef-114">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="001ef-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="001ef-115">承载</span><span class="sxs-lookup"><span data-stu-id="001ef-115">hosted</span></span>|<span data-ttu-id="001ef-116">1</span><span class="sxs-lookup"><span data-stu-id="001ef-116">1</span></span>|<span data-ttu-id="001ef-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="001ef-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="001ef-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="001ef-118">serviceToService</span></span>|<span data-ttu-id="001ef-119">2</span><span class="sxs-lookup"><span data-stu-id="001ef-119">2</span></span>|<span data-ttu-id="001ef-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="001ef-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="001ef-121">专用</span><span class="sxs-lookup"><span data-stu-id="001ef-121">dedicated</span></span>|<span data-ttu-id="001ef-122">3</span><span class="sxs-lookup"><span data-stu-id="001ef-122">3</span></span>|<span data-ttu-id="001ef-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="001ef-123">Connects to O365 Dedicated Exchange environment.</span></span>|





