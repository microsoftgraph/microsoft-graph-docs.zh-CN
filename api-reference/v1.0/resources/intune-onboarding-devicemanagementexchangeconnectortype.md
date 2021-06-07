---
title: deviceManagementExchangeConnectorType 枚举类型
description: 连接器Exchange类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 1f13c17971821cceae2d70b14a328367d918db76
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751578"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="58b72-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="58b72-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="58b72-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58b72-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58b72-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58b72-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58b72-106">连接器Exchange类型。</span><span class="sxs-lookup"><span data-stu-id="58b72-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="58b72-107">成员</span><span class="sxs-lookup"><span data-stu-id="58b72-107">Members</span></span>
|<span data-ttu-id="58b72-108">成员</span><span class="sxs-lookup"><span data-stu-id="58b72-108">Member</span></span>|<span data-ttu-id="58b72-109">值</span><span class="sxs-lookup"><span data-stu-id="58b72-109">Value</span></span>|<span data-ttu-id="58b72-110">Description</span><span class="sxs-lookup"><span data-stu-id="58b72-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58b72-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="58b72-111">onPremises</span></span>|<span data-ttu-id="58b72-112">0</span><span class="sxs-lookup"><span data-stu-id="58b72-112">0</span></span>|<span data-ttu-id="58b72-113">连接到本地部署Exchange环境。</span><span class="sxs-lookup"><span data-stu-id="58b72-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="58b72-114">托管</span><span class="sxs-lookup"><span data-stu-id="58b72-114">hosted</span></span>|<span data-ttu-id="58b72-115">1</span><span class="sxs-lookup"><span data-stu-id="58b72-115">1</span></span>|<span data-ttu-id="58b72-116">连接到 O365 多租户Exchange环境</span><span class="sxs-lookup"><span data-stu-id="58b72-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="58b72-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="58b72-117">serviceToService</span></span>|<span data-ttu-id="58b72-118">2</span><span class="sxs-lookup"><span data-stu-id="58b72-118">2</span></span>|<span data-ttu-id="58b72-119">Intune 服务直接连接到 O365 多租户Exchange环境</span><span class="sxs-lookup"><span data-stu-id="58b72-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="58b72-120">dedicated</span><span class="sxs-lookup"><span data-stu-id="58b72-120">dedicated</span></span>|<span data-ttu-id="58b72-121">3</span><span class="sxs-lookup"><span data-stu-id="58b72-121">3</span></span>|<span data-ttu-id="58b72-122">连接到 O365 专用Exchange环境。</span><span class="sxs-lookup"><span data-stu-id="58b72-122">Connects to O365 Dedicated Exchange environment.</span></span>|




