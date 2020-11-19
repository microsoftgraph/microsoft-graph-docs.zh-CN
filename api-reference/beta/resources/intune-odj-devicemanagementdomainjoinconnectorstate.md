---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 58b0a3a9e590913d0415062d6737fc6d9c33c451
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49222756"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="4a0a2-103">deviceManagementDomainJoinConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4a0a2-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="4a0a2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a0a2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4a0a2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a0a2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a0a2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a0a2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a0a2-107">ODJ 请求状态。</span><span class="sxs-lookup"><span data-stu-id="4a0a2-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="4a0a2-108">成员</span><span class="sxs-lookup"><span data-stu-id="4a0a2-108">Members</span></span>
|<span data-ttu-id="4a0a2-109">成员</span><span class="sxs-lookup"><span data-stu-id="4a0a2-109">Member</span></span>|<span data-ttu-id="4a0a2-110">值</span><span class="sxs-lookup"><span data-stu-id="4a0a2-110">Value</span></span>|<span data-ttu-id="4a0a2-111">说明</span><span class="sxs-lookup"><span data-stu-id="4a0a2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a0a2-112">工作</span><span class="sxs-lookup"><span data-stu-id="4a0a2-112">active</span></span>|<span data-ttu-id="4a0a2-113">0</span><span class="sxs-lookup"><span data-stu-id="4a0a2-113">0</span></span>|<span data-ttu-id="4a0a2-114">连接器积极 ping Intune。</span><span class="sxs-lookup"><span data-stu-id="4a0a2-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="4a0a2-115">error</span><span class="sxs-lookup"><span data-stu-id="4a0a2-115">error</span></span>|<span data-ttu-id="4a0a2-116">1</span><span class="sxs-lookup"><span data-stu-id="4a0a2-116">1</span></span>|<span data-ttu-id="4a0a2-117">来自最近一小时内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="4a0a2-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="4a0a2-118">不再</span><span class="sxs-lookup"><span data-stu-id="4a0a2-118">inactive</span></span>|<span data-ttu-id="4a0a2-119">双面</span><span class="sxs-lookup"><span data-stu-id="4a0a2-119">2</span></span>|<span data-ttu-id="4a0a2-120">来自过去5天内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="4a0a2-120">There is no heart-beat from connector from last 5 days.</span></span>|




