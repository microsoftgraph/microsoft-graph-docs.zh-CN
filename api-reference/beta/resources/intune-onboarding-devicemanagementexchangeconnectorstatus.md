---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange Connector 的当前状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 87b45805c7beb15147cf90f8c2f6bef1b82ecb7f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32566617"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="a9ff5-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a9ff5-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="a9ff5-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9ff5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9ff5-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9ff5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9ff5-106">Exchange Connector 的当前状态。</span><span class="sxs-lookup"><span data-stu-id="a9ff5-106">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="a9ff5-107">成员</span><span class="sxs-lookup"><span data-stu-id="a9ff5-107">Members</span></span>
|<span data-ttu-id="a9ff5-108">成员</span><span class="sxs-lookup"><span data-stu-id="a9ff5-108">Member</span></span>|<span data-ttu-id="a9ff5-109">值</span><span class="sxs-lookup"><span data-stu-id="a9ff5-109">Value</span></span>|<span data-ttu-id="a9ff5-110">说明</span><span class="sxs-lookup"><span data-stu-id="a9ff5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9ff5-111">无</span><span class="sxs-lookup"><span data-stu-id="a9ff5-111">none</span></span>|<span data-ttu-id="a9ff5-112">0</span><span class="sxs-lookup"><span data-stu-id="a9ff5-112">0</span></span>|<span data-ttu-id="a9ff5-113">不存在任何连接器。</span><span class="sxs-lookup"><span data-stu-id="a9ff5-113">No Connector exists.</span></span>|
|<span data-ttu-id="a9ff5-114">connectionPending</span><span class="sxs-lookup"><span data-stu-id="a9ff5-114">connectionPending</span></span>|<span data-ttu-id="a9ff5-115">1</span><span class="sxs-lookup"><span data-stu-id="a9ff5-115">1</span></span>|<span data-ttu-id="a9ff5-116">与 Exchange 环境的挂起连接。</span><span class="sxs-lookup"><span data-stu-id="a9ff5-116">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="a9ff5-117">连</span><span class="sxs-lookup"><span data-stu-id="a9ff5-117">connected</span></span>|<span data-ttu-id="a9ff5-118">2 </span><span class="sxs-lookup"><span data-stu-id="a9ff5-118">2</span></span>|<span data-ttu-id="a9ff5-119">已连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="a9ff5-119">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="a9ff5-120">被</span><span class="sxs-lookup"><span data-stu-id="a9ff5-120">disconnected</span></span>|<span data-ttu-id="a9ff5-121">3 </span><span class="sxs-lookup"><span data-stu-id="a9ff5-121">3</span></span>|<span data-ttu-id="a9ff5-122">断开与 Exchange 环境的连接</span><span class="sxs-lookup"><span data-stu-id="a9ff5-122">Disconnected from the Exchange Environment</span></span>|





