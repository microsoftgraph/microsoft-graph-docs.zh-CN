---
title: deviceManagementDomainJoinConnectorState 枚举类型
description: ODJ 请求状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: e8eff02a8ff4d47f920bad6506bcb9e3b37f0785
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42779882"
---
# <a name="devicemanagementdomainjoinconnectorstate-enum-type"></a><span data-ttu-id="9a986-103">deviceManagementDomainJoinConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9a986-103">deviceManagementDomainJoinConnectorState enum type</span></span>

> <span data-ttu-id="9a986-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a986-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a986-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a986-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a986-106">ODJ 请求状态。</span><span class="sxs-lookup"><span data-stu-id="9a986-106">The ODJ request states.</span></span>

## <a name="members"></a><span data-ttu-id="9a986-107">成员</span><span class="sxs-lookup"><span data-stu-id="9a986-107">Members</span></span>
|<span data-ttu-id="9a986-108">成员</span><span class="sxs-lookup"><span data-stu-id="9a986-108">Member</span></span>|<span data-ttu-id="9a986-109">值</span><span class="sxs-lookup"><span data-stu-id="9a986-109">Value</span></span>|<span data-ttu-id="9a986-110">说明</span><span class="sxs-lookup"><span data-stu-id="9a986-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a986-111">工作</span><span class="sxs-lookup"><span data-stu-id="9a986-111">active</span></span>|<span data-ttu-id="9a986-112">0</span><span class="sxs-lookup"><span data-stu-id="9a986-112">0</span></span>|<span data-ttu-id="9a986-113">连接器积极 ping Intune。</span><span class="sxs-lookup"><span data-stu-id="9a986-113">Connector is actively pinging Intune.</span></span>|
|<span data-ttu-id="9a986-114">error</span><span class="sxs-lookup"><span data-stu-id="9a986-114">error</span></span>|<span data-ttu-id="9a986-115">1</span><span class="sxs-lookup"><span data-stu-id="9a986-115">1</span></span>|<span data-ttu-id="9a986-116">来自最近一小时内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="9a986-116">There is no heart-beat from connector from last one hour.</span></span>|
|<span data-ttu-id="9a986-117">不再</span><span class="sxs-lookup"><span data-stu-id="9a986-117">inactive</span></span>|<span data-ttu-id="9a986-118">双面</span><span class="sxs-lookup"><span data-stu-id="9a986-118">2</span></span>|<span data-ttu-id="9a986-119">来自过去5天内的连接器没有任何信号。</span><span class="sxs-lookup"><span data-stu-id="9a986-119">There is no heart-beat from connector from last 5 days.</span></span>|



