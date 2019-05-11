---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c6a0c880fe8fa7fe743bea3ad42fee6d1e24d209
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943114"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="69b9d-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="69b9d-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="69b9d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69b9d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69b9d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69b9d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69b9d-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="69b9d-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="69b9d-107">成员</span><span class="sxs-lookup"><span data-stu-id="69b9d-107">Members</span></span>
|<span data-ttu-id="69b9d-108">成员</span><span class="sxs-lookup"><span data-stu-id="69b9d-108">Member</span></span>|<span data-ttu-id="69b9d-109">值</span><span class="sxs-lookup"><span data-stu-id="69b9d-109">Value</span></span>|<span data-ttu-id="69b9d-110">说明</span><span class="sxs-lookup"><span data-stu-id="69b9d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="69b9d-111">决</span><span class="sxs-lookup"><span data-stu-id="69b9d-111">pending</span></span>|<span data-ttu-id="69b9d-112">0</span><span class="sxs-lookup"><span data-stu-id="69b9d-112">0</span></span>|<span data-ttu-id="69b9d-113">请求正在等待处理或在处理</span><span class="sxs-lookup"><span data-stu-id="69b9d-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="69b9d-114">后</span><span class="sxs-lookup"><span data-stu-id="69b9d-114">completed</span></span>|<span data-ttu-id="69b9d-115">1</span><span class="sxs-lookup"><span data-stu-id="69b9d-115">1</span></span>|<span data-ttu-id="69b9d-116">请求已完成, 且文件已上载到 Azure blob 以供下载。</span><span class="sxs-lookup"><span data-stu-id="69b9d-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="69b9d-117">未能</span><span class="sxs-lookup"><span data-stu-id="69b9d-117">failed</span></span>|<span data-ttu-id="69b9d-118">双面</span><span class="sxs-lookup"><span data-stu-id="69b9d-118">2</span></span>|<span data-ttu-id="69b9d-119">请求已完成处理且处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="69b9d-119">Request finished processing and in error state.</span></span>|




