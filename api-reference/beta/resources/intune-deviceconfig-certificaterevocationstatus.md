---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9a1231373597096905d4e0614d4b1b6e2d70b6c6
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35971009"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="1b153-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b153-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="1b153-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b153-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b153-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b153-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b153-106">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="1b153-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="1b153-107">成员</span><span class="sxs-lookup"><span data-stu-id="1b153-107">Members</span></span>
|<span data-ttu-id="1b153-108">成员</span><span class="sxs-lookup"><span data-stu-id="1b153-108">Member</span></span>|<span data-ttu-id="1b153-109">值</span><span class="sxs-lookup"><span data-stu-id="1b153-109">Value</span></span>|<span data-ttu-id="1b153-110">说明</span><span class="sxs-lookup"><span data-stu-id="1b153-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b153-111">无</span><span class="sxs-lookup"><span data-stu-id="1b153-111">none</span></span>|<span data-ttu-id="1b153-112">0</span><span class="sxs-lookup"><span data-stu-id="1b153-112">0</span></span>|<span data-ttu-id="1b153-113">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="1b153-113">Not revoked.</span></span>|
|<span data-ttu-id="1b153-114">决</span><span class="sxs-lookup"><span data-stu-id="1b153-114">pending</span></span>|<span data-ttu-id="1b153-115">1</span><span class="sxs-lookup"><span data-stu-id="1b153-115">1</span></span>|<span data-ttu-id="1b153-116">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="1b153-116">Revocation pending.</span></span>|
|<span data-ttu-id="1b153-117">io</span><span class="sxs-lookup"><span data-stu-id="1b153-117">issued</span></span>|<span data-ttu-id="1b153-118">双面</span><span class="sxs-lookup"><span data-stu-id="1b153-118">2</span></span>|<span data-ttu-id="1b153-119">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="1b153-119">Revocation command issued.</span></span>|
|<span data-ttu-id="1b153-120">未能</span><span class="sxs-lookup"><span data-stu-id="1b153-120">failed</span></span>|<span data-ttu-id="1b153-121">第三章</span><span class="sxs-lookup"><span data-stu-id="1b153-121">3</span></span>|<span data-ttu-id="1b153-122">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="1b153-122">Revocation failed.</span></span>|
|<span data-ttu-id="1b153-123">吊销</span><span class="sxs-lookup"><span data-stu-id="1b153-123">revoked</span></span>|<span data-ttu-id="1b153-124">4</span><span class="sxs-lookup"><span data-stu-id="1b153-124">4</span></span>|<span data-ttu-id="1b153-125">吊销.</span><span class="sxs-lookup"><span data-stu-id="1b153-125">Revoked.</span></span>|





