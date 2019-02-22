---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c182cf2317f185108570116a283973d481f17ab2
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159442"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="3c763-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="3c763-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="3c763-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c763-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c763-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c763-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c763-106">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="3c763-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="3c763-107">成员</span><span class="sxs-lookup"><span data-stu-id="3c763-107">Members</span></span>
|<span data-ttu-id="3c763-108">成员</span><span class="sxs-lookup"><span data-stu-id="3c763-108">Member</span></span>|<span data-ttu-id="3c763-109">值</span><span class="sxs-lookup"><span data-stu-id="3c763-109">Value</span></span>|<span data-ttu-id="3c763-110">说明</span><span class="sxs-lookup"><span data-stu-id="3c763-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c763-111">无</span><span class="sxs-lookup"><span data-stu-id="3c763-111">none</span></span>|<span data-ttu-id="3c763-112">0</span><span class="sxs-lookup"><span data-stu-id="3c763-112">0</span></span>|<span data-ttu-id="3c763-113">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="3c763-113">Not revoked.</span></span>|
|<span data-ttu-id="3c763-114">决</span><span class="sxs-lookup"><span data-stu-id="3c763-114">pending</span></span>|<span data-ttu-id="3c763-115">1</span><span class="sxs-lookup"><span data-stu-id="3c763-115">1</span></span>|<span data-ttu-id="3c763-116">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="3c763-116">Revocation pending.</span></span>|
|<span data-ttu-id="3c763-117">io</span><span class="sxs-lookup"><span data-stu-id="3c763-117">issued</span></span>|<span data-ttu-id="3c763-118">双面</span><span class="sxs-lookup"><span data-stu-id="3c763-118">2</span></span>|<span data-ttu-id="3c763-119">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="3c763-119">Revocation command issued.</span></span>|
|<span data-ttu-id="3c763-120">failed</span><span class="sxs-lookup"><span data-stu-id="3c763-120">failed</span></span>|<span data-ttu-id="3c763-121">第三章</span><span class="sxs-lookup"><span data-stu-id="3c763-121">3</span></span>|<span data-ttu-id="3c763-122">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="3c763-122">Revocation failed.</span></span>|
|<span data-ttu-id="3c763-123">吊销</span><span class="sxs-lookup"><span data-stu-id="3c763-123">revoked</span></span>|<span data-ttu-id="3c763-124">4</span><span class="sxs-lookup"><span data-stu-id="3c763-124">4</span></span>|<span data-ttu-id="3c763-125">吊销.</span><span class="sxs-lookup"><span data-stu-id="3c763-125">Revoked.</span></span>|




