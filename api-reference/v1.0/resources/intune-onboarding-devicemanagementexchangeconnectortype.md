---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange 连接器的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8e9e50a4475ca2d57b3f38567703046588d4fb3c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27986430"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="dedfb-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="dedfb-103">deviceManagementExchangeConnectorType enum type</span></span>

> <span data-ttu-id="dedfb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="dedfb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dedfb-105">Exchange 连接器的类型。</span><span class="sxs-lookup"><span data-stu-id="dedfb-105">The type of Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="dedfb-106">成员</span><span class="sxs-lookup"><span data-stu-id="dedfb-106">Members</span></span>
|<span data-ttu-id="dedfb-107">成员</span><span class="sxs-lookup"><span data-stu-id="dedfb-107">Member</span></span>|<span data-ttu-id="dedfb-108">值</span><span class="sxs-lookup"><span data-stu-id="dedfb-108">Value</span></span>|<span data-ttu-id="dedfb-109">说明</span><span class="sxs-lookup"><span data-stu-id="dedfb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dedfb-110">onPremises</span><span class="sxs-lookup"><span data-stu-id="dedfb-110">onPremises</span></span>|<span data-ttu-id="dedfb-111">0</span><span class="sxs-lookup"><span data-stu-id="dedfb-111">0</span></span>|<span data-ttu-id="dedfb-112">连接到内部部署 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="dedfb-112">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="dedfb-113">承载</span><span class="sxs-lookup"><span data-stu-id="dedfb-113">hosted</span></span>|<span data-ttu-id="dedfb-114">1</span><span class="sxs-lookup"><span data-stu-id="dedfb-114">1</span></span>|<span data-ttu-id="dedfb-115">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="dedfb-115">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="dedfb-116">serviceToService</span><span class="sxs-lookup"><span data-stu-id="dedfb-116">serviceToService</span></span>|<span data-ttu-id="dedfb-117">2</span><span class="sxs-lookup"><span data-stu-id="dedfb-117">2</span></span>|<span data-ttu-id="dedfb-118">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="dedfb-118">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="dedfb-119">专用</span><span class="sxs-lookup"><span data-stu-id="dedfb-119">dedicated</span></span>|<span data-ttu-id="dedfb-120">3</span><span class="sxs-lookup"><span data-stu-id="dedfb-120">3</span></span>|<span data-ttu-id="dedfb-121">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="dedfb-121">Connects to O365 Dedicated Exchange environment.</span></span>|



