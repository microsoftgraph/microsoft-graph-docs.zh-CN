---
title: applicationGuardBlockFileTransferType 枚举类型
description: applicationGuardBlockFileTransfer 的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5a35c830375195c9957884771b8e837a40ca984c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562291"
---
# <a name="applicationguardblockfiletransfertype-enum-type"></a><span data-ttu-id="0adbc-103">applicationGuardBlockFileTransferType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0adbc-103">applicationGuardBlockFileTransferType enum type</span></span>

> <span data-ttu-id="0adbc-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0adbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0adbc-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0adbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0adbc-106">applicationGuardBlockFileTransfer 的可能值</span><span class="sxs-lookup"><span data-stu-id="0adbc-106">Possible values for applicationGuardBlockFileTransfer</span></span>

## <a name="members"></a><span data-ttu-id="0adbc-107">成员</span><span class="sxs-lookup"><span data-stu-id="0adbc-107">Members</span></span>
|<span data-ttu-id="0adbc-108">成员</span><span class="sxs-lookup"><span data-stu-id="0adbc-108">Member</span></span>|<span data-ttu-id="0adbc-109">值</span><span class="sxs-lookup"><span data-stu-id="0adbc-109">Value</span></span>|<span data-ttu-id="0adbc-110">说明</span><span class="sxs-lookup"><span data-stu-id="0adbc-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0adbc-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0adbc-111">notConfigured</span></span>|<span data-ttu-id="0adbc-112">0</span><span class="sxs-lookup"><span data-stu-id="0adbc-112">0</span></span>|<span data-ttu-id="0adbc-113">未配置</span><span class="sxs-lookup"><span data-stu-id="0adbc-113">Not Configured</span></span>|
|<span data-ttu-id="0adbc-114">blockImageAndTextFile</span><span class="sxs-lookup"><span data-stu-id="0adbc-114">blockImageAndTextFile</span></span>|<span data-ttu-id="0adbc-115">1</span><span class="sxs-lookup"><span data-stu-id="0adbc-115">1</span></span>|<span data-ttu-id="0adbc-116">阻止剪贴板传输图像和文本文件</span><span class="sxs-lookup"><span data-stu-id="0adbc-116">Block clipboard to transfer Image and Text file</span></span>|
|<span data-ttu-id="0adbc-117">blockImageFile</span><span class="sxs-lookup"><span data-stu-id="0adbc-117">blockImageFile</span></span>|<span data-ttu-id="0adbc-118">2 </span><span class="sxs-lookup"><span data-stu-id="0adbc-118">2</span></span>|<span data-ttu-id="0adbc-119">阻止剪贴板传输图像文件</span><span class="sxs-lookup"><span data-stu-id="0adbc-119">Block clipboard to transfer Image file</span></span>|
|<span data-ttu-id="0adbc-120">blockNone</span><span class="sxs-lookup"><span data-stu-id="0adbc-120">blockNone</span></span>|<span data-ttu-id="0adbc-121">3 </span><span class="sxs-lookup"><span data-stu-id="0adbc-121">3</span></span>|<span data-ttu-id="0adbc-122">不会阻止文本文件或图像文件传输</span><span class="sxs-lookup"><span data-stu-id="0adbc-122">Neither of text file or image file is blocked from transferring</span></span>|
|<span data-ttu-id="0adbc-123">blockTextFile</span><span class="sxs-lookup"><span data-stu-id="0adbc-123">blockTextFile</span></span>|<span data-ttu-id="0adbc-124">4 </span><span class="sxs-lookup"><span data-stu-id="0adbc-124">4</span></span>|<span data-ttu-id="0adbc-125">阻止剪贴板传输文本文件</span><span class="sxs-lookup"><span data-stu-id="0adbc-125">Block clipboard to transfer Text file</span></span>|





