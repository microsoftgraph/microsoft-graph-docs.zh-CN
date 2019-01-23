---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 20eb1053d3dbf6cb657313f0c68f6c6c84804848
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398980"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="228ea-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="228ea-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="228ea-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="228ea-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="228ea-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="228ea-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="228ea-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="228ea-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="228ea-107">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="228ea-107">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="228ea-108">成员</span><span class="sxs-lookup"><span data-stu-id="228ea-108">Members</span></span>
|<span data-ttu-id="228ea-109">成员</span><span class="sxs-lookup"><span data-stu-id="228ea-109">Member</span></span>|<span data-ttu-id="228ea-110">值</span><span class="sxs-lookup"><span data-stu-id="228ea-110">Value</span></span>|<span data-ttu-id="228ea-111">说明</span><span class="sxs-lookup"><span data-stu-id="228ea-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="228ea-112">onPremises</span><span class="sxs-lookup"><span data-stu-id="228ea-112">onPremises</span></span>|<span data-ttu-id="228ea-113">0</span><span class="sxs-lookup"><span data-stu-id="228ea-113">0</span></span>|<span data-ttu-id="228ea-114">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="228ea-114">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="228ea-115">承载</span><span class="sxs-lookup"><span data-stu-id="228ea-115">hosted</span></span>|<span data-ttu-id="228ea-116">1</span><span class="sxs-lookup"><span data-stu-id="228ea-116">1</span></span>|<span data-ttu-id="228ea-117">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="228ea-117">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="228ea-118">serviceToService</span><span class="sxs-lookup"><span data-stu-id="228ea-118">serviceToService</span></span>|<span data-ttu-id="228ea-119">2</span><span class="sxs-lookup"><span data-stu-id="228ea-119">2</span></span>|<span data-ttu-id="228ea-120">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="228ea-120">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="228ea-121">专用</span><span class="sxs-lookup"><span data-stu-id="228ea-121">dedicated</span></span>|<span data-ttu-id="228ea-122">3</span><span class="sxs-lookup"><span data-stu-id="228ea-122">3</span></span>|<span data-ttu-id="228ea-123">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="228ea-123">Connects to O365 Dedicated Exchange environment.</span></span>|




