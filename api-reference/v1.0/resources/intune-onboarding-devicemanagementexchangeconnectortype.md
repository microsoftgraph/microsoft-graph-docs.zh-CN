---
title: deviceManagementExchangeConnectorType 枚举类型
description: Exchange Connector 的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 9b34a3e51161ffd11321893f2f612385874188c3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48056518"
---
# <a name="devicemanagementexchangeconnectortype-enum-type"></a><span data-ttu-id="4b4f7-103">deviceManagementExchangeConnectorType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4b4f7-103">deviceManagementExchangeConnectorType enum type</span></span>

<span data-ttu-id="4b4f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4b4f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4b4f7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4b4f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4b4f7-106">Exchange Connector 的类型。</span><span class="sxs-lookup"><span data-stu-id="4b4f7-106">The type of Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="4b4f7-107">成员</span><span class="sxs-lookup"><span data-stu-id="4b4f7-107">Members</span></span>
|<span data-ttu-id="4b4f7-108">成员</span><span class="sxs-lookup"><span data-stu-id="4b4f7-108">Member</span></span>|<span data-ttu-id="4b4f7-109">值</span><span class="sxs-lookup"><span data-stu-id="4b4f7-109">Value</span></span>|<span data-ttu-id="4b4f7-110">说明</span><span class="sxs-lookup"><span data-stu-id="4b4f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b4f7-111">onPremises</span><span class="sxs-lookup"><span data-stu-id="4b4f7-111">onPremises</span></span>|<span data-ttu-id="4b4f7-112">0</span><span class="sxs-lookup"><span data-stu-id="4b4f7-112">0</span></span>|<span data-ttu-id="4b4f7-113">连接到本地 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="4b4f7-113">Connects to on-premises Exchange Environment.</span></span>|
|<span data-ttu-id="4b4f7-114">otg</span><span class="sxs-lookup"><span data-stu-id="4b4f7-114">hosted</span></span>|<span data-ttu-id="4b4f7-115">1 </span><span class="sxs-lookup"><span data-stu-id="4b4f7-115">1</span></span>|<span data-ttu-id="4b4f7-116">连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="4b4f7-116">Connects to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="4b4f7-117">serviceToService</span><span class="sxs-lookup"><span data-stu-id="4b4f7-117">serviceToService</span></span>|<span data-ttu-id="4b4f7-118">2 </span><span class="sxs-lookup"><span data-stu-id="4b4f7-118">2</span></span>|<span data-ttu-id="4b4f7-119">Intune 服务直接连接到 O365 多租户 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="4b4f7-119">Intune Service connects directly to O365 multi-tenant Exchange environment</span></span>|
|<span data-ttu-id="4b4f7-120">专用</span><span class="sxs-lookup"><span data-stu-id="4b4f7-120">dedicated</span></span>|<span data-ttu-id="4b4f7-121">第三章</span><span class="sxs-lookup"><span data-stu-id="4b4f7-121">3</span></span>|<span data-ttu-id="4b4f7-122">连接到 O365 专用 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="4b4f7-122">Connects to O365 Dedicated Exchange environment.</span></span>|









