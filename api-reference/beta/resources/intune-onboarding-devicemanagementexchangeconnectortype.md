---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c05410c3b3b7c889840d0b47aca05f6457564eb4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934950"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="21ebe-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21ebe-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="21ebe-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="21ebe-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="21ebe-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="21ebe-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="21ebe-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="21ebe-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="21ebe-107">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="21ebe-107">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="21ebe-108">成员</span><span class="sxs-lookup"><span data-stu-id="21ebe-108">Members</span></span>
|<span data-ttu-id="21ebe-109">成员</span><span class="sxs-lookup"><span data-stu-id="21ebe-109">Member</span></span>|<span data-ttu-id="21ebe-110">值</span><span class="sxs-lookup"><span data-stu-id="21ebe-110">Value</span></span>|<span data-ttu-id="21ebe-111">说明</span><span class="sxs-lookup"><span data-stu-id="21ebe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21ebe-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="21ebe-112">onPremises</span></span>|<span data-ttu-id="21ebe-113">0</span><span class="sxs-lookup"><span data-stu-id="21ebe-113">0</span></span>|<span data-ttu-id="21ebe-114">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="21ebe-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="21ebe-115">承载</span><span class="sxs-lookup"><span data-stu-id="21ebe-115">hosted</span></span>|<span data-ttu-id="21ebe-116">1</span><span class="sxs-lookup"><span data-stu-id="21ebe-116">1</span></span>|<span data-ttu-id="21ebe-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="21ebe-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="21ebe-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="21ebe-118">serviceToService</span></span>|<span data-ttu-id="21ebe-119">2</span><span class="sxs-lookup"><span data-stu-id="21ebe-119">2</span></span>|<span data-ttu-id="21ebe-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="21ebe-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="21ebe-121">专用</span><span class="sxs-lookup"><span data-stu-id="21ebe-121">dedicated</span></span>|<span data-ttu-id="21ebe-122">3</span><span class="sxs-lookup"><span data-stu-id="21ebe-122">3</span></span>|<span data-ttu-id="21ebe-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="21ebe-123">Connects to O365 Dedicated Exchange environment.</span></span>|





