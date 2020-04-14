---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 8d449fc723fd4c3a03c9a72bdbc74768b7db698c
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43402229"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="fc18d-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fc18d-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="fc18d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc18d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc18d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc18d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc18d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc18d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc18d-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="fc18d-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="fc18d-108">成员</span><span class="sxs-lookup"><span data-stu-id="fc18d-108">Members</span></span>
|<span data-ttu-id="fc18d-109">成员</span><span class="sxs-lookup"><span data-stu-id="fc18d-109">Member</span></span>|<span data-ttu-id="fc18d-110">值</span><span class="sxs-lookup"><span data-stu-id="fc18d-110">Value</span></span>|<span data-ttu-id="fc18d-111">说明</span><span class="sxs-lookup"><span data-stu-id="fc18d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc18d-112">无</span><span class="sxs-lookup"><span data-stu-id="fc18d-112">none</span></span>|<span data-ttu-id="fc18d-113">0</span><span class="sxs-lookup"><span data-stu-id="fc18d-113">0</span></span>|<span data-ttu-id="fc18d-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="fc18d-114">Not revoked.</span></span>|
|<span data-ttu-id="fc18d-115">决</span><span class="sxs-lookup"><span data-stu-id="fc18d-115">pending</span></span>|<span data-ttu-id="fc18d-116">1</span><span class="sxs-lookup"><span data-stu-id="fc18d-116">1</span></span>|<span data-ttu-id="fc18d-117">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="fc18d-117">Revocation pending.</span></span>|
|<span data-ttu-id="fc18d-118">io</span><span class="sxs-lookup"><span data-stu-id="fc18d-118">issued</span></span>|<span data-ttu-id="fc18d-119">双面</span><span class="sxs-lookup"><span data-stu-id="fc18d-119">2</span></span>|<span data-ttu-id="fc18d-120">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="fc18d-120">Revocation command issued.</span></span>|
|<span data-ttu-id="fc18d-121">未能</span><span class="sxs-lookup"><span data-stu-id="fc18d-121">failed</span></span>|<span data-ttu-id="fc18d-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fc18d-122">3</span></span>|<span data-ttu-id="fc18d-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="fc18d-123">Revocation failed.</span></span>|
|<span data-ttu-id="fc18d-124">吊销</span><span class="sxs-lookup"><span data-stu-id="fc18d-124">revoked</span></span>|<span data-ttu-id="fc18d-125">4 </span><span class="sxs-lookup"><span data-stu-id="fc18d-125">4</span></span>|<span data-ttu-id="fc18d-126">吊销.</span><span class="sxs-lookup"><span data-stu-id="fc18d-126">Revoked.</span></span>|



