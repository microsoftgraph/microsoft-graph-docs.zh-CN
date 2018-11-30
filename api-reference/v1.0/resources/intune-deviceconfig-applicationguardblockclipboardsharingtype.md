---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
ms.openlocfilehash: 59d325612430a184feaf7df655a4da660b65ea78
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008947"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="e1735-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1735-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="e1735-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e1735-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1735-105">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="e1735-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="e1735-106">成员</span><span class="sxs-lookup"><span data-stu-id="e1735-106">Members</span></span>
|<span data-ttu-id="e1735-107">成员</span><span class="sxs-lookup"><span data-stu-id="e1735-107">Member</span></span>|<span data-ttu-id="e1735-108">值</span><span class="sxs-lookup"><span data-stu-id="e1735-108">Value</span></span>|<span data-ttu-id="e1735-109">说明</span><span class="sxs-lookup"><span data-stu-id="e1735-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1735-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="e1735-110">notConfigured</span></span>|<span data-ttu-id="e1735-111">0</span><span class="sxs-lookup"><span data-stu-id="e1735-111">0</span></span>|<span data-ttu-id="e1735-112">未配置</span><span class="sxs-lookup"><span data-stu-id="e1735-112">Not Configured</span></span>|
|<span data-ttu-id="e1735-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="e1735-113">blockBoth</span></span>|<span data-ttu-id="e1735-114">1</span><span class="sxs-lookup"><span data-stu-id="e1735-114">1</span></span>|<span data-ttu-id="e1735-115">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="e1735-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="e1735-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="e1735-116">blockHostToContainer</span></span>|<span data-ttu-id="e1735-117">2</span><span class="sxs-lookup"><span data-stu-id="e1735-117">2</span></span>|<span data-ttu-id="e1735-118">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="e1735-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="e1735-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="e1735-119">blockContainerToHost</span></span>|<span data-ttu-id="e1735-120">3</span><span class="sxs-lookup"><span data-stu-id="e1735-120">3</span></span>|<span data-ttu-id="e1735-121">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="e1735-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="e1735-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="e1735-122">blockNone</span></span>|<span data-ttu-id="e1735-123">4</span><span class="sxs-lookup"><span data-stu-id="e1735-123">4</span></span>|<span data-ttu-id="e1735-124">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="e1735-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



