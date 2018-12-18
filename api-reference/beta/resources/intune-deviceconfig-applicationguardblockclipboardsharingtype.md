---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
ms.openlocfilehash: d55945c0e229801bab9a338a475e6ef6fd5e8b02
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311506"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="e9921-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e9921-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="e9921-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e9921-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e9921-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e9921-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9921-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e9921-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9921-107">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="e9921-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="e9921-108">成员</span><span class="sxs-lookup"><span data-stu-id="e9921-108">Members</span></span>
|<span data-ttu-id="e9921-109">成员</span><span class="sxs-lookup"><span data-stu-id="e9921-109">Member</span></span>|<span data-ttu-id="e9921-110">值</span><span class="sxs-lookup"><span data-stu-id="e9921-110">Value</span></span>|<span data-ttu-id="e9921-111">说明</span><span class="sxs-lookup"><span data-stu-id="e9921-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9921-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e9921-112">notConfigured</span></span>|<span data-ttu-id="e9921-113">0</span><span class="sxs-lookup"><span data-stu-id="e9921-113">0</span></span>|<span data-ttu-id="e9921-114">未配置</span><span class="sxs-lookup"><span data-stu-id="e9921-114">Not Configured</span></span>|
|<span data-ttu-id="e9921-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="e9921-115">blockBoth</span></span>|<span data-ttu-id="e9921-116">1</span><span class="sxs-lookup"><span data-stu-id="e9921-116">1</span></span>|<span data-ttu-id="e9921-117">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="e9921-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="e9921-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="e9921-118">blockHostToContainer</span></span>|<span data-ttu-id="e9921-119">2</span><span class="sxs-lookup"><span data-stu-id="e9921-119">2</span></span>|<span data-ttu-id="e9921-120">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="e9921-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="e9921-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="e9921-121">blockContainerToHost</span></span>|<span data-ttu-id="e9921-122">3</span><span class="sxs-lookup"><span data-stu-id="e9921-122">3</span></span>|<span data-ttu-id="e9921-123">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="e9921-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="e9921-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="e9921-124">blockNone</span></span>|<span data-ttu-id="e9921-125">4</span><span class="sxs-lookup"><span data-stu-id="e9921-125">4</span></span>|<span data-ttu-id="e9921-126">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="e9921-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





