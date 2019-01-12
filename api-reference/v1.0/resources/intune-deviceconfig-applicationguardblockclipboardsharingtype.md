---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7dacce6dbe91a2bbc76b52795bc20de4cf0e5f71
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27911880"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="caea6-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="caea6-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="caea6-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="caea6-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="caea6-105">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="caea6-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>
## <a name="members"></a><span data-ttu-id="caea6-106">成员</span><span class="sxs-lookup"><span data-stu-id="caea6-106">Members</span></span>
|<span data-ttu-id="caea6-107">成员</span><span class="sxs-lookup"><span data-stu-id="caea6-107">Member</span></span>|<span data-ttu-id="caea6-108">值</span><span class="sxs-lookup"><span data-stu-id="caea6-108">Value</span></span>|<span data-ttu-id="caea6-109">说明</span><span class="sxs-lookup"><span data-stu-id="caea6-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="caea6-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="caea6-110">notConfigured</span></span>|<span data-ttu-id="caea6-111">0</span><span class="sxs-lookup"><span data-stu-id="caea6-111">0</span></span>|<span data-ttu-id="caea6-112">未配置</span><span class="sxs-lookup"><span data-stu-id="caea6-112">Not Configured</span></span>|
|<span data-ttu-id="caea6-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="caea6-113">blockBoth</span></span>|<span data-ttu-id="caea6-114">1</span><span class="sxs-lookup"><span data-stu-id="caea6-114">1</span></span>|<span data-ttu-id="caea6-115">阻止剪贴板共享数据从主机到容器和容器迁移到主机</span><span class="sxs-lookup"><span data-stu-id="caea6-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="caea6-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="caea6-116">blockHostToContainer</span></span>|<span data-ttu-id="caea6-117">2</span><span class="sxs-lookup"><span data-stu-id="caea6-117">2</span></span>|<span data-ttu-id="caea6-118">阻止剪贴板共享数据从主机到容器</span><span class="sxs-lookup"><span data-stu-id="caea6-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="caea6-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="caea6-119">blockContainerToHost</span></span>|<span data-ttu-id="caea6-120">3</span><span class="sxs-lookup"><span data-stu-id="caea6-120">3</span></span>|<span data-ttu-id="caea6-121">阻止剪贴板共享数据从容器到主机</span><span class="sxs-lookup"><span data-stu-id="caea6-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="caea6-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="caea6-122">blockNone</span></span>|<span data-ttu-id="caea6-123">4</span><span class="sxs-lookup"><span data-stu-id="caea6-123">4</span></span>|<span data-ttu-id="caea6-124">共享数据从主机到容器和从容器迁移到主机都不阻止剪贴板</span><span class="sxs-lookup"><span data-stu-id="caea6-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



