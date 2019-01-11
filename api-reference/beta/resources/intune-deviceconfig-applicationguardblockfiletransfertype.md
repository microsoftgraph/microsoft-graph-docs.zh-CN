---
title: applicationGuardBlockFileTransferType 枚举类型
description: ApplicationGuardBlockFileTransfer 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 63460da5d7b3d78c302b706a8aeedcdedb066c48
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835298"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="94b53-103">applicationGuardBlockFileTransferType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="94b53-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="94b53-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="94b53-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="94b53-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="94b53-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="94b53-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="94b53-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="94b53-107">ApplicationGuardBlockFileTransfer 的可能值</span><span class="sxs-lookup"><span data-stu-id="94b53-107">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="94b53-108">成员</span><span class="sxs-lookup"><span data-stu-id="94b53-108">Members</span></span>
|<span data-ttu-id="94b53-109">成员</span><span class="sxs-lookup"><span data-stu-id="94b53-109">Member</span></span>|<span data-ttu-id="94b53-110">值</span><span class="sxs-lookup"><span data-stu-id="94b53-110">Value</span></span>|<span data-ttu-id="94b53-111">Description</span><span class="sxs-lookup"><span data-stu-id="94b53-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94b53-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="94b53-112">notConfigured</span></span>|<span data-ttu-id="94b53-113">0</span><span class="sxs-lookup"><span data-stu-id="94b53-113">0</span></span>|<span data-ttu-id="94b53-114">未配置</span><span class="sxs-lookup"><span data-stu-id="94b53-114">Not Configured</span></span>|
|<span data-ttu-id="94b53-115">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="94b53-115">blockImageAndTextFile</span></span>|<span data-ttu-id="94b53-116">1</span><span class="sxs-lookup"><span data-stu-id="94b53-116">1</span></span>|<span data-ttu-id="94b53-117">阻止剪贴板将图像和文本文件传输</span><span class="sxs-lookup"><span data-stu-id="94b53-117">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="94b53-118">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="94b53-118">blockImageFile</span></span>|<span data-ttu-id="94b53-119">2</span><span class="sxs-lookup"><span data-stu-id="94b53-119">2</span></span>|<span data-ttu-id="94b53-120">阻止剪贴板将图像文件传输</span><span class="sxs-lookup"><span data-stu-id="94b53-120">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="94b53-121">blockNone</span><span class="sxs-lookup"><span data-stu-id="94b53-121">blockNone</span></span>|<span data-ttu-id="94b53-122">3</span><span class="sxs-lookup"><span data-stu-id="94b53-122">3</span></span>|<span data-ttu-id="94b53-123">都不文本文件或图像文件，阻止在转接</span><span class="sxs-lookup"><span data-stu-id="94b53-123">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="94b53-124">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="94b53-124">blockTextFile</span></span>|<span data-ttu-id="94b53-125">4</span><span class="sxs-lookup"><span data-stu-id="94b53-125">4</span></span>|<span data-ttu-id="94b53-126">若要将文本文件传输的块剪贴板</span><span class="sxs-lookup"><span data-stu-id="94b53-126">Block clipboard to transfer Text file</span></span>|





