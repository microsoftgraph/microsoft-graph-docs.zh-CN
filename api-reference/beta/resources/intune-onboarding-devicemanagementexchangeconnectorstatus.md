---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange 连接器的当前状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 455d7ecbe2d22de7825faf36e743f830480a5737
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27928273"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="a3053-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a3053-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="a3053-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a3053-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a3053-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a3053-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a3053-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a3053-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3053-107">Exchange 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a3053-107">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="a3053-108">成员</span><span class="sxs-lookup"><span data-stu-id="a3053-108">Members</span></span>
|<span data-ttu-id="a3053-109">成员</span><span class="sxs-lookup"><span data-stu-id="a3053-109">Member</span></span>|<span data-ttu-id="a3053-110">值</span><span class="sxs-lookup"><span data-stu-id="a3053-110">Value</span></span>|<span data-ttu-id="a3053-111">Description</span><span class="sxs-lookup"><span data-stu-id="a3053-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3053-112">无</span><span class="sxs-lookup"><span data-stu-id="a3053-112">none</span></span>|<span data-ttu-id="a3053-113">0</span><span class="sxs-lookup"><span data-stu-id="a3053-113">0</span></span>|<span data-ttu-id="a3053-114">没有连接线存在。</span><span class="sxs-lookup"><span data-stu-id="a3053-114">No Connector exists.</span></span>|
|<span data-ttu-id="a3053-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="a3053-115">connectionPending</span></span>|<span data-ttu-id="a3053-116">1</span><span class="sxs-lookup"><span data-stu-id="a3053-116">1</span></span>|<span data-ttu-id="a3053-117">挂起的连接到 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="a3053-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="a3053-118">连接</span><span class="sxs-lookup"><span data-stu-id="a3053-118">connected</span></span>|<span data-ttu-id="a3053-119">2</span><span class="sxs-lookup"><span data-stu-id="a3053-119">2</span></span>|<span data-ttu-id="a3053-120">连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="a3053-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="a3053-121">断开连接</span><span class="sxs-lookup"><span data-stu-id="a3053-121">disconnected</span></span>|<span data-ttu-id="a3053-122">3</span><span class="sxs-lookup"><span data-stu-id="a3053-122">3</span></span>|<span data-ttu-id="a3053-123">从 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="a3053-123">Disconnected from the Exchange Environment</span></span>|





