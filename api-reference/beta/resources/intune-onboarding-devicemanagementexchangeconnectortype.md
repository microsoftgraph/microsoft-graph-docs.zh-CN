---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
ms.openlocfilehash: 59bc1aa080f84fdd25a2da26ec9e7ff9aba20641
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043122"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="97f16-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="97f16-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="97f16-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="97f16-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97f16-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="97f16-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="97f16-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="97f16-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97f16-107">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="97f16-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="97f16-108">成员</span><span class="sxs-lookup"><span data-stu-id="97f16-108">Members</span></span>
|<span data-ttu-id="97f16-109">成员</span><span class="sxs-lookup"><span data-stu-id="97f16-109">Member</span></span>|<span data-ttu-id="97f16-110">值</span><span class="sxs-lookup"><span data-stu-id="97f16-110">Value</span></span>|<span data-ttu-id="97f16-111">说明</span><span class="sxs-lookup"><span data-stu-id="97f16-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97f16-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="97f16-112">onPremises</span></span>|<span data-ttu-id="97f16-113">0</span><span class="sxs-lookup"><span data-stu-id="97f16-113">0</span></span>|<span data-ttu-id="97f16-114">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="97f16-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="97f16-115">承载</span><span class="sxs-lookup"><span data-stu-id="97f16-115">hosted</span></span>|<span data-ttu-id="97f16-116">1</span><span class="sxs-lookup"><span data-stu-id="97f16-116">1</span></span>|<span data-ttu-id="97f16-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="97f16-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="97f16-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="97f16-118">serviceToService</span></span>|<span data-ttu-id="97f16-119">2</span><span class="sxs-lookup"><span data-stu-id="97f16-119">2</span></span>|<span data-ttu-id="97f16-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="97f16-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="97f16-121">专用</span><span class="sxs-lookup"><span data-stu-id="97f16-121">dedicated</span></span>|<span data-ttu-id="97f16-122">3</span><span class="sxs-lookup"><span data-stu-id="97f16-122">3</span></span>|<span data-ttu-id="97f16-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="97f16-123">Connects to O365 Dedicated Exchange environment.</span></span>|





