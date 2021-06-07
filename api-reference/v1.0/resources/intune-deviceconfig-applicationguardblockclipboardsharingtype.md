---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: applicationGuardBlockClipboardSharingType 的可能值
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: a70f654c283a32db4e89ccc1b3991ffba49fc89e
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755936"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="479f7-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="479f7-103">applicationGuardBlockClipboardSharingType enum type</span></span>

<span data-ttu-id="479f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="479f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="479f7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="479f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="479f7-106">applicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="479f7-106">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="479f7-107">成员</span><span class="sxs-lookup"><span data-stu-id="479f7-107">Members</span></span>
|<span data-ttu-id="479f7-108">成员</span><span class="sxs-lookup"><span data-stu-id="479f7-108">Member</span></span>|<span data-ttu-id="479f7-109">值</span><span class="sxs-lookup"><span data-stu-id="479f7-109">Value</span></span>|<span data-ttu-id="479f7-110">Description</span><span class="sxs-lookup"><span data-stu-id="479f7-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="479f7-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="479f7-111">notConfigured</span></span>|<span data-ttu-id="479f7-112">0</span><span class="sxs-lookup"><span data-stu-id="479f7-112">0</span></span>|<span data-ttu-id="479f7-113">未配置</span><span class="sxs-lookup"><span data-stu-id="479f7-113">Not Configured</span></span>|
|<span data-ttu-id="479f7-114">blockBoth</span><span class="sxs-lookup"><span data-stu-id="479f7-114">blockBoth</span></span>|<span data-ttu-id="479f7-115">1</span><span class="sxs-lookup"><span data-stu-id="479f7-115">1</span></span>|<span data-ttu-id="479f7-116">阻止剪贴板从主机共享到容器以及从容器共享数据到主机</span><span class="sxs-lookup"><span data-stu-id="479f7-116">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="479f7-117">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="479f7-117">blockHostToContainer</span></span>|<span data-ttu-id="479f7-118">2</span><span class="sxs-lookup"><span data-stu-id="479f7-118">2</span></span>|<span data-ttu-id="479f7-119">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="479f7-119">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="479f7-120">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="479f7-120">blockContainerToHost</span></span>|<span data-ttu-id="479f7-121">3</span><span class="sxs-lookup"><span data-stu-id="479f7-121">3</span></span>|<span data-ttu-id="479f7-122">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="479f7-122">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="479f7-123">blockNone</span><span class="sxs-lookup"><span data-stu-id="479f7-123">blockNone</span></span>|<span data-ttu-id="479f7-124">4 </span><span class="sxs-lookup"><span data-stu-id="479f7-124">4</span></span>|<span data-ttu-id="479f7-125">阻止剪贴板从主机共享到容器，也不从容器共享数据到主机</span><span class="sxs-lookup"><span data-stu-id="479f7-125">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|




