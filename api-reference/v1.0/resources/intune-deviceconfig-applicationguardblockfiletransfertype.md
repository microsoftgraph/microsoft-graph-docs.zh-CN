---
title: applicationGuardBlockFileTransferType 枚举类型
description: ApplicationGuardBlockFileTransfer 的可能值
author: tfitzmac
ms.openlocfilehash: 5ec313ea62341734152382f3ff7852bf8bc051bb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27326619"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="befc1-103">applicationGuardBlockFileTransferType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="befc1-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="befc1-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="befc1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="befc1-105">ApplicationGuardBlockFileTransfer 的可能值</span><span class="sxs-lookup"><span data-stu-id="befc1-105">Possible values for applicationGuardBlockFileTransfer</span></span>
## <a name="members"></a><span data-ttu-id="befc1-106">成员</span><span class="sxs-lookup"><span data-stu-id="befc1-106">Members</span></span>
|<span data-ttu-id="befc1-107">成员</span><span class="sxs-lookup"><span data-stu-id="befc1-107">Member</span></span>|<span data-ttu-id="befc1-108">值</span><span class="sxs-lookup"><span data-stu-id="befc1-108">Value</span></span>|<span data-ttu-id="befc1-109">说明</span><span class="sxs-lookup"><span data-stu-id="befc1-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="befc1-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="befc1-110">notConfigured</span></span>|<span data-ttu-id="befc1-111">0</span><span class="sxs-lookup"><span data-stu-id="befc1-111">0</span></span>|<span data-ttu-id="befc1-112">未配置</span><span class="sxs-lookup"><span data-stu-id="befc1-112">Not Configured</span></span>|
|<span data-ttu-id="befc1-113">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="befc1-113">blockImageAndTextFile</span></span>|<span data-ttu-id="befc1-114">1</span><span class="sxs-lookup"><span data-stu-id="befc1-114">1</span></span>|<span data-ttu-id="befc1-115">阻止剪贴板将图像和文本文件传输</span><span class="sxs-lookup"><span data-stu-id="befc1-115">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="befc1-116">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="befc1-116">blockImageFile</span></span>|<span data-ttu-id="befc1-117">2</span><span class="sxs-lookup"><span data-stu-id="befc1-117">2</span></span>|<span data-ttu-id="befc1-118">阻止剪贴板将图像文件传输</span><span class="sxs-lookup"><span data-stu-id="befc1-118">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="befc1-119">blockNone</span><span class="sxs-lookup"><span data-stu-id="befc1-119">blockNone</span></span>|<span data-ttu-id="befc1-120">3</span><span class="sxs-lookup"><span data-stu-id="befc1-120">3</span></span>|<span data-ttu-id="befc1-121">都不文本文件或图像文件，阻止在转接</span><span class="sxs-lookup"><span data-stu-id="befc1-121">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="befc1-122">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="befc1-122">blockTextFile</span></span>|<span data-ttu-id="befc1-123">4</span><span class="sxs-lookup"><span data-stu-id="befc1-123">4</span></span>|<span data-ttu-id="befc1-124">若要将文本文件传输的块剪贴板</span><span class="sxs-lookup"><span data-stu-id="befc1-124">Block clipboard to transfer Text file</span></span>|



