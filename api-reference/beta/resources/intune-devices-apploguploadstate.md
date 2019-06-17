---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebfbed2517143cb4574d75afad77f2f822e503cd
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983377"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="5934a-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5934a-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="5934a-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5934a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5934a-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5934a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5934a-106">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="5934a-106">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="5934a-107">成员</span><span class="sxs-lookup"><span data-stu-id="5934a-107">Members</span></span>
|<span data-ttu-id="5934a-108">成员</span><span class="sxs-lookup"><span data-stu-id="5934a-108">Member</span></span>|<span data-ttu-id="5934a-109">值</span><span class="sxs-lookup"><span data-stu-id="5934a-109">Value</span></span>|<span data-ttu-id="5934a-110">说明</span><span class="sxs-lookup"><span data-stu-id="5934a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5934a-111">决</span><span class="sxs-lookup"><span data-stu-id="5934a-111">pending</span></span>|<span data-ttu-id="5934a-112">0</span><span class="sxs-lookup"><span data-stu-id="5934a-112">0</span></span>|<span data-ttu-id="5934a-113">请求正在等待处理或在处理</span><span class="sxs-lookup"><span data-stu-id="5934a-113">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="5934a-114">后</span><span class="sxs-lookup"><span data-stu-id="5934a-114">completed</span></span>|<span data-ttu-id="5934a-115">1</span><span class="sxs-lookup"><span data-stu-id="5934a-115">1</span></span>|<span data-ttu-id="5934a-116">请求已完成, 且文件已上载到 Azure blob 以供下载。</span><span class="sxs-lookup"><span data-stu-id="5934a-116">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="5934a-117">未能</span><span class="sxs-lookup"><span data-stu-id="5934a-117">failed</span></span>|<span data-ttu-id="5934a-118">双面</span><span class="sxs-lookup"><span data-stu-id="5934a-118">2</span></span>|<span data-ttu-id="5934a-119">请求已完成处理且处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="5934a-119">Request finished processing and in error state.</span></span>|





