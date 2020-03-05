---
title: secureBootWithDMAType 枚举类型
description: 具有 DMA 的安全引导的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1d1d989d7b39e2db96c3140fca5845230e1984e2
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529419"
---
# <a name="securebootwithdmatype-enum-type"></a><span data-ttu-id="722b3-103">secureBootWithDMAType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="722b3-103">secureBootWithDMAType enum type</span></span>

<span data-ttu-id="722b3-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="722b3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="722b3-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="722b3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="722b3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="722b3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="722b3-107">具有 DMA 的安全引导的可能值</span><span class="sxs-lookup"><span data-stu-id="722b3-107">Possible values of Secure Boot with DMA</span></span>

## <a name="members"></a><span data-ttu-id="722b3-108">成员</span><span class="sxs-lookup"><span data-stu-id="722b3-108">Members</span></span>
|<span data-ttu-id="722b3-109">成员</span><span class="sxs-lookup"><span data-stu-id="722b3-109">Member</span></span>|<span data-ttu-id="722b3-110">值</span><span class="sxs-lookup"><span data-stu-id="722b3-110">Value</span></span>|<span data-ttu-id="722b3-111">说明</span><span class="sxs-lookup"><span data-stu-id="722b3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="722b3-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="722b3-112">notConfigured</span></span>|<span data-ttu-id="722b3-113">0</span><span class="sxs-lookup"><span data-stu-id="722b3-113">0</span></span>|<span data-ttu-id="722b3-114">未配置，无操作</span><span class="sxs-lookup"><span data-stu-id="722b3-114">Not configured, no operation</span></span>|
|<span data-ttu-id="722b3-115">withoutDMA</span><span class="sxs-lookup"><span data-stu-id="722b3-115">withoutDMA</span></span>|<span data-ttu-id="722b3-116">1 </span><span class="sxs-lookup"><span data-stu-id="722b3-116">1</span></span>|<span data-ttu-id="722b3-117">启用安全启动的 VBS</span><span class="sxs-lookup"><span data-stu-id="722b3-117">Turns on VBS with Secure Boot</span></span>|
|<span data-ttu-id="722b3-118">withDMA</span><span class="sxs-lookup"><span data-stu-id="722b3-118">withDMA</span></span>|<span data-ttu-id="722b3-119">3 </span><span class="sxs-lookup"><span data-stu-id="722b3-119">3</span></span>|<span data-ttu-id="722b3-120">启用安全启动和 DMA 的 VBS</span><span class="sxs-lookup"><span data-stu-id="722b3-120">Turns on VBS with Secure Boot and DMA</span></span>|



