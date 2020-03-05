---
title: ndesConnectorState 枚举类型
description: Ndes 连接器的当前状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d1f430b659a1ab2057a069cb2ede7997aab2613f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529593"
---
# <a name="ndesconnectorstate-enum-type"></a><span data-ttu-id="f5ed5-103">ndesConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5ed5-103">ndesConnectorState enum type</span></span>

<span data-ttu-id="f5ed5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="f5ed5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f5ed5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f5ed5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f5ed5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f5ed5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f5ed5-107">Ndes 连接器的当前状态。</span><span class="sxs-lookup"><span data-stu-id="f5ed5-107">The current status of the Ndes Connector.</span></span>

## <a name="members"></a><span data-ttu-id="f5ed5-108">成员</span><span class="sxs-lookup"><span data-stu-id="f5ed5-108">Members</span></span>
|<span data-ttu-id="f5ed5-109">成员</span><span class="sxs-lookup"><span data-stu-id="f5ed5-109">Member</span></span>|<span data-ttu-id="f5ed5-110">值</span><span class="sxs-lookup"><span data-stu-id="f5ed5-110">Value</span></span>|<span data-ttu-id="f5ed5-111">说明</span><span class="sxs-lookup"><span data-stu-id="f5ed5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5ed5-112">无</span><span class="sxs-lookup"><span data-stu-id="f5ed5-112">none</span></span>|<span data-ttu-id="f5ed5-113">0</span><span class="sxs-lookup"><span data-stu-id="f5ed5-113">0</span></span>|<span data-ttu-id="f5ed5-114">尚不提供此连接器的状态。</span><span class="sxs-lookup"><span data-stu-id="f5ed5-114">State not available yet for this connector.</span></span>|
|<span data-ttu-id="f5ed5-115">工作</span><span class="sxs-lookup"><span data-stu-id="f5ed5-115">active</span></span>|<span data-ttu-id="f5ed5-116">1 </span><span class="sxs-lookup"><span data-stu-id="f5ed5-116">1</span></span>|<span data-ttu-id="f5ed5-117">Ndes 连接器最近已连接</span><span class="sxs-lookup"><span data-stu-id="f5ed5-117">Ndes connector has connected recently</span></span>|
|<span data-ttu-id="f5ed5-118">不再</span><span class="sxs-lookup"><span data-stu-id="f5ed5-118">inactive</span></span>|<span data-ttu-id="f5ed5-119">2 </span><span class="sxs-lookup"><span data-stu-id="f5ed5-119">2</span></span>|<span data-ttu-id="f5ed5-120">Ndes 连接器的最近活动</span><span class="sxs-lookup"><span data-stu-id="f5ed5-120">No recent activity for the Ndes connector</span></span>|



