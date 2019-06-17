---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a584a77c0a921b9d5864270c5a42a9991123eb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "35001914"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="1e6fd-103">deviceManagementDomainJoinConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1e6fd-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="1e6fd-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e6fd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e6fd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e6fd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e6fd-106">ODJ 请求状态。</span><span class="sxs-lookup"><span data-stu-id="1e6fd-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="1e6fd-107">成员</span><span class="sxs-lookup"><span data-stu-id="1e6fd-107">Members</span></span>
|<span data-ttu-id="1e6fd-108">成员</span><span class="sxs-lookup"><span data-stu-id="1e6fd-108">Member</span></span>|<span data-ttu-id="1e6fd-109">值</span><span class="sxs-lookup"><span data-stu-id="1e6fd-109">Value</span></span>|<span data-ttu-id="1e6fd-110">说明</span><span class="sxs-lookup"><span data-stu-id="1e6fd-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e6fd-111">工作</span><span class="sxs-lookup"><span data-stu-id="1e6fd-111">active</span></span>|<span data-ttu-id="1e6fd-112">0</span><span class="sxs-lookup"><span data-stu-id="1e6fd-112">0</span></span>|<span data-ttu-id="1e6fd-113">连接器积极 ping Intune。</span><span class="sxs-lookup"><span data-stu-id="1e6fd-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="1e6fd-114">error</span><span class="sxs-lookup"><span data-stu-id="1e6fd-114">error</span></span>|<span data-ttu-id="1e6fd-115">1</span><span class="sxs-lookup"><span data-stu-id="1e6fd-115">1</span></span>|<span data-ttu-id="1e6fd-116">来自最近一小时内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="1e6fd-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="1e6fd-117">不再</span><span class="sxs-lookup"><span data-stu-id="1e6fd-117">inactive</span></span>|<span data-ttu-id="1e6fd-118">双面</span><span class="sxs-lookup"><span data-stu-id="1e6fd-118">2</span></span>|<span data-ttu-id="1e6fd-119">来自过去5天内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="1e6fd-119">There is no heart-beat from connector from last 5 days.</span></span>|





