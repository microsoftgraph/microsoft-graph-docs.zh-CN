---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 870cf8a59dc2f7a8ae26f3e7a76dd49249b0e008
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526980"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="55b4a-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="55b4a-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="55b4a-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="55b4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="55b4a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="55b4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="55b4a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="55b4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55b4a-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="55b4a-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="55b4a-108">成员</span><span class="sxs-lookup"><span data-stu-id="55b4a-108">Members</span></span>
|<span data-ttu-id="55b4a-109">成员</span><span class="sxs-lookup"><span data-stu-id="55b4a-109">Member</span></span>|<span data-ttu-id="55b4a-110">值</span><span class="sxs-lookup"><span data-stu-id="55b4a-110">Value</span></span>|<span data-ttu-id="55b4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="55b4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55b4a-112">无</span><span class="sxs-lookup"><span data-stu-id="55b4a-112">none</span></span>|<span data-ttu-id="55b4a-113">0</span><span class="sxs-lookup"><span data-stu-id="55b4a-113">0</span></span>|<span data-ttu-id="55b4a-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="55b4a-114">Not revoked.</span></span>|
|<span data-ttu-id="55b4a-115">决</span><span class="sxs-lookup"><span data-stu-id="55b4a-115">pending</span></span>|<span data-ttu-id="55b4a-116">1 </span><span class="sxs-lookup"><span data-stu-id="55b4a-116">1</span></span>|<span data-ttu-id="55b4a-117">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="55b4a-117">Revocation pending.</span></span>|
|<span data-ttu-id="55b4a-118">io</span><span class="sxs-lookup"><span data-stu-id="55b4a-118">issued</span></span>|<span data-ttu-id="55b4a-119">2 </span><span class="sxs-lookup"><span data-stu-id="55b4a-119">2</span></span>|<span data-ttu-id="55b4a-120">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="55b4a-120">Revocation command issued.</span></span>|
|<span data-ttu-id="55b4a-121">未能</span><span class="sxs-lookup"><span data-stu-id="55b4a-121">failed</span></span>|<span data-ttu-id="55b4a-122">3 </span><span class="sxs-lookup"><span data-stu-id="55b4a-122">3</span></span>|<span data-ttu-id="55b4a-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="55b4a-123">Revocation failed.</span></span>|
|<span data-ttu-id="55b4a-124">吊销</span><span class="sxs-lookup"><span data-stu-id="55b4a-124">revoked</span></span>|<span data-ttu-id="55b4a-125">4 </span><span class="sxs-lookup"><span data-stu-id="55b4a-125">4</span></span>|<span data-ttu-id="55b4a-126">吊销.</span><span class="sxs-lookup"><span data-stu-id="55b4a-126">Revoked.</span></span>|



