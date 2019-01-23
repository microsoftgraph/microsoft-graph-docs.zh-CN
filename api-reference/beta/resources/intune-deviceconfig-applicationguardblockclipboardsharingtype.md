---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3f9621db53e16231f710cccb12d79f65d22d4017
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415059"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="8102a-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8102a-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="8102a-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="8102a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8102a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8102a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8102a-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8102a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8102a-107">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="8102a-107">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="8102a-108">成员</span><span class="sxs-lookup"><span data-stu-id="8102a-108">Members</span></span>
|<span data-ttu-id="8102a-109">成员</span><span class="sxs-lookup"><span data-stu-id="8102a-109">Member</span></span>|<span data-ttu-id="8102a-110">值</span><span class="sxs-lookup"><span data-stu-id="8102a-110">Value</span></span>|<span data-ttu-id="8102a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8102a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8102a-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="8102a-112">notConfigured</span></span>|<span data-ttu-id="8102a-113">0</span><span class="sxs-lookup"><span data-stu-id="8102a-113">0</span></span>|<span data-ttu-id="8102a-114">未配置</span><span class="sxs-lookup"><span data-stu-id="8102a-114">Not Configured</span></span>|
|<span data-ttu-id="8102a-115">blockBoth</span><span class="sxs-lookup"><span data-stu-id="8102a-115">blockBoth</span></span>|<span data-ttu-id="8102a-116">1</span><span class="sxs-lookup"><span data-stu-id="8102a-116">1</span></span>|<span data-ttu-id="8102a-117">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="8102a-117">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="8102a-118">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="8102a-118">blockHostToContainer</span></span>|<span data-ttu-id="8102a-119">2</span><span class="sxs-lookup"><span data-stu-id="8102a-119">2</span></span>|<span data-ttu-id="8102a-120">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="8102a-120">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="8102a-121">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="8102a-121">blockContainerToHost</span></span>|<span data-ttu-id="8102a-122">3</span><span class="sxs-lookup"><span data-stu-id="8102a-122">3</span></span>|<span data-ttu-id="8102a-123">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="8102a-123">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="8102a-124">blockNone</span><span class="sxs-lookup"><span data-stu-id="8102a-124">blockNone</span></span>|<span data-ttu-id="8102a-125">4</span><span class="sxs-lookup"><span data-stu-id="8102a-125">4</span></span>|<span data-ttu-id="8102a-126">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="8102a-126">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




