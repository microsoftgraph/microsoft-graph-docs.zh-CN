---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 25b429fdd4fdbbb4e5be6a450c814c8fccbbdc54
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366760"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="c3ac8-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c3ac8-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="c3ac8-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3ac8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3ac8-105">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="c3ac8-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="c3ac8-106">成员</span><span class="sxs-lookup"><span data-stu-id="c3ac8-106">Members</span></span>
|<span data-ttu-id="c3ac8-107">成员</span><span class="sxs-lookup"><span data-stu-id="c3ac8-107">Member</span></span>|<span data-ttu-id="c3ac8-108">值</span><span class="sxs-lookup"><span data-stu-id="c3ac8-108">Value</span></span>|<span data-ttu-id="c3ac8-109">说明</span><span class="sxs-lookup"><span data-stu-id="c3ac8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3ac8-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c3ac8-110">notConfigured</span></span>|<span data-ttu-id="c3ac8-111">0</span><span class="sxs-lookup"><span data-stu-id="c3ac8-111">0</span></span>|<span data-ttu-id="c3ac8-112">未配置</span><span class="sxs-lookup"><span data-stu-id="c3ac8-112">Not Configured</span></span>|
|<span data-ttu-id="c3ac8-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="c3ac8-113">blockBoth</span></span>|<span data-ttu-id="c3ac8-114">1</span><span class="sxs-lookup"><span data-stu-id="c3ac8-114">1</span></span>|<span data-ttu-id="c3ac8-115">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="c3ac8-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="c3ac8-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="c3ac8-116">blockHostToContainer</span></span>|<span data-ttu-id="c3ac8-117">双面</span><span class="sxs-lookup"><span data-stu-id="c3ac8-117">2</span></span>|<span data-ttu-id="c3ac8-118">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="c3ac8-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="c3ac8-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="c3ac8-119">blockContainerToHost</span></span>|<span data-ttu-id="c3ac8-120">第三章</span><span class="sxs-lookup"><span data-stu-id="c3ac8-120">3</span></span>|<span data-ttu-id="c3ac8-121">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="c3ac8-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="c3ac8-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="c3ac8-122">blockNone</span></span>|<span data-ttu-id="c3ac8-123">4</span><span class="sxs-lookup"><span data-stu-id="c3ac8-123">4</span></span>|<span data-ttu-id="c3ac8-124">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="c3ac8-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




