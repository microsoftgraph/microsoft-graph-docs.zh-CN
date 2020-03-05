---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: d692e352f177c7f882a33e49604934c4b1a22912
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42525164"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="6ed02-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6ed02-103">appLogUploadState enum type</span></span>

<span data-ttu-id="6ed02-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6ed02-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6ed02-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6ed02-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ed02-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6ed02-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ed02-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="6ed02-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="6ed02-108">成员</span><span class="sxs-lookup"><span data-stu-id="6ed02-108">Members</span></span>
|<span data-ttu-id="6ed02-109">成员</span><span class="sxs-lookup"><span data-stu-id="6ed02-109">Member</span></span>|<span data-ttu-id="6ed02-110">值</span><span class="sxs-lookup"><span data-stu-id="6ed02-110">Value</span></span>|<span data-ttu-id="6ed02-111">说明</span><span class="sxs-lookup"><span data-stu-id="6ed02-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ed02-112">决</span><span class="sxs-lookup"><span data-stu-id="6ed02-112">pending</span></span>|<span data-ttu-id="6ed02-113">0</span><span class="sxs-lookup"><span data-stu-id="6ed02-113">0</span></span>|<span data-ttu-id="6ed02-114">请求正在等待处理或在处理</span><span class="sxs-lookup"><span data-stu-id="6ed02-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="6ed02-115">后</span><span class="sxs-lookup"><span data-stu-id="6ed02-115">completed</span></span>|<span data-ttu-id="6ed02-116">1 </span><span class="sxs-lookup"><span data-stu-id="6ed02-116">1</span></span>|<span data-ttu-id="6ed02-117">请求已完成，且文件已上载到 Azure blob 以供下载。</span><span class="sxs-lookup"><span data-stu-id="6ed02-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="6ed02-118">未能</span><span class="sxs-lookup"><span data-stu-id="6ed02-118">failed</span></span>|<span data-ttu-id="6ed02-119">2 </span><span class="sxs-lookup"><span data-stu-id="6ed02-119">2</span></span>|<span data-ttu-id="6ed02-120">请求已完成处理且处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="6ed02-120">Request finished processing and in error state.</span></span>|



