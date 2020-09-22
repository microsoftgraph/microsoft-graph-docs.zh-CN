---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 0698e527a75c414b714f9b00f61f2c2f7c036388
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081564"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="0dd4c-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0dd4c-103">certificateRevocationStatus enum type</span></span>

<span data-ttu-id="0dd4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0dd4c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0dd4c-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dd4c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dd4c-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-107">Certificate Revocation Status.</span></span>

## <a name="members"></a><span data-ttu-id="0dd4c-108">成员</span><span class="sxs-lookup"><span data-stu-id="0dd4c-108">Members</span></span>
|<span data-ttu-id="0dd4c-109">成员</span><span class="sxs-lookup"><span data-stu-id="0dd4c-109">Member</span></span>|<span data-ttu-id="0dd4c-110">值</span><span class="sxs-lookup"><span data-stu-id="0dd4c-110">Value</span></span>|<span data-ttu-id="0dd4c-111">说明</span><span class="sxs-lookup"><span data-stu-id="0dd4c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dd4c-112">无</span><span class="sxs-lookup"><span data-stu-id="0dd4c-112">none</span></span>|<span data-ttu-id="0dd4c-113">0</span><span class="sxs-lookup"><span data-stu-id="0dd4c-113">0</span></span>|<span data-ttu-id="0dd4c-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-114">Not revoked.</span></span>|
|<span data-ttu-id="0dd4c-115">决</span><span class="sxs-lookup"><span data-stu-id="0dd4c-115">pending</span></span>|<span data-ttu-id="0dd4c-116">1 </span><span class="sxs-lookup"><span data-stu-id="0dd4c-116">1</span></span>|<span data-ttu-id="0dd4c-117">撤销挂起。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-117">Revocation pending.</span></span>|
|<span data-ttu-id="0dd4c-118">io</span><span class="sxs-lookup"><span data-stu-id="0dd4c-118">issued</span></span>|<span data-ttu-id="0dd4c-119">2 </span><span class="sxs-lookup"><span data-stu-id="0dd4c-119">2</span></span>|<span data-ttu-id="0dd4c-120">已发出吊销命令。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-120">Revocation command issued.</span></span>|
|<span data-ttu-id="0dd4c-121">未能</span><span class="sxs-lookup"><span data-stu-id="0dd4c-121">failed</span></span>|<span data-ttu-id="0dd4c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="0dd4c-122">3</span></span>|<span data-ttu-id="0dd4c-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="0dd4c-123">Revocation failed.</span></span>|
|<span data-ttu-id="0dd4c-124">吊销</span><span class="sxs-lookup"><span data-stu-id="0dd4c-124">revoked</span></span>|<span data-ttu-id="0dd4c-125">4 </span><span class="sxs-lookup"><span data-stu-id="0dd4c-125">4</span></span>|<span data-ttu-id="0dd4c-126">吊销.</span><span class="sxs-lookup"><span data-stu-id="0dd4c-126">Revoked.</span></span>|






