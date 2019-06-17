---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 565980a570b0334cac02e2bc4646d0b70298b4fc
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987605"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="862f6-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="862f6-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="862f6-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="862f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="862f6-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="862f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="862f6-106">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="862f6-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="862f6-107">成员</span><span class="sxs-lookup"><span data-stu-id="862f6-107">Members</span></span>
|<span data-ttu-id="862f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="862f6-108">Member</span></span>|<span data-ttu-id="862f6-109">值</span><span class="sxs-lookup"><span data-stu-id="862f6-109">Value</span></span>|<span data-ttu-id="862f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="862f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="862f6-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="862f6-111">notConfigured</span></span>|<span data-ttu-id="862f6-112">0</span><span class="sxs-lookup"><span data-stu-id="862f6-112">0</span></span>|<span data-ttu-id="862f6-113">未配置</span><span class="sxs-lookup"><span data-stu-id="862f6-113">Not Configured</span></span>|
|<span data-ttu-id="862f6-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="862f6-114">blockBoth</span></span>|<span data-ttu-id="862f6-115">1</span><span class="sxs-lookup"><span data-stu-id="862f6-115">1</span></span>|<span data-ttu-id="862f6-116">阻止剪贴板将数据从主机共享到容器, 并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="862f6-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="862f6-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="862f6-117">blockHostToContainer</span></span>|<span data-ttu-id="862f6-118">双面</span><span class="sxs-lookup"><span data-stu-id="862f6-118">2</span></span>|<span data-ttu-id="862f6-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="862f6-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="862f6-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="862f6-120">blockContainerToHost</span></span>|<span data-ttu-id="862f6-121">第三章</span><span class="sxs-lookup"><span data-stu-id="862f6-121">3</span></span>|<span data-ttu-id="862f6-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="862f6-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="862f6-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="862f6-123">blockNone</span></span>|<span data-ttu-id="862f6-124">4</span><span class="sxs-lookup"><span data-stu-id="862f6-124">4</span></span>|<span data-ttu-id="862f6-125">阻止剪贴板将数据从主机共享到容器, 也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="862f6-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





