---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: ebf56c4dc7e31a4c6a70e808c6f7f35aaaf9181d
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43470018"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="bb571-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bb571-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="bb571-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bb571-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bb571-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bb571-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bb571-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bb571-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bb571-107">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="bb571-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="bb571-108">成员</span><span class="sxs-lookup"><span data-stu-id="bb571-108">Members</span></span>
|<span data-ttu-id="bb571-109">成员</span><span class="sxs-lookup"><span data-stu-id="bb571-109">Member</span></span>|<span data-ttu-id="bb571-110">值</span><span class="sxs-lookup"><span data-stu-id="bb571-110">Value</span></span>|<span data-ttu-id="bb571-111">说明</span><span class="sxs-lookup"><span data-stu-id="bb571-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bb571-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="bb571-112">notConfigured</span></span>|<span data-ttu-id="bb571-113">0</span><span class="sxs-lookup"><span data-stu-id="bb571-113">0</span></span>|<span data-ttu-id="bb571-114">未配置</span><span class="sxs-lookup"><span data-stu-id="bb571-114">Not Configured</span></span>|
|<span data-ttu-id="bb571-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="bb571-115">blockBoth</span></span>|<span data-ttu-id="bb571-116">1</span><span class="sxs-lookup"><span data-stu-id="bb571-116">1</span></span>|<span data-ttu-id="bb571-117">阻止剪贴板将数据从主机共享到容器，并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="bb571-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="bb571-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="bb571-118">blockHostToContainer</span></span>|<span data-ttu-id="bb571-119">双面</span><span class="sxs-lookup"><span data-stu-id="bb571-119">2</span></span>|<span data-ttu-id="bb571-120">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="bb571-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="bb571-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="bb571-121">blockContainerToHost</span></span>|<span data-ttu-id="bb571-122">第三章</span><span class="sxs-lookup"><span data-stu-id="bb571-122">3</span></span>|<span data-ttu-id="bb571-123">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="bb571-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="bb571-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="bb571-124">blockNone</span></span>|<span data-ttu-id="bb571-125">4 </span><span class="sxs-lookup"><span data-stu-id="bb571-125">4</span></span>|<span data-ttu-id="bb571-126">阻止剪贴板将数据从主机共享到容器，也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="bb571-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



