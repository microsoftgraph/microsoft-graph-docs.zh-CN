---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: applicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9dba5ba1a2d27862c9adaaa1430631b8cb4cf94d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30160660"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="f8d43-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f8d43-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="f8d43-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f8d43-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f8d43-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8d43-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8d43-106">applicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="f8d43-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="f8d43-107">成员</span><span class="sxs-lookup"><span data-stu-id="f8d43-107">Members</span></span>
|<span data-ttu-id="f8d43-108">成员</span><span class="sxs-lookup"><span data-stu-id="f8d43-108">Member</span></span>|<span data-ttu-id="f8d43-109">值</span><span class="sxs-lookup"><span data-stu-id="f8d43-109">Value</span></span>|<span data-ttu-id="f8d43-110">说明</span><span class="sxs-lookup"><span data-stu-id="f8d43-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8d43-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f8d43-111">notConfigured</span></span>|<span data-ttu-id="f8d43-112">0</span><span class="sxs-lookup"><span data-stu-id="f8d43-112">0</span></span>|<span data-ttu-id="f8d43-113">未配置</span><span class="sxs-lookup"><span data-stu-id="f8d43-113">Not Configured</span></span>|
|<span data-ttu-id="f8d43-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="f8d43-114">blockBoth</span></span>|<span data-ttu-id="f8d43-115">1</span><span class="sxs-lookup"><span data-stu-id="f8d43-115">1</span></span>|<span data-ttu-id="f8d43-116">阻止剪贴板将数据从主机共享到容器, 并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="f8d43-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="f8d43-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="f8d43-117">blockHostToContainer</span></span>|<span data-ttu-id="f8d43-118">双面</span><span class="sxs-lookup"><span data-stu-id="f8d43-118">2</span></span>|<span data-ttu-id="f8d43-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="f8d43-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="f8d43-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="f8d43-120">blockContainerToHost</span></span>|<span data-ttu-id="f8d43-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f8d43-121">3</span></span>|<span data-ttu-id="f8d43-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="f8d43-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="f8d43-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="f8d43-123">blockNone</span></span>|<span data-ttu-id="f8d43-124">4</span><span class="sxs-lookup"><span data-stu-id="f8d43-124">4</span></span>|<span data-ttu-id="f8d43-125">阻止剪贴板将数据从主机共享到容器, 也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="f8d43-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




