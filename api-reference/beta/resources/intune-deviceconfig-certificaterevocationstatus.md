---
title: certificateRevocationStatus 枚举类型
description: 证书吊销状态。
author: tfitzmac
ms.openlocfilehash: d41845ba882136c15d944c8a7f91083e6fa47cdb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358224"
---
# <a name="certificaterevocationstatus-enum-type"></a><span data-ttu-id="a93af-103">certificateRevocationStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a93af-103">certificateRevocationStatus enum type</span></span>

> <span data-ttu-id="a93af-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a93af-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a93af-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a93af-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a93af-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a93af-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a93af-107">证书吊销状态。</span><span class="sxs-lookup"><span data-stu-id="a93af-107">Certificate Revocation Status.</span></span>
## <a name="members"></a><span data-ttu-id="a93af-108">成员</span><span class="sxs-lookup"><span data-stu-id="a93af-108">Members</span></span>
|<span data-ttu-id="a93af-109">成员</span><span class="sxs-lookup"><span data-stu-id="a93af-109">Member</span></span>|<span data-ttu-id="a93af-110">值</span><span class="sxs-lookup"><span data-stu-id="a93af-110">Value</span></span>|<span data-ttu-id="a93af-111">说明</span><span class="sxs-lookup"><span data-stu-id="a93af-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a93af-112">无</span><span class="sxs-lookup"><span data-stu-id="a93af-112">none</span></span>|<span data-ttu-id="a93af-113">0</span><span class="sxs-lookup"><span data-stu-id="a93af-113">0</span></span>|<span data-ttu-id="a93af-114">未被吊销。</span><span class="sxs-lookup"><span data-stu-id="a93af-114">Not revoked.</span></span>|
|<span data-ttu-id="a93af-115">挂起</span><span class="sxs-lookup"><span data-stu-id="a93af-115">pending</span></span>|<span data-ttu-id="a93af-116">1</span><span class="sxs-lookup"><span data-stu-id="a93af-116">1</span></span>|<span data-ttu-id="a93af-117">待处理的吊销。</span><span class="sxs-lookup"><span data-stu-id="a93af-117">Revocation pending.</span></span>|
|<span data-ttu-id="a93af-118">颁发</span><span class="sxs-lookup"><span data-stu-id="a93af-118">issued</span></span>|<span data-ttu-id="a93af-119">2</span><span class="sxs-lookup"><span data-stu-id="a93af-119">2</span></span>|<span data-ttu-id="a93af-120">吊销发出命令。</span><span class="sxs-lookup"><span data-stu-id="a93af-120">Revocation command issued.</span></span>|
|<span data-ttu-id="a93af-121">failed</span><span class="sxs-lookup"><span data-stu-id="a93af-121">failed</span></span>|<span data-ttu-id="a93af-122">3</span><span class="sxs-lookup"><span data-stu-id="a93af-122">3</span></span>|<span data-ttu-id="a93af-123">吊销失败。</span><span class="sxs-lookup"><span data-stu-id="a93af-123">Revocation failed.</span></span>|
|<span data-ttu-id="a93af-124">吊销</span><span class="sxs-lookup"><span data-stu-id="a93af-124">revoked</span></span>|<span data-ttu-id="a93af-125">4</span><span class="sxs-lookup"><span data-stu-id="a93af-125">4</span></span>|<span data-ttu-id="a93af-126">吊销。</span><span class="sxs-lookup"><span data-stu-id="a93af-126">Revoked.</span></span>|





