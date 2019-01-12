---
title: applicationGuardBlockFileTransferType 枚举类型
description: ApplicationGuardBlockFileTransfer 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f6eb5c7c3f26fb62e73e9b1e103d111f6c652f5c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27931263"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="ba638-103">applicationGuardBlockFileTransferType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ba638-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="ba638-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ba638-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ba638-105">ApplicationGuardBlockFileTransfer 的可能值</span><span class="sxs-lookup"><span data-stu-id="ba638-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="ba638-106">成员</span><span class="sxs-lookup"><span data-stu-id="ba638-106">Members</span></span>
|<span data-ttu-id="ba638-107">成员</span><span class="sxs-lookup"><span data-stu-id="ba638-107">Member</span></span>|<span data-ttu-id="ba638-108">值</span><span class="sxs-lookup"><span data-stu-id="ba638-108">Value</span></span>|<span data-ttu-id="ba638-109">Description</span><span class="sxs-lookup"><span data-stu-id="ba638-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ba638-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ba638-110">notConfigured</span></span>|<span data-ttu-id="ba638-111">0</span><span class="sxs-lookup"><span data-stu-id="ba638-111">0</span></span>|<span data-ttu-id="ba638-112">未配置</span><span class="sxs-lookup"><span data-stu-id="ba638-112">Not Configured</span></span>|
|<span data-ttu-id="ba638-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="ba638-113">blockImageAndTextFile</span></span>|<span data-ttu-id="ba638-114">1</span><span class="sxs-lookup"><span data-stu-id="ba638-114">1</span></span>|<span data-ttu-id="ba638-115">阻止剪贴板将图像和文本文件传输</span><span class="sxs-lookup"><span data-stu-id="ba638-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="ba638-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="ba638-116">blockImageFile</span></span>|<span data-ttu-id="ba638-117">2</span><span class="sxs-lookup"><span data-stu-id="ba638-117">2</span></span>|<span data-ttu-id="ba638-118">阻止剪贴板将图像文件传输</span><span class="sxs-lookup"><span data-stu-id="ba638-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="ba638-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="ba638-119">blockNone</span></span>|<span data-ttu-id="ba638-120">3</span><span class="sxs-lookup"><span data-stu-id="ba638-120">3</span></span>|<span data-ttu-id="ba638-121">都不文本文件或图像文件，阻止在转接</span><span class="sxs-lookup"><span data-stu-id="ba638-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="ba638-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="ba638-122">blockTextFile</span></span>|<span data-ttu-id="ba638-123">4</span><span class="sxs-lookup"><span data-stu-id="ba638-123">4</span></span>|<span data-ttu-id="ba638-124">若要将文本文件传输的块剪贴板</span><span class="sxs-lookup"><span data-stu-id="ba638-124">Block clipboard to transfer Text file</span></span>|



