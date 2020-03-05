---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 848e7aba02627042603e4240694fc7f267ef903e
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448100"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="d3243-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d3243-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="d3243-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d3243-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d3243-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3243-106">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="d3243-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="d3243-107">成员</span><span class="sxs-lookup"><span data-stu-id="d3243-107">Members</span></span>
|<span data-ttu-id="d3243-108">成员</span><span class="sxs-lookup"><span data-stu-id="d3243-108">Member</span></span>|<span data-ttu-id="d3243-109">值</span><span class="sxs-lookup"><span data-stu-id="d3243-109">Value</span></span>|<span data-ttu-id="d3243-110">说明</span><span class="sxs-lookup"><span data-stu-id="d3243-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3243-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="d3243-111">onPremises</span></span>|<span data-ttu-id="d3243-112">0</span><span class="sxs-lookup"><span data-stu-id="d3243-112">0</span></span>|<span data-ttu-id="d3243-113">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="d3243-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="d3243-114">otg</span><span class="sxs-lookup"><span data-stu-id="d3243-114">hosted</span></span>|<span data-ttu-id="d3243-115">1 </span><span class="sxs-lookup"><span data-stu-id="d3243-115">1</span></span>|<span data-ttu-id="d3243-116">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="d3243-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="d3243-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="d3243-117">serviceToService</span></span>|<span data-ttu-id="d3243-118">2 </span><span class="sxs-lookup"><span data-stu-id="d3243-118">2</span></span>|<span data-ttu-id="d3243-119">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="d3243-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="d3243-120">专用</span><span class="sxs-lookup"><span data-stu-id="d3243-120">dedicated</span></span>|<span data-ttu-id="d3243-121">3 </span><span class="sxs-lookup"><span data-stu-id="d3243-121">3</span></span>|<span data-ttu-id="d3243-122">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="d3243-122">Connects to O365 Dedicated Exchange environment.</span></span>|




