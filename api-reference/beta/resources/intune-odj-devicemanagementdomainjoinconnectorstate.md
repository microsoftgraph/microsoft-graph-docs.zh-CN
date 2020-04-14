---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 919b8e22b119b211cea4b897c7f2f7c713307e02
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43419114"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="aefe7-103">deviceManagementDomainJoinConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aefe7-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="aefe7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aefe7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aefe7-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aefe7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aefe7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aefe7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aefe7-107">ODJ 请求状态。</span><span class="sxs-lookup"><span data-stu-id="aefe7-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="aefe7-108">成员</span><span class="sxs-lookup"><span data-stu-id="aefe7-108">Members</span></span>
|<span data-ttu-id="aefe7-109">成员</span><span class="sxs-lookup"><span data-stu-id="aefe7-109">Member</span></span>|<span data-ttu-id="aefe7-110">值</span><span class="sxs-lookup"><span data-stu-id="aefe7-110">Value</span></span>|<span data-ttu-id="aefe7-111">说明</span><span class="sxs-lookup"><span data-stu-id="aefe7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aefe7-112">工作</span><span class="sxs-lookup"><span data-stu-id="aefe7-112">active</span></span>|<span data-ttu-id="aefe7-113">0</span><span class="sxs-lookup"><span data-stu-id="aefe7-113">0</span></span>|<span data-ttu-id="aefe7-114">连接器积极 ping Intune。</span><span class="sxs-lookup"><span data-stu-id="aefe7-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="aefe7-115">error</span><span class="sxs-lookup"><span data-stu-id="aefe7-115">error</span></span>|<span data-ttu-id="aefe7-116">1</span><span class="sxs-lookup"><span data-stu-id="aefe7-116">1</span></span>|<span data-ttu-id="aefe7-117">来自最近一小时内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="aefe7-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="aefe7-118">不再</span><span class="sxs-lookup"><span data-stu-id="aefe7-118">inactive</span></span>|<span data-ttu-id="aefe7-119">双面</span><span class="sxs-lookup"><span data-stu-id="aefe7-119">2</span></span>|<span data-ttu-id="aefe7-120">来自过去5天内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="aefe7-120">There is no heart-beat from connector from last 5 days.</span></span>|



