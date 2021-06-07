---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: 连接器的当前Exchange状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 8a96613647b732ba233e5633ebd7f0f1440997e8
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751214"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="5dd01-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5dd01-103">deviceManagementExchangeConnectorStatus enum type</span></span>

<span data-ttu-id="5dd01-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5dd01-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5dd01-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5dd01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dd01-106">连接器的当前Exchange状态。</span><span class="sxs-lookup"><span data-stu-id="5dd01-106">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="5dd01-107">成员</span><span class="sxs-lookup"><span data-stu-id="5dd01-107">Members</span></span>
|<span data-ttu-id="5dd01-108">成员</span><span class="sxs-lookup"><span data-stu-id="5dd01-108">Member</span></span>|<span data-ttu-id="5dd01-109">值</span><span class="sxs-lookup"><span data-stu-id="5dd01-109">Value</span></span>|<span data-ttu-id="5dd01-110">Description</span><span class="sxs-lookup"><span data-stu-id="5dd01-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dd01-111">无</span><span class="sxs-lookup"><span data-stu-id="5dd01-111">none</span></span>|<span data-ttu-id="5dd01-112">0</span><span class="sxs-lookup"><span data-stu-id="5dd01-112">0</span></span>|<span data-ttu-id="5dd01-113">不存在连接器。</span><span class="sxs-lookup"><span data-stu-id="5dd01-113">No Connector exists.</span></span>|
|<span data-ttu-id="5dd01-114">connectionPending</span><span class="sxs-lookup"><span data-stu-id="5dd01-114">connectionPending</span></span>|<span data-ttu-id="5dd01-115">1</span><span class="sxs-lookup"><span data-stu-id="5dd01-115">1</span></span>|<span data-ttu-id="5dd01-116">挂起与 Exchange 的连接。</span><span class="sxs-lookup"><span data-stu-id="5dd01-116">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="5dd01-117">connected</span><span class="sxs-lookup"><span data-stu-id="5dd01-117">connected</span></span>|<span data-ttu-id="5dd01-118">2</span><span class="sxs-lookup"><span data-stu-id="5dd01-118">2</span></span>|<span data-ttu-id="5dd01-119">连接到Exchange环境</span><span class="sxs-lookup"><span data-stu-id="5dd01-119">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="5dd01-120">已断开连接</span><span class="sxs-lookup"><span data-stu-id="5dd01-120">disconnected</span></span>|<span data-ttu-id="5dd01-121">3</span><span class="sxs-lookup"><span data-stu-id="5dd01-121">3</span></span>|<span data-ttu-id="5dd01-122">与 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="5dd01-122">Disconnected from the Exchange Environment</span></span>|




