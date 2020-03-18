---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 445d3fb20bcd159979694093eac0b03f6a876072
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42796045"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="b2709-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b2709-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="b2709-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b2709-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b2709-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b2709-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b2709-106">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="b2709-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="b2709-107">成员</span><span class="sxs-lookup"><span data-stu-id="b2709-107">Members</span></span>
|<span data-ttu-id="b2709-108">成员</span><span class="sxs-lookup"><span data-stu-id="b2709-108">Member</span></span>|<span data-ttu-id="b2709-109">值</span><span class="sxs-lookup"><span data-stu-id="b2709-109">Value</span></span>|<span data-ttu-id="b2709-110">说明</span><span class="sxs-lookup"><span data-stu-id="b2709-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b2709-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b2709-111">notConfigured</span></span>|<span data-ttu-id="b2709-112">0</span><span class="sxs-lookup"><span data-stu-id="b2709-112">0</span></span>|<span data-ttu-id="b2709-113">未配置</span><span class="sxs-lookup"><span data-stu-id="b2709-113">Not Configured</span></span>|
|<span data-ttu-id="b2709-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="b2709-114">blockBoth</span></span>|<span data-ttu-id="b2709-115">1</span><span class="sxs-lookup"><span data-stu-id="b2709-115">1</span></span>|<span data-ttu-id="b2709-116">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="b2709-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="b2709-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="b2709-117">blockHostToContainer</span></span>|<span data-ttu-id="b2709-118">双面</span><span class="sxs-lookup"><span data-stu-id="b2709-118">2</span></span>|<span data-ttu-id="b2709-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="b2709-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="b2709-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="b2709-120">blockContainerToHost</span></span>|<span data-ttu-id="b2709-121">第三章</span><span class="sxs-lookup"><span data-stu-id="b2709-121">3</span></span>|<span data-ttu-id="b2709-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="b2709-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="b2709-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="b2709-123">blockNone</span></span>|<span data-ttu-id="b2709-124">4 </span><span class="sxs-lookup"><span data-stu-id="b2709-124">4</span></span>|<span data-ttu-id="b2709-125">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="b2709-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



