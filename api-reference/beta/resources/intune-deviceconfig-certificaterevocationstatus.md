---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f0e0342924faf166e6daf0a66149e841b88d6d0c
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42795692"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="b86cb-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b86cb-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="b86cb-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b86cb-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b86cb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b86cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b86cb-106">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="b86cb-106">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="b86cb-107">成员</span><span class="sxs-lookup"><span data-stu-id="b86cb-107">Members</span></span>
|<span data-ttu-id="b86cb-108">成员</span><span class="sxs-lookup"><span data-stu-id="b86cb-108">Member</span></span>|<span data-ttu-id="b86cb-109">值</span><span class="sxs-lookup"><span data-stu-id="b86cb-109">Value</span></span>|<span data-ttu-id="b86cb-110">说明</span><span class="sxs-lookup"><span data-stu-id="b86cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b86cb-111">无</span><span class="sxs-lookup"><span data-stu-id="b86cb-111">none</span></span>|<span data-ttu-id="b86cb-112">0</span><span class="sxs-lookup"><span data-stu-id="b86cb-112">0</span></span>|<span data-ttu-id="b86cb-113">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="b86cb-113">Not revoked.</span></span>|
|<span data-ttu-id="b86cb-114">决</span><span class="sxs-lookup"><span data-stu-id="b86cb-114">pending</span></span>|<span data-ttu-id="b86cb-115">1</span><span class="sxs-lookup"><span data-stu-id="b86cb-115">1</span></span>|<span data-ttu-id="b86cb-116">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="b86cb-116">Revocation pending.</span></span>|
|<span data-ttu-id="b86cb-117">io</span><span class="sxs-lookup"><span data-stu-id="b86cb-117">issued</span></span>|<span data-ttu-id="b86cb-118">双面</span><span class="sxs-lookup"><span data-stu-id="b86cb-118">2</span></span>|<span data-ttu-id="b86cb-119">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="b86cb-119">Revocation command issued.</span></span>|
|<span data-ttu-id="b86cb-120">未能</span><span class="sxs-lookup"><span data-stu-id="b86cb-120">failed</span></span>|<span data-ttu-id="b86cb-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b86cb-121">3</span></span>|<span data-ttu-id="b86cb-122">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="b86cb-122">Revocation failed.</span></span>|
|<span data-ttu-id="b86cb-123">吊销</span><span class="sxs-lookup"><span data-stu-id="b86cb-123">revoked</span></span>|<span data-ttu-id="b86cb-124">4 </span><span class="sxs-lookup"><span data-stu-id="b86cb-124">4</span></span>|<span data-ttu-id="b86cb-125">吊销.</span><span class="sxs-lookup"><span data-stu-id="b86cb-125">Revoked.</span></span>|



