---
title: applicationGuardBlockFileTransferType 枚举类型
description: ApplicationGuardBlockFileTransfer 的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 02eb1989c0218b66688f158461c4a66fa8c0a38a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27871951"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="f5888-103">applicationGuardBlockFileTransferType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f5888-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="f5888-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f5888-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f5888-105">ApplicationGuardBlockFileTransfer 的可能值</span><span class="sxs-lookup"><span data-stu-id="f5888-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="f5888-106">成员</span><span class="sxs-lookup"><span data-stu-id="f5888-106">Members</span></span>
|<span data-ttu-id="f5888-107">成员</span><span class="sxs-lookup"><span data-stu-id="f5888-107">Member</span></span>|<span data-ttu-id="f5888-108">值</span><span class="sxs-lookup"><span data-stu-id="f5888-108">Value</span></span>|<span data-ttu-id="f5888-109">Description</span><span class="sxs-lookup"><span data-stu-id="f5888-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f5888-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="f5888-110">notConfigured</span></span>|<span data-ttu-id="f5888-111">0</span><span class="sxs-lookup"><span data-stu-id="f5888-111">0</span></span>|<span data-ttu-id="f5888-112">未配置</span><span class="sxs-lookup"><span data-stu-id="f5888-112">Not Configured</span></span>|
|<span data-ttu-id="f5888-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="f5888-113">blockImageAndTextFile</span></span>|<span data-ttu-id="f5888-114">1</span><span class="sxs-lookup"><span data-stu-id="f5888-114">1</span></span>|<span data-ttu-id="f5888-115">阻止剪贴板将图像和文本文件传输</span><span class="sxs-lookup"><span data-stu-id="f5888-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="f5888-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="f5888-116">blockImageFile</span></span>|<span data-ttu-id="f5888-117">2</span><span class="sxs-lookup"><span data-stu-id="f5888-117">2</span></span>|<span data-ttu-id="f5888-118">阻止剪贴板将图像文件传输</span><span class="sxs-lookup"><span data-stu-id="f5888-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="f5888-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="f5888-119">blockNone</span></span>|<span data-ttu-id="f5888-120">3</span><span class="sxs-lookup"><span data-stu-id="f5888-120">3</span></span>|<span data-ttu-id="f5888-121">都不文本文件或图像文件，阻止在转接</span><span class="sxs-lookup"><span data-stu-id="f5888-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="f5888-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="f5888-122">blockTextFile</span></span>|<span data-ttu-id="f5888-123">4</span><span class="sxs-lookup"><span data-stu-id="f5888-123">4</span></span>|<span data-ttu-id="f5888-124">若要将文本文件传输的块剪贴板</span><span class="sxs-lookup"><span data-stu-id="f5888-124">Block clipboard to transfer Text file</span></span>|



