---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 89cfe40f949cf8daa5c7e2f68fa41366a498a31a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530937"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="aebe5-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="aebe5-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="aebe5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aebe5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aebe5-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aebe5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aebe5-106">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="aebe5-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="aebe5-107">成员</span><span class="sxs-lookup"><span data-stu-id="aebe5-107">Members</span></span>
|<span data-ttu-id="aebe5-108">成员</span><span class="sxs-lookup"><span data-stu-id="aebe5-108">Member</span></span>|<span data-ttu-id="aebe5-109">值</span><span class="sxs-lookup"><span data-stu-id="aebe5-109">Value</span></span>|<span data-ttu-id="aebe5-110">说明</span><span class="sxs-lookup"><span data-stu-id="aebe5-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aebe5-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="aebe5-111">notConfigured</span></span>|<span data-ttu-id="aebe5-112">0</span><span class="sxs-lookup"><span data-stu-id="aebe5-112">0</span></span>|<span data-ttu-id="aebe5-113">未配置</span><span class="sxs-lookup"><span data-stu-id="aebe5-113">Not Configured</span></span>|
|<span data-ttu-id="aebe5-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="aebe5-114">blockBoth</span></span>|<span data-ttu-id="aebe5-115">1 </span><span class="sxs-lookup"><span data-stu-id="aebe5-115">1</span></span>|<span data-ttu-id="aebe5-116">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="aebe5-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="aebe5-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="aebe5-117">blockHostToContainer</span></span>|<span data-ttu-id="aebe5-118">2 </span><span class="sxs-lookup"><span data-stu-id="aebe5-118">2</span></span>|<span data-ttu-id="aebe5-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="aebe5-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="aebe5-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="aebe5-120">blockContainerToHost</span></span>|<span data-ttu-id="aebe5-121">3 </span><span class="sxs-lookup"><span data-stu-id="aebe5-121">3</span></span>|<span data-ttu-id="aebe5-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="aebe5-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="aebe5-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="aebe5-123">blockNone</span></span>|<span data-ttu-id="aebe5-124">4 </span><span class="sxs-lookup"><span data-stu-id="aebe5-124">4</span></span>|<span data-ttu-id="aebe5-125">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="aebe5-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




