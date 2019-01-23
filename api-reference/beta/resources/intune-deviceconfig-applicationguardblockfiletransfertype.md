---
title: applicationGuardBlockFileTransferType 枚举类型
description: ApplicationGuardBlockFileTransfer 的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9997956d192686a5287e181b25bd5f98184299c5
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396271"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="cc4b6-103">applicationGuardBlockFileTransferType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cc4b6-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="cc4b6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="cc4b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="cc4b6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cc4b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cc4b6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cc4b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc4b6-107">ApplicationGuardBlockFileTransfer 的可能值</span><span class="sxs-lookup"><span data-stu-id="cc4b6-107">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="cc4b6-108">成员</span><span class="sxs-lookup"><span data-stu-id="cc4b6-108">Members</span></span>
|<span data-ttu-id="cc4b6-109">成员</span><span class="sxs-lookup"><span data-stu-id="cc4b6-109">Member</span></span>|<span data-ttu-id="cc4b6-110">值</span><span class="sxs-lookup"><span data-stu-id="cc4b6-110">Value</span></span>|<span data-ttu-id="cc4b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="cc4b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cc4b6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="cc4b6-112">notConfigured</span></span>|<span data-ttu-id="cc4b6-113">0</span><span class="sxs-lookup"><span data-stu-id="cc4b6-113">0</span></span>|<span data-ttu-id="cc4b6-114">未配置</span><span class="sxs-lookup"><span data-stu-id="cc4b6-114">Not Configured</span></span>|
|<span data-ttu-id="cc4b6-115">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="cc4b6-115">blockImageAndTextFile</span></span>|<span data-ttu-id="cc4b6-116">1</span><span class="sxs-lookup"><span data-stu-id="cc4b6-116">1</span></span>|<span data-ttu-id="cc4b6-117">阻止剪贴板将图像和文本文件传输</span><span class="sxs-lookup"><span data-stu-id="cc4b6-117">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="cc4b6-118">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="cc4b6-118">blockImageFile</span></span>|<span data-ttu-id="cc4b6-119">2</span><span class="sxs-lookup"><span data-stu-id="cc4b6-119">2</span></span>|<span data-ttu-id="cc4b6-120">阻止剪贴板将图像文件传输</span><span class="sxs-lookup"><span data-stu-id="cc4b6-120">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="cc4b6-121">blockNone</span><span class="sxs-lookup"><span data-stu-id="cc4b6-121">blockNone</span></span>|<span data-ttu-id="cc4b6-122">3</span><span class="sxs-lookup"><span data-stu-id="cc4b6-122">3</span></span>|<span data-ttu-id="cc4b6-123">都不文本文件或图像文件，阻止在转接</span><span class="sxs-lookup"><span data-stu-id="cc4b6-123">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="cc4b6-124">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="cc4b6-124">blockTextFile</span></span>|<span data-ttu-id="cc4b6-125">4</span><span class="sxs-lookup"><span data-stu-id="cc4b6-125">4</span></span>|<span data-ttu-id="cc4b6-126">若要将文本文件传输的块剪贴板</span><span class="sxs-lookup"><span data-stu-id="cc4b6-126">Block clipboard to transfer Text file</span></span>|




