---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange Connector 的当前状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 034a73cc8f75228977ea7387b2cea38672df1cb3
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029636"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="e9fb3-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e9fb3-103">deviceManagementExchangeConnectorStatus enum type</span></span>

<span data-ttu-id="e9fb3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e9fb3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e9fb3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e9fb3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e9fb3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9fb3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9fb3-107">Exchange Connector 的当前状态。</span><span class="sxs-lookup"><span data-stu-id="e9fb3-107">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="e9fb3-108">成员</span><span class="sxs-lookup"><span data-stu-id="e9fb3-108">Members</span></span>
|<span data-ttu-id="e9fb3-109">成员</span><span class="sxs-lookup"><span data-stu-id="e9fb3-109">Member</span></span>|<span data-ttu-id="e9fb3-110">值</span><span class="sxs-lookup"><span data-stu-id="e9fb3-110">Value</span></span>|<span data-ttu-id="e9fb3-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9fb3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9fb3-112">无</span><span class="sxs-lookup"><span data-stu-id="e9fb3-112">none</span></span>|<span data-ttu-id="e9fb3-113">0</span><span class="sxs-lookup"><span data-stu-id="e9fb3-113">0</span></span>|<span data-ttu-id="e9fb3-114">不存在任何连接器。</span><span class="sxs-lookup"><span data-stu-id="e9fb3-114">No Connector exists.</span></span>|
|<span data-ttu-id="e9fb3-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="e9fb3-115">connectionPending</span></span>|<span data-ttu-id="e9fb3-116">1 </span><span class="sxs-lookup"><span data-stu-id="e9fb3-116">1</span></span>|<span data-ttu-id="e9fb3-117">与 Exchange 环境的挂起连接。</span><span class="sxs-lookup"><span data-stu-id="e9fb3-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="e9fb3-118">连</span><span class="sxs-lookup"><span data-stu-id="e9fb3-118">connected</span></span>|<span data-ttu-id="e9fb3-119">2 </span><span class="sxs-lookup"><span data-stu-id="e9fb3-119">2</span></span>|<span data-ttu-id="e9fb3-120">已连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="e9fb3-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="e9fb3-121">被</span><span class="sxs-lookup"><span data-stu-id="e9fb3-121">disconnected</span></span>|<span data-ttu-id="e9fb3-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e9fb3-122">3</span></span>|<span data-ttu-id="e9fb3-123">断开与 Exchange 环境的连接</span><span class="sxs-lookup"><span data-stu-id="e9fb3-123">Disconnected from the Exchange Environment</span></span>|






