---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange 连接器的当前状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 16181c49b05c74ef680f456b4bffd11b435299fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397769"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="25645-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="25645-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="25645-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="25645-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="25645-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="25645-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="25645-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25645-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25645-107">Exchange 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="25645-107">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="25645-108">成员</span><span class="sxs-lookup"><span data-stu-id="25645-108">Members</span></span>
|<span data-ttu-id="25645-109">成员</span><span class="sxs-lookup"><span data-stu-id="25645-109">Member</span></span>|<span data-ttu-id="25645-110">值</span><span class="sxs-lookup"><span data-stu-id="25645-110">Value</span></span>|<span data-ttu-id="25645-111">说明</span><span class="sxs-lookup"><span data-stu-id="25645-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25645-112">无</span><span class="sxs-lookup"><span data-stu-id="25645-112">none</span></span>|<span data-ttu-id="25645-113">0</span><span class="sxs-lookup"><span data-stu-id="25645-113">0</span></span>|<span data-ttu-id="25645-114">没有连接线存在。</span><span class="sxs-lookup"><span data-stu-id="25645-114">No Connector exists.</span></span>|
|<span data-ttu-id="25645-115">connectionPending</span><span class="sxs-lookup"><span data-stu-id="25645-115">connectionPending</span></span>|<span data-ttu-id="25645-116">1</span><span class="sxs-lookup"><span data-stu-id="25645-116">1</span></span>|<span data-ttu-id="25645-117">挂起的连接到 Exchange 环境。</span><span class="sxs-lookup"><span data-stu-id="25645-117">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="25645-118">连接</span><span class="sxs-lookup"><span data-stu-id="25645-118">connected</span></span>|<span data-ttu-id="25645-119">2</span><span class="sxs-lookup"><span data-stu-id="25645-119">2</span></span>|<span data-ttu-id="25645-120">连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="25645-120">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="25645-121">断开连接</span><span class="sxs-lookup"><span data-stu-id="25645-121">disconnected</span></span>|<span data-ttu-id="25645-122">3</span><span class="sxs-lookup"><span data-stu-id="25645-122">3</span></span>|<span data-ttu-id="25645-123">从 Exchange 环境断开连接</span><span class="sxs-lookup"><span data-stu-id="25645-123">Disconnected from the Exchange Environment</span></span>|




