---
title: deviceManagementExchangeConnectorStatus 枚举类型
description: Exchange Connector 的当前状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 472cc91b97547459694239c07bd211d1bd4ba1be
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32565963"
---
# <a name="devicemanagementexchangeconnectorstatus-enum-type"></a><span data-ttu-id="c707b-103">deviceManagementExchangeConnectorStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c707b-103">deviceManagementExchangeConnectorStatus enum type</span></span>

> <span data-ttu-id="c707b-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c707b-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c707b-105">Exchange Connector 的当前状态。</span><span class="sxs-lookup"><span data-stu-id="c707b-105">The current status of the Exchange Connector.</span></span>

## <a name="members"></a><span data-ttu-id="c707b-106">成员</span><span class="sxs-lookup"><span data-stu-id="c707b-106">Members</span></span>
|<span data-ttu-id="c707b-107">成员</span><span class="sxs-lookup"><span data-stu-id="c707b-107">Member</span></span>|<span data-ttu-id="c707b-108">值</span><span class="sxs-lookup"><span data-stu-id="c707b-108">Value</span></span>|<span data-ttu-id="c707b-109">说明</span><span class="sxs-lookup"><span data-stu-id="c707b-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c707b-110">无</span><span class="sxs-lookup"><span data-stu-id="c707b-110">none</span></span>|<span data-ttu-id="c707b-111">0</span><span class="sxs-lookup"><span data-stu-id="c707b-111">0</span></span>|<span data-ttu-id="c707b-112">不存在任何连接器。</span><span class="sxs-lookup"><span data-stu-id="c707b-112">No Connector exists.</span></span>|
|<span data-ttu-id="c707b-113">connectionPending</span><span class="sxs-lookup"><span data-stu-id="c707b-113">connectionPending</span></span>|<span data-ttu-id="c707b-114">1</span><span class="sxs-lookup"><span data-stu-id="c707b-114">1</span></span>|<span data-ttu-id="c707b-115">与 Exchange 环境的挂起连接。</span><span class="sxs-lookup"><span data-stu-id="c707b-115">Pending Connection to the Exchange Environment.</span></span>|
|<span data-ttu-id="c707b-116">连</span><span class="sxs-lookup"><span data-stu-id="c707b-116">connected</span></span>|<span data-ttu-id="c707b-117">2 </span><span class="sxs-lookup"><span data-stu-id="c707b-117">2</span></span>|<span data-ttu-id="c707b-118">已连接到 Exchange 环境</span><span class="sxs-lookup"><span data-stu-id="c707b-118">Connected to the Exchange Environment</span></span>|
|<span data-ttu-id="c707b-119">被</span><span class="sxs-lookup"><span data-stu-id="c707b-119">disconnected</span></span>|<span data-ttu-id="c707b-120">3 </span><span class="sxs-lookup"><span data-stu-id="c707b-120">3</span></span>|<span data-ttu-id="c707b-121">断开与 Exchange 环境的连接</span><span class="sxs-lookup"><span data-stu-id="c707b-121">Disconnected from the Exchange Environment</span></span>|



