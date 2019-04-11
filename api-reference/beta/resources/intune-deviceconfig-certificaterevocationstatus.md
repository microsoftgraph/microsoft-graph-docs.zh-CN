---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5fd9a6cd34df322a057d16e3d803d8685f7cd173
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31782805"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="894d0-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="894d0-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="894d0-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="894d0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="894d0-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="894d0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="894d0-106">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="894d0-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="894d0-107">成员</span><span class="sxs-lookup"><span data-stu-id="894d0-107">Members</span></span>
|<span data-ttu-id="894d0-108">成员</span><span class="sxs-lookup"><span data-stu-id="894d0-108">Member</span></span>|<span data-ttu-id="894d0-109">值</span><span class="sxs-lookup"><span data-stu-id="894d0-109">Value</span></span>|<span data-ttu-id="894d0-110">说明</span><span class="sxs-lookup"><span data-stu-id="894d0-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="894d0-111">无</span><span class="sxs-lookup"><span data-stu-id="894d0-111">none</span></span>|<span data-ttu-id="894d0-112">0</span><span class="sxs-lookup"><span data-stu-id="894d0-112">0</span></span>|<span data-ttu-id="894d0-113">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="894d0-113">Not revoked.</span></span>|
|<span data-ttu-id="894d0-114">决</span><span class="sxs-lookup"><span data-stu-id="894d0-114">pending</span></span>|<span data-ttu-id="894d0-115">1</span><span class="sxs-lookup"><span data-stu-id="894d0-115">1</span></span>|<span data-ttu-id="894d0-116">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="894d0-116">Revocation pending.</span></span>|
|<span data-ttu-id="894d0-117">io</span><span class="sxs-lookup"><span data-stu-id="894d0-117">issued</span></span>|<span data-ttu-id="894d0-118">双面</span><span class="sxs-lookup"><span data-stu-id="894d0-118">2</span></span>|<span data-ttu-id="894d0-119">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="894d0-119">Revocation command issued.</span></span>|
|<span data-ttu-id="894d0-120">未能</span><span class="sxs-lookup"><span data-stu-id="894d0-120">failed</span></span>|<span data-ttu-id="894d0-121">第三章</span><span class="sxs-lookup"><span data-stu-id="894d0-121">3</span></span>|<span data-ttu-id="894d0-122">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="894d0-122">Revocation failed.</span></span>|
|<span data-ttu-id="894d0-123">吊销</span><span class="sxs-lookup"><span data-stu-id="894d0-123">revoked</span></span>|<span data-ttu-id="894d0-124">4</span><span class="sxs-lookup"><span data-stu-id="894d0-124">4</span></span>|<span data-ttu-id="894d0-125">吊销.</span><span class="sxs-lookup"><span data-stu-id="894d0-125">Revoked.</span></span>|





