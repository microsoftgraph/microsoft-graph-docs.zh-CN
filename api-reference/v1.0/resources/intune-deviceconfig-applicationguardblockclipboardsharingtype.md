---
title: applicationGuardBlockClipboardSharingType 枚举类型
description: ApplicationGuardBlockClipboardSharingType 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a0c6263fe48876ed52e7da81b41975a781cc9636
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36028642"
---
# <a name="applicationguardblockclipboardsharingtype-enum-type"></a><span data-ttu-id="ac4d7-103">applicationGuardBlockClipboardSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ac4d7-103">applicationGuardBlockClipboardSharingType enum type</span></span>

> <span data-ttu-id="ac4d7-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ac4d7-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ac4d7-105">ApplicationGuardBlockClipboardSharingType 的可能值</span><span class="sxs-lookup"><span data-stu-id="ac4d7-105">Possible values for applicationGuardBlockClipboardSharingType</span></span>

## <a name="members"></a><span data-ttu-id="ac4d7-106">成员</span><span class="sxs-lookup"><span data-stu-id="ac4d7-106">Members</span></span>
|<span data-ttu-id="ac4d7-107">成员</span><span class="sxs-lookup"><span data-stu-id="ac4d7-107">Member</span></span>|<span data-ttu-id="ac4d7-108">值</span><span class="sxs-lookup"><span data-stu-id="ac4d7-108">Value</span></span>|<span data-ttu-id="ac4d7-109">说明</span><span class="sxs-lookup"><span data-stu-id="ac4d7-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ac4d7-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ac4d7-110">notConfigured</span></span>|<span data-ttu-id="ac4d7-111">0</span><span class="sxs-lookup"><span data-stu-id="ac4d7-111">0</span></span>|<span data-ttu-id="ac4d7-112">未配置</span><span class="sxs-lookup"><span data-stu-id="ac4d7-112">Not Configured</span></span>|
|<span data-ttu-id="ac4d7-113">blockBoth</span><span class="sxs-lookup"><span data-stu-id="ac4d7-113">blockBoth</span></span>|<span data-ttu-id="ac4d7-114">1</span><span class="sxs-lookup"><span data-stu-id="ac4d7-114">1</span></span>|<span data-ttu-id="ac4d7-115">阻止剪贴板将数据从主机共享到容器, 并将容器从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="ac4d7-115">Block clipboard to share data both from Host to Container and from Container to Host</span></span>|
|<span data-ttu-id="ac4d7-116">blockHostToContainer</span><span class="sxs-lookup"><span data-stu-id="ac4d7-116">blockHostToContainer</span></span>|<span data-ttu-id="ac4d7-117">双面</span><span class="sxs-lookup"><span data-stu-id="ac4d7-117">2</span></span>|<span data-ttu-id="ac4d7-118">阻止剪贴板将数据从主机共享到容器</span><span class="sxs-lookup"><span data-stu-id="ac4d7-118">Block clipboard to share data from Host to Container</span></span>|
|<span data-ttu-id="ac4d7-119">blockContainerToHost</span><span class="sxs-lookup"><span data-stu-id="ac4d7-119">blockContainerToHost</span></span>|<span data-ttu-id="ac4d7-120">第三章</span><span class="sxs-lookup"><span data-stu-id="ac4d7-120">3</span></span>|<span data-ttu-id="ac4d7-121">阻止剪贴板将数据从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="ac4d7-121">Block clipboard to share data from Container to Host</span></span>|
|<span data-ttu-id="ac4d7-122">blockNone</span><span class="sxs-lookup"><span data-stu-id="ac4d7-122">blockNone</span></span>|<span data-ttu-id="ac4d7-123">4</span><span class="sxs-lookup"><span data-stu-id="ac4d7-123">4</span></span>|<span data-ttu-id="ac4d7-124">阻止剪贴板将数据从主机共享到容器, 也不将其从容器共享到主机</span><span class="sxs-lookup"><span data-stu-id="ac4d7-124">Block clipboard to share data neither from Host to Container nor from Container to Host</span></span>|



