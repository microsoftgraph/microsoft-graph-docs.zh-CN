---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 51f259fbd201869de2c69a019fa17f674fd095c2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48051170"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="9f720-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9f720-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="9f720-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f720-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9f720-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9f720-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9f720-106">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="9f720-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="9f720-107">成员</span><span class="sxs-lookup"><span data-stu-id="9f720-107">Members</span></span>
|<span data-ttu-id="9f720-108">成员</span><span class="sxs-lookup"><span data-stu-id="9f720-108">Member</span></span>|<span data-ttu-id="9f720-109">值</span><span class="sxs-lookup"><span data-stu-id="9f720-109">Value</span></span>|<span data-ttu-id="9f720-110">说明</span><span class="sxs-lookup"><span data-stu-id="9f720-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f720-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9f720-111">notConfigured</span></span>|<span data-ttu-id="9f720-112">0</span><span class="sxs-lookup"><span data-stu-id="9f720-112">0</span></span>|<span data-ttu-id="9f720-113">未配置</span><span class="sxs-lookup"><span data-stu-id="9f720-113">Not Configured</span></span>|
|<span data-ttu-id="9f720-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="9f720-114">blockBoth</span></span>|<span data-ttu-id="9f720-115">1 </span><span class="sxs-lookup"><span data-stu-id="9f720-115">1</span></span>|<span data-ttu-id="9f720-116">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="9f720-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="9f720-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="9f720-117">blockHostToContainer</span></span>|<span data-ttu-id="9f720-118">2 </span><span class="sxs-lookup"><span data-stu-id="9f720-118">2</span></span>|<span data-ttu-id="9f720-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="9f720-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="9f720-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="9f720-120">blockContainerToHost</span></span>|<span data-ttu-id="9f720-121">第三章</span><span class="sxs-lookup"><span data-stu-id="9f720-121">3</span></span>|<span data-ttu-id="9f720-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="9f720-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="9f720-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="9f720-123">blockNone</span></span>|<span data-ttu-id="9f720-124">4 </span><span class="sxs-lookup"><span data-stu-id="9f720-124">4</span></span>|<span data-ttu-id="9f720-125">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="9f720-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|









