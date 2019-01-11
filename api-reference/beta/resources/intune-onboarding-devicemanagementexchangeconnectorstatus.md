---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange 连接器的当前状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d2d1bc97795a664515eb4ea6f620c41a64394be0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27816056"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="45b02-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="45b02-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="45b02-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="45b02-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45b02-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45b02-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45b02-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45b02-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45b02-107">Exchange 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="45b02-107">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="45b02-108">成员</span><span class="sxs-lookup"><span data-stu-id="45b02-108">Members</span></span>
|<span data-ttu-id="45b02-109">成员</span><span class="sxs-lookup"><span data-stu-id="45b02-109">Member</span></span>|<span data-ttu-id="45b02-110">值</span><span class="sxs-lookup"><span data-stu-id="45b02-110">Value</span></span>|<span data-ttu-id="45b02-111">Description</span><span class="sxs-lookup"><span data-stu-id="45b02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45b02-112">无</span><span class="sxs-lookup"><span data-stu-id="45b02-112">none</span></span>|<span data-ttu-id="45b02-113">0</span><span class="sxs-lookup"><span data-stu-id="45b02-113">0</span></span>|<span data-ttu-id="45b02-114">没有连接线存在。</span><span class="sxs-lookup"><span data-stu-id="45b02-114">No Connector exists.</span></span>|
|<span data-ttu-id="45b02-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="45b02-115">connectionPending</span></span>|<span data-ttu-id="45b02-116">1</span><span class="sxs-lookup"><span data-stu-id="45b02-116">1</span></span>|<span data-ttu-id="45b02-117">挂起的连接到 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="45b02-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="45b02-118">连接</span><span class="sxs-lookup"><span data-stu-id="45b02-118">connected</span></span>|<span data-ttu-id="45b02-119">2</span><span class="sxs-lookup"><span data-stu-id="45b02-119">2</span></span>|<span data-ttu-id="45b02-120">连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="45b02-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="45b02-121">断开连接</span><span class="sxs-lookup"><span data-stu-id="45b02-121">disconnected</span></span>|<span data-ttu-id="45b02-122">3</span><span class="sxs-lookup"><span data-stu-id="45b02-122">3</span></span>|<span data-ttu-id="45b02-123">从 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="45b02-123">Disconnected from the Exchange Environment</span></span>|





