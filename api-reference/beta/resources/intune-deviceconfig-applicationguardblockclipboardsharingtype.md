---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: applicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 83a0adf84ea57e6afa1749d1f6f7152403847b5f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562298"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="aad3a-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aad3a-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="aad3a-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="aad3a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aad3a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aad3a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aad3a-106">applicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="aad3a-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="aad3a-107">成员</span><span class="sxs-lookup"><span data-stu-id="aad3a-107">Members</span></span>
|<span data-ttu-id="aad3a-108">成员</span><span class="sxs-lookup"><span data-stu-id="aad3a-108">Member</span></span>|<span data-ttu-id="aad3a-109">值</span><span class="sxs-lookup"><span data-stu-id="aad3a-109">Value</span></span>|<span data-ttu-id="aad3a-110">说明</span><span class="sxs-lookup"><span data-stu-id="aad3a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aad3a-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="aad3a-111">notConfigured</span></span>|<span data-ttu-id="aad3a-112">0</span><span class="sxs-lookup"><span data-stu-id="aad3a-112">0</span></span>|<span data-ttu-id="aad3a-113">未配置</span><span class="sxs-lookup"><span data-stu-id="aad3a-113">Not Configured</span></span>|
|<span data-ttu-id="aad3a-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="aad3a-114">blockBoth</span></span>|<span data-ttu-id="aad3a-115">1</span><span class="sxs-lookup"><span data-stu-id="aad3a-115">1</span></span>|<span data-ttu-id="aad3a-116">阻止剪贴板将数据从主机共享到容器, 并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="aad3a-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="aad3a-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="aad3a-117">blockHostToContainer</span></span>|<span data-ttu-id="aad3a-118">2 </span><span class="sxs-lookup"><span data-stu-id="aad3a-118">2</span></span>|<span data-ttu-id="aad3a-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="aad3a-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="aad3a-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="aad3a-120">blockContainerToHost</span></span>|<span data-ttu-id="aad3a-121">3 </span><span class="sxs-lookup"><span data-stu-id="aad3a-121">3</span></span>|<span data-ttu-id="aad3a-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="aad3a-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="aad3a-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="aad3a-123">blockNone</span></span>|<span data-ttu-id="aad3a-124">4 </span><span class="sxs-lookup"><span data-stu-id="aad3a-124">4</span></span>|<span data-ttu-id="aad3a-125">阻止剪贴板将数据从主机共享到容器, 也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="aad3a-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





