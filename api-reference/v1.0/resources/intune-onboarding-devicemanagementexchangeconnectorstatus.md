---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange Connector 的当前状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ecc11286ff4935ee496de72acaceb01e7b272214
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42448114"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="0144e-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0144e-103">deviceManagementExchangeConnectorStatus enum type</span></span>

<span data-ttu-id="0144e-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0144e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0144e-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0144e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0144e-106">Exchange Connector 的当前状态。</span><span class="sxs-lookup"><span data-stu-id="0144e-106">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="0144e-107">成员</span><span class="sxs-lookup"><span data-stu-id="0144e-107">Members</span></span>
|<span data-ttu-id="0144e-108">成员</span><span class="sxs-lookup"><span data-stu-id="0144e-108">Member</span></span>|<span data-ttu-id="0144e-109">值</span><span class="sxs-lookup"><span data-stu-id="0144e-109">Value</span></span>|<span data-ttu-id="0144e-110">说明</span><span class="sxs-lookup"><span data-stu-id="0144e-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0144e-111">无</span><span class="sxs-lookup"><span data-stu-id="0144e-111">none</span></span>|<span data-ttu-id="0144e-112">0</span><span class="sxs-lookup"><span data-stu-id="0144e-112">0</span></span>|<span data-ttu-id="0144e-113">不存在任何连接器。</span><span class="sxs-lookup"><span data-stu-id="0144e-113">No Connector exists.</span></span>|
|<span data-ttu-id="0144e-114">connectionPending</span><span class="sxs-lookup"><span data-stu-id="0144e-114">connectionPending</span></span>|<span data-ttu-id="0144e-115">1 </span><span class="sxs-lookup"><span data-stu-id="0144e-115">1</span></span>|<span data-ttu-id="0144e-116">与 Exchange 环境的挂起连接。</span><span class="sxs-lookup"><span data-stu-id="0144e-116">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="0144e-117">连</span><span class="sxs-lookup"><span data-stu-id="0144e-117">connected</span></span>|<span data-ttu-id="0144e-118">2 </span><span class="sxs-lookup"><span data-stu-id="0144e-118">2</span></span>|<span data-ttu-id="0144e-119">已连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="0144e-119">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="0144e-120">被</span><span class="sxs-lookup"><span data-stu-id="0144e-120">disconnected</span></span>|<span data-ttu-id="0144e-121">3 </span><span class="sxs-lookup"><span data-stu-id="0144e-121">3</span></span>|<span data-ttu-id="0144e-122">断开与 Exchange 环境的连接</span><span class="sxs-lookup"><span data-stu-id="0144e-122">Disconnected from the Exchange Environment</span></span>|




