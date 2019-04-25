---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: applicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3d1b5132773bb0bf92f35c39b660726d7a1ef66
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575077"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="950bc-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="950bc-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="950bc-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="950bc-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="950bc-105">applicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="950bc-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="950bc-106">成员</span><span class="sxs-lookup"><span data-stu-id="950bc-106">Members</span></span>
|<span data-ttu-id="950bc-107">成员</span><span class="sxs-lookup"><span data-stu-id="950bc-107">Member</span></span>|<span data-ttu-id="950bc-108">值</span><span class="sxs-lookup"><span data-stu-id="950bc-108">Value</span></span>|<span data-ttu-id="950bc-109">说明</span><span class="sxs-lookup"><span data-stu-id="950bc-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="950bc-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="950bc-110">notConfigured</span></span>|<span data-ttu-id="950bc-111">0</span><span class="sxs-lookup"><span data-stu-id="950bc-111">0</span></span>|<span data-ttu-id="950bc-112">未配置</span><span class="sxs-lookup"><span data-stu-id="950bc-112">Not Configured</span></span>|
|<span data-ttu-id="950bc-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="950bc-113">blockBoth</span></span>|<span data-ttu-id="950bc-114">1</span><span class="sxs-lookup"><span data-stu-id="950bc-114">1</span></span>|<span data-ttu-id="950bc-115">阻止剪贴板将数据从主机共享到容器, 并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="950bc-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="950bc-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="950bc-116">blockHostToContainer</span></span>|<span data-ttu-id="950bc-117">2 </span><span class="sxs-lookup"><span data-stu-id="950bc-117">2</span></span>|<span data-ttu-id="950bc-118">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="950bc-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="950bc-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="950bc-119">blockContainerToHost</span></span>|<span data-ttu-id="950bc-120">3 </span><span class="sxs-lookup"><span data-stu-id="950bc-120">3</span></span>|<span data-ttu-id="950bc-121">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="950bc-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="950bc-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="950bc-122">blockNone</span></span>|<span data-ttu-id="950bc-123">4 </span><span class="sxs-lookup"><span data-stu-id="950bc-123">4</span></span>|<span data-ttu-id="950bc-124">阻止剪贴板将数据从主机共享到容器, 也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="950bc-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



