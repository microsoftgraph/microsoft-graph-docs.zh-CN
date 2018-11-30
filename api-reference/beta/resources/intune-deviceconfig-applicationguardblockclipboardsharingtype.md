---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
ms.openlocfilehash: e0e05001e4f3cedc2893fc6b2006f5b5b5d74db6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045892"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="49e5a-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="49e5a-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="49e5a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="49e5a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="49e5a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="49e5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="49e5a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="49e5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="49e5a-107">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="49e5a-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="49e5a-108">成员</span><span class="sxs-lookup"><span data-stu-id="49e5a-108">Members</span></span>
|<span data-ttu-id="49e5a-109">成员</span><span class="sxs-lookup"><span data-stu-id="49e5a-109">Member</span></span>|<span data-ttu-id="49e5a-110">值</span><span class="sxs-lookup"><span data-stu-id="49e5a-110">Value</span></span>|<span data-ttu-id="49e5a-111">说明</span><span class="sxs-lookup"><span data-stu-id="49e5a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49e5a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="49e5a-112">notConfigured</span></span>|<span data-ttu-id="49e5a-113">0</span><span class="sxs-lookup"><span data-stu-id="49e5a-113">0</span></span>|<span data-ttu-id="49e5a-114">未配置</span><span class="sxs-lookup"><span data-stu-id="49e5a-114">Not Configured</span></span>|
|<span data-ttu-id="49e5a-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="49e5a-115">blockBoth</span></span>|<span data-ttu-id="49e5a-116">1</span><span class="sxs-lookup"><span data-stu-id="49e5a-116">1</span></span>|<span data-ttu-id="49e5a-117">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="49e5a-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="49e5a-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="49e5a-118">blockHostToContainer</span></span>|<span data-ttu-id="49e5a-119">2</span><span class="sxs-lookup"><span data-stu-id="49e5a-119">2</span></span>|<span data-ttu-id="49e5a-120">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="49e5a-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="49e5a-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="49e5a-121">blockContainerToHost</span></span>|<span data-ttu-id="49e5a-122">3</span><span class="sxs-lookup"><span data-stu-id="49e5a-122">3</span></span>|<span data-ttu-id="49e5a-123">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="49e5a-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="49e5a-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="49e5a-124">blockNone</span></span>|<span data-ttu-id="49e5a-125">4</span><span class="sxs-lookup"><span data-stu-id="49e5a-125">4</span></span>|<span data-ttu-id="49e5a-126">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="49e5a-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|





