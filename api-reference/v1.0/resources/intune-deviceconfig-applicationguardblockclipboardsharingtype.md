---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b2046626b308fc4322f7947c5bfc3d8fabbbbee9
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449219"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="5bdaf-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5bdaf-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="5bdaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5bdaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5bdaf-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5bdaf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bdaf-106">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="5bdaf-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="5bdaf-107">成员</span><span class="sxs-lookup"><span data-stu-id="5bdaf-107">Members</span></span>
|<span data-ttu-id="5bdaf-108">成员</span><span class="sxs-lookup"><span data-stu-id="5bdaf-108">Member</span></span>|<span data-ttu-id="5bdaf-109">值</span><span class="sxs-lookup"><span data-stu-id="5bdaf-109">Value</span></span>|<span data-ttu-id="5bdaf-110">说明</span><span class="sxs-lookup"><span data-stu-id="5bdaf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5bdaf-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="5bdaf-111">notConfigured</span></span>|<span data-ttu-id="5bdaf-112">0</span><span class="sxs-lookup"><span data-stu-id="5bdaf-112">0</span></span>|<span data-ttu-id="5bdaf-113">未配置</span><span class="sxs-lookup"><span data-stu-id="5bdaf-113">Not Configured</span></span>|
|<span data-ttu-id="5bdaf-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="5bdaf-114">blockBoth</span></span>|<span data-ttu-id="5bdaf-115">1</span><span class="sxs-lookup"><span data-stu-id="5bdaf-115">1</span></span>|<span data-ttu-id="5bdaf-116">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="5bdaf-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="5bdaf-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="5bdaf-117">blockHostToContainer</span></span>|<span data-ttu-id="5bdaf-118">双面</span><span class="sxs-lookup"><span data-stu-id="5bdaf-118">2</span></span>|<span data-ttu-id="5bdaf-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="5bdaf-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="5bdaf-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="5bdaf-120">blockContainerToHost</span></span>|<span data-ttu-id="5bdaf-121">第三章</span><span class="sxs-lookup"><span data-stu-id="5bdaf-121">3</span></span>|<span data-ttu-id="5bdaf-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="5bdaf-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="5bdaf-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="5bdaf-123">blockNone</span></span>|<span data-ttu-id="5bdaf-124">4 </span><span class="sxs-lookup"><span data-stu-id="5bdaf-124">4</span></span>|<span data-ttu-id="5bdaf-125">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="5bdaf-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|







