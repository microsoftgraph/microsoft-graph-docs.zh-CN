---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
ms.openlocfilehash: af1843a8d7515e5ca14997256968942f485eab64
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27304079"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="fd31e-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fd31e-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="fd31e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fd31e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd31e-105">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="fd31e-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="fd31e-106">成员</span><span class="sxs-lookup"><span data-stu-id="fd31e-106">Members</span></span>
|<span data-ttu-id="fd31e-107">成员</span><span class="sxs-lookup"><span data-stu-id="fd31e-107">Member</span></span>|<span data-ttu-id="fd31e-108">值</span><span class="sxs-lookup"><span data-stu-id="fd31e-108">Value</span></span>|<span data-ttu-id="fd31e-109">说明</span><span class="sxs-lookup"><span data-stu-id="fd31e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd31e-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="fd31e-110">notConfigured</span></span>|<span data-ttu-id="fd31e-111">0</span><span class="sxs-lookup"><span data-stu-id="fd31e-111">0</span></span>|<span data-ttu-id="fd31e-112">未配置</span><span class="sxs-lookup"><span data-stu-id="fd31e-112">Not Configured</span></span>|
|<span data-ttu-id="fd31e-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="fd31e-113">blockBoth</span></span>|<span data-ttu-id="fd31e-114">1</span><span class="sxs-lookup"><span data-stu-id="fd31e-114">1</span></span>|<span data-ttu-id="fd31e-115">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="fd31e-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="fd31e-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="fd31e-116">blockHostToContainer</span></span>|<span data-ttu-id="fd31e-117">2</span><span class="sxs-lookup"><span data-stu-id="fd31e-117">2</span></span>|<span data-ttu-id="fd31e-118">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="fd31e-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="fd31e-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="fd31e-119">blockContainerToHost</span></span>|<span data-ttu-id="fd31e-120">3</span><span class="sxs-lookup"><span data-stu-id="fd31e-120">3</span></span>|<span data-ttu-id="fd31e-121">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="fd31e-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="fd31e-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="fd31e-122">blockNone</span></span>|<span data-ttu-id="fd31e-123">4</span><span class="sxs-lookup"><span data-stu-id="fd31e-123">4</span></span>|<span data-ttu-id="fd31e-124">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="fd31e-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



