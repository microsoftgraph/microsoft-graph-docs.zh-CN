---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9cee18df0fe6ba3cc59d8d427aa472f8943e03d9
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527794"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="66d9a-103">deviceManagementDomainJoinConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="66d9a-103">deviceManagementDomainJoinConnectorState enum type</span></span>

<span data-ttu-id="66d9a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="66d9a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="66d9a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="66d9a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="66d9a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="66d9a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="66d9a-107">ODJ 请求状态。</span><span class="sxs-lookup"><span data-stu-id="66d9a-107">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="66d9a-108">成员</span><span class="sxs-lookup"><span data-stu-id="66d9a-108">Members</span></span>
|<span data-ttu-id="66d9a-109">成员</span><span class="sxs-lookup"><span data-stu-id="66d9a-109">Member</span></span>|<span data-ttu-id="66d9a-110">值</span><span class="sxs-lookup"><span data-stu-id="66d9a-110">Value</span></span>|<span data-ttu-id="66d9a-111">说明</span><span class="sxs-lookup"><span data-stu-id="66d9a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66d9a-112">工作</span><span class="sxs-lookup"><span data-stu-id="66d9a-112">active</span></span>|<span data-ttu-id="66d9a-113">0</span><span class="sxs-lookup"><span data-stu-id="66d9a-113">0</span></span>|<span data-ttu-id="66d9a-114">连接器积极 ping Intune。</span><span class="sxs-lookup"><span data-stu-id="66d9a-114">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="66d9a-115">error</span><span class="sxs-lookup"><span data-stu-id="66d9a-115">error</span></span>|<span data-ttu-id="66d9a-116">1 </span><span class="sxs-lookup"><span data-stu-id="66d9a-116">1</span></span>|<span data-ttu-id="66d9a-117">来自最近一小时内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="66d9a-117">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="66d9a-118">不再</span><span class="sxs-lookup"><span data-stu-id="66d9a-118">inactive</span></span>|<span data-ttu-id="66d9a-119">2 </span><span class="sxs-lookup"><span data-stu-id="66d9a-119">2</span></span>|<span data-ttu-id="66d9a-120">来自过去5天内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="66d9a-120">There is no heart-beat from connector from last 5 days.</span></span>|



