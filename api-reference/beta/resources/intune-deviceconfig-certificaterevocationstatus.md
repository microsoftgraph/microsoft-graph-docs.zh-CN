---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8d24d515f992ed396c3530595240a107852d83e1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868304"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="80677-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="80677-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="80677-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80677-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80677-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80677-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80677-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80677-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80677-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="80677-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="80677-108">成员</span><span class="sxs-lookup"><span data-stu-id="80677-108">Members</span></span>
|<span data-ttu-id="80677-109">成员</span><span class="sxs-lookup"><span data-stu-id="80677-109">Member</span></span>|<span data-ttu-id="80677-110">值</span><span class="sxs-lookup"><span data-stu-id="80677-110">Value</span></span>|<span data-ttu-id="80677-111">Description</span><span class="sxs-lookup"><span data-stu-id="80677-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80677-112">无</span><span class="sxs-lookup"><span data-stu-id="80677-112">none</span></span>|<span data-ttu-id="80677-113">0</span><span class="sxs-lookup"><span data-stu-id="80677-113">0</span></span>|<span data-ttu-id="80677-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="80677-114">Not revoked.</span></span>|
|<span data-ttu-id="80677-115">挂起</span><span class="sxs-lookup"><span data-stu-id="80677-115">pending</span></span>|<span data-ttu-id="80677-116">1</span><span class="sxs-lookup"><span data-stu-id="80677-116">1</span></span>|<span data-ttu-id="80677-117">待处理的吊销。</span><span class="sxs-lookup"><span data-stu-id="80677-117">Revocation pending.</span></span>|
|<span data-ttu-id="80677-118">颁发</span><span class="sxs-lookup"><span data-stu-id="80677-118">issued</span></span>|<span data-ttu-id="80677-119">2</span><span class="sxs-lookup"><span data-stu-id="80677-119">2</span></span>|<span data-ttu-id="80677-120">吊销发出命令。</span><span class="sxs-lookup"><span data-stu-id="80677-120">Revocation command issued.</span></span>|
|<span data-ttu-id="80677-121">failed</span><span class="sxs-lookup"><span data-stu-id="80677-121">failed</span></span>|<span data-ttu-id="80677-122">3</span><span class="sxs-lookup"><span data-stu-id="80677-122">3</span></span>|<span data-ttu-id="80677-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="80677-123">Revocation failed.</span></span>|
|<span data-ttu-id="80677-124">吊销</span><span class="sxs-lookup"><span data-stu-id="80677-124">revoked</span></span>|<span data-ttu-id="80677-125">4</span><span class="sxs-lookup"><span data-stu-id="80677-125">4</span></span>|<span data-ttu-id="80677-126">吊销。</span><span class="sxs-lookup"><span data-stu-id="80677-126">Revoked.</span></span>|





