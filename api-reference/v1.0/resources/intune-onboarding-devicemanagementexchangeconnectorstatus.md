---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange 连接器的当前状态。
author: tfitzmac
ms.openlocfilehash: 6655e4c659141558d0c1e873f0e17ee3439ea95b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330665"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="e0eae-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e0eae-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="e0eae-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e0eae-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e0eae-105">Exchange 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="e0eae-105">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="e0eae-106">成员</span><span class="sxs-lookup"><span data-stu-id="e0eae-106">Members</span></span>
|<span data-ttu-id="e0eae-107">成员</span><span class="sxs-lookup"><span data-stu-id="e0eae-107">Member</span></span>|<span data-ttu-id="e0eae-108">值</span><span class="sxs-lookup"><span data-stu-id="e0eae-108">Value</span></span>|<span data-ttu-id="e0eae-109">说明</span><span class="sxs-lookup"><span data-stu-id="e0eae-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e0eae-110">无</span><span class="sxs-lookup"><span data-stu-id="e0eae-110">none</span></span>|<span data-ttu-id="e0eae-111">0</span><span class="sxs-lookup"><span data-stu-id="e0eae-111">0</span></span>|<span data-ttu-id="e0eae-112">没有连接线存在。</span><span class="sxs-lookup"><span data-stu-id="e0eae-112">No Connector exists.</span></span>|
|<span data-ttu-id="e0eae-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="e0eae-113">connectionPending</span></span>|<span data-ttu-id="e0eae-114">1</span><span class="sxs-lookup"><span data-stu-id="e0eae-114">1</span></span>|<span data-ttu-id="e0eae-115">挂起的连接到 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="e0eae-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="e0eae-116">连接</span><span class="sxs-lookup"><span data-stu-id="e0eae-116">connected</span></span>|<span data-ttu-id="e0eae-117">2</span><span class="sxs-lookup"><span data-stu-id="e0eae-117">2</span></span>|<span data-ttu-id="e0eae-118">连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="e0eae-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="e0eae-119">断开连接</span><span class="sxs-lookup"><span data-stu-id="e0eae-119">disconnected</span></span>|<span data-ttu-id="e0eae-120">3</span><span class="sxs-lookup"><span data-stu-id="e0eae-120">3</span></span>|<span data-ttu-id="e0eae-121">从 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="e0eae-121">Disconnected from the Exchange Environment</span></span>|



