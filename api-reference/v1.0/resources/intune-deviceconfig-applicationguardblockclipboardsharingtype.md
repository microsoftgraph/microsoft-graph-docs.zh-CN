---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6fe418aa1f91c0e65770b797781dda9e29803d86
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865973"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="43ceb-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="43ceb-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="43ceb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="43ceb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="43ceb-105">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="43ceb-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="43ceb-106">成员</span><span class="sxs-lookup"><span data-stu-id="43ceb-106">Members</span></span>
|<span data-ttu-id="43ceb-107">成员</span><span class="sxs-lookup"><span data-stu-id="43ceb-107">Member</span></span>|<span data-ttu-id="43ceb-108">值</span><span class="sxs-lookup"><span data-stu-id="43ceb-108">Value</span></span>|<span data-ttu-id="43ceb-109">Description</span><span class="sxs-lookup"><span data-stu-id="43ceb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43ceb-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="43ceb-110">notConfigured</span></span>|<span data-ttu-id="43ceb-111">0</span><span class="sxs-lookup"><span data-stu-id="43ceb-111">0</span></span>|<span data-ttu-id="43ceb-112">未配置</span><span class="sxs-lookup"><span data-stu-id="43ceb-112">Not Configured</span></span>|
|<span data-ttu-id="43ceb-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="43ceb-113">blockBoth</span></span>|<span data-ttu-id="43ceb-114">1</span><span class="sxs-lookup"><span data-stu-id="43ceb-114">1</span></span>|<span data-ttu-id="43ceb-115">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="43ceb-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="43ceb-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="43ceb-116">blockHostToContainer</span></span>|<span data-ttu-id="43ceb-117">2</span><span class="sxs-lookup"><span data-stu-id="43ceb-117">2</span></span>|<span data-ttu-id="43ceb-118">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="43ceb-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="43ceb-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="43ceb-119">blockContainerToHost</span></span>|<span data-ttu-id="43ceb-120">3</span><span class="sxs-lookup"><span data-stu-id="43ceb-120">3</span></span>|<span data-ttu-id="43ceb-121">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="43ceb-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="43ceb-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="43ceb-122">blockNone</span></span>|<span data-ttu-id="43ceb-123">4</span><span class="sxs-lookup"><span data-stu-id="43ceb-123">4</span></span>|<span data-ttu-id="43ceb-124">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="43ceb-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



