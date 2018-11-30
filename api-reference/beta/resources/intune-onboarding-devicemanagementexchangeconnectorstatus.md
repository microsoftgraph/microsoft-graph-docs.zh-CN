---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange 连接器的当前状态。
ms.openlocfilehash: cd8b845f4902788029be8661b47161997203fc73
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043772"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="7fa6d-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7fa6d-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="7fa6d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7fa6d-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7fa6d-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7fa6d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7fa6d-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7fa6d-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7fa6d-107">Exchange 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="7fa6d-107">The current status of the Exchange Connector.</span></span>
## <a name="members"></a><span data-ttu-id="7fa6d-108">成员</span><span class="sxs-lookup"><span data-stu-id="7fa6d-108">Members</span></span>
|<span data-ttu-id="7fa6d-109">成员</span><span class="sxs-lookup"><span data-stu-id="7fa6d-109">Member</span></span>|<span data-ttu-id="7fa6d-110">值</span><span class="sxs-lookup"><span data-stu-id="7fa6d-110">Value</span></span>|<span data-ttu-id="7fa6d-111">说明</span><span class="sxs-lookup"><span data-stu-id="7fa6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7fa6d-112">无</span><span class="sxs-lookup"><span data-stu-id="7fa6d-112">none</span></span>|<span data-ttu-id="7fa6d-113">0</span><span class="sxs-lookup"><span data-stu-id="7fa6d-113">0</span></span>|<span data-ttu-id="7fa6d-114">没有连接线存在。</span><span class="sxs-lookup"><span data-stu-id="7fa6d-114">No Connector exists.</span></span>|
|<span data-ttu-id="7fa6d-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="7fa6d-115">connectionPending</span></span>|<span data-ttu-id="7fa6d-116">1</span><span class="sxs-lookup"><span data-stu-id="7fa6d-116">1</span></span>|<span data-ttu-id="7fa6d-117">挂起的连接到 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="7fa6d-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="7fa6d-118">连接</span><span class="sxs-lookup"><span data-stu-id="7fa6d-118">connected</span></span>|<span data-ttu-id="7fa6d-119">2</span><span class="sxs-lookup"><span data-stu-id="7fa6d-119">2</span></span>|<span data-ttu-id="7fa6d-120">连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="7fa6d-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="7fa6d-121">断开连接</span><span class="sxs-lookup"><span data-stu-id="7fa6d-121">disconnected</span></span>|<span data-ttu-id="7fa6d-122">3</span><span class="sxs-lookup"><span data-stu-id="7fa6d-122">3</span></span>|<span data-ttu-id="7fa6d-123">从 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="7fa6d-123">Disconnected from the Exchange Environment</span></span>|





