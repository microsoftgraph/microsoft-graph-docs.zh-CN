---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4544968e473c41d787df606112801c9b60e2cb98
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33947426"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="0bea8-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0bea8-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="0bea8-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0bea8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0bea8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0bea8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0bea8-106">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="0bea8-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="0bea8-107">成员</span><span class="sxs-lookup"><span data-stu-id="0bea8-107">Members</span></span>
|<span data-ttu-id="0bea8-108">成员</span><span class="sxs-lookup"><span data-stu-id="0bea8-108">Member</span></span>|<span data-ttu-id="0bea8-109">值</span><span class="sxs-lookup"><span data-stu-id="0bea8-109">Value</span></span>|<span data-ttu-id="0bea8-110">说明</span><span class="sxs-lookup"><span data-stu-id="0bea8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0bea8-111">无</span><span class="sxs-lookup"><span data-stu-id="0bea8-111">none</span></span>|<span data-ttu-id="0bea8-112">0</span><span class="sxs-lookup"><span data-stu-id="0bea8-112">0</span></span>|<span data-ttu-id="0bea8-113">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="0bea8-113">Not revoked.</span></span>|
|<span data-ttu-id="0bea8-114">决</span><span class="sxs-lookup"><span data-stu-id="0bea8-114">pending</span></span>|<span data-ttu-id="0bea8-115">1</span><span class="sxs-lookup"><span data-stu-id="0bea8-115">1</span></span>|<span data-ttu-id="0bea8-116">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="0bea8-116">Revocation pending.</span></span>|
|<span data-ttu-id="0bea8-117">io</span><span class="sxs-lookup"><span data-stu-id="0bea8-117">issued</span></span>|<span data-ttu-id="0bea8-118">双面</span><span class="sxs-lookup"><span data-stu-id="0bea8-118">2</span></span>|<span data-ttu-id="0bea8-119">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="0bea8-119">Revocation command issued.</span></span>|
|<span data-ttu-id="0bea8-120">未能</span><span class="sxs-lookup"><span data-stu-id="0bea8-120">failed</span></span>|<span data-ttu-id="0bea8-121">第三章</span><span class="sxs-lookup"><span data-stu-id="0bea8-121">3</span></span>|<span data-ttu-id="0bea8-122">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="0bea8-122">Revocation failed.</span></span>|
|<span data-ttu-id="0bea8-123">吊销</span><span class="sxs-lookup"><span data-stu-id="0bea8-123">revoked</span></span>|<span data-ttu-id="0bea8-124">4</span><span class="sxs-lookup"><span data-stu-id="0bea8-124">4</span></span>|<span data-ttu-id="0bea8-125">吊销.</span><span class="sxs-lookup"><span data-stu-id="0bea8-125">Revoked.</span></span>|




