---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 5e4ea44dfc5a0a5425b587b95d1a932c0af528f7
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48075943"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="b1f90-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1f90-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="b1f90-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1f90-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b1f90-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b1f90-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b1f90-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1f90-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1f90-107">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="b1f90-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="b1f90-108">成员</span><span class="sxs-lookup"><span data-stu-id="b1f90-108">Members</span></span>
|<span data-ttu-id="b1f90-109">成员</span><span class="sxs-lookup"><span data-stu-id="b1f90-109">Member</span></span>|<span data-ttu-id="b1f90-110">值</span><span class="sxs-lookup"><span data-stu-id="b1f90-110">Value</span></span>|<span data-ttu-id="b1f90-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1f90-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1f90-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b1f90-112">notConfigured</span></span>|<span data-ttu-id="b1f90-113">0</span><span class="sxs-lookup"><span data-stu-id="b1f90-113">0</span></span>|<span data-ttu-id="b1f90-114">未配置</span><span class="sxs-lookup"><span data-stu-id="b1f90-114">Not Configured</span></span>|
|<span data-ttu-id="b1f90-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="b1f90-115">blockBoth</span></span>|<span data-ttu-id="b1f90-116">1 </span><span class="sxs-lookup"><span data-stu-id="b1f90-116">1</span></span>|<span data-ttu-id="b1f90-117">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="b1f90-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="b1f90-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="b1f90-118">blockHostToContainer</span></span>|<span data-ttu-id="b1f90-119">2 </span><span class="sxs-lookup"><span data-stu-id="b1f90-119">2</span></span>|<span data-ttu-id="b1f90-120">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="b1f90-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="b1f90-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="b1f90-121">blockContainerToHost</span></span>|<span data-ttu-id="b1f90-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b1f90-122">3</span></span>|<span data-ttu-id="b1f90-123">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="b1f90-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="b1f90-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="b1f90-124">blockNone</span></span>|<span data-ttu-id="b1f90-125">4 </span><span class="sxs-lookup"><span data-stu-id="b1f90-125">4</span></span>|<span data-ttu-id="b1f90-126">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="b1f90-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|






