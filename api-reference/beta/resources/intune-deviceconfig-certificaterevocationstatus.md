---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8c1c77e267da5528088a7a8ef6400a872790aaf3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27983119"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="168e9-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="168e9-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="168e9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="168e9-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="168e9-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="168e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="168e9-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="168e9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="168e9-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="168e9-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="168e9-108">成员</span><span class="sxs-lookup"><span data-stu-id="168e9-108">Members</span></span>
|<span data-ttu-id="168e9-109">成员</span><span class="sxs-lookup"><span data-stu-id="168e9-109">Member</span></span>|<span data-ttu-id="168e9-110">值</span><span class="sxs-lookup"><span data-stu-id="168e9-110">Value</span></span>|<span data-ttu-id="168e9-111">说明</span><span class="sxs-lookup"><span data-stu-id="168e9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="168e9-112">无</span><span class="sxs-lookup"><span data-stu-id="168e9-112">none</span></span>|<span data-ttu-id="168e9-113">0</span><span class="sxs-lookup"><span data-stu-id="168e9-113">0</span></span>|<span data-ttu-id="168e9-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="168e9-114">Not revoked.</span></span>|
|<span data-ttu-id="168e9-115">挂起</span><span class="sxs-lookup"><span data-stu-id="168e9-115">pending</span></span>|<span data-ttu-id="168e9-116">1</span><span class="sxs-lookup"><span data-stu-id="168e9-116">1</span></span>|<span data-ttu-id="168e9-117">待处理的吊销。</span><span class="sxs-lookup"><span data-stu-id="168e9-117">Revocation pending.</span></span>|
|<span data-ttu-id="168e9-118">颁发</span><span class="sxs-lookup"><span data-stu-id="168e9-118">issued</span></span>|<span data-ttu-id="168e9-119">2</span><span class="sxs-lookup"><span data-stu-id="168e9-119">2</span></span>|<span data-ttu-id="168e9-120">吊销发出命令。</span><span class="sxs-lookup"><span data-stu-id="168e9-120">Revocation command issued.</span></span>|
|<span data-ttu-id="168e9-121">failed</span><span class="sxs-lookup"><span data-stu-id="168e9-121">failed</span></span>|<span data-ttu-id="168e9-122">3</span><span class="sxs-lookup"><span data-stu-id="168e9-122">3</span></span>|<span data-ttu-id="168e9-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="168e9-123">Revocation failed.</span></span>|
|<span data-ttu-id="168e9-124">吊销</span><span class="sxs-lookup"><span data-stu-id="168e9-124">revoked</span></span>|<span data-ttu-id="168e9-125">4</span><span class="sxs-lookup"><span data-stu-id="168e9-125">4</span></span>|<span data-ttu-id="168e9-126">吊销。</span><span class="sxs-lookup"><span data-stu-id="168e9-126">Revoked.</span></span>|





