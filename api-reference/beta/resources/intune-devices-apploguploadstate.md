---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fed773a22ba0e538785211ece7849669efd9d383
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48725524"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="252fe-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="252fe-103">appLogUploadState enum type</span></span>

<span data-ttu-id="252fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="252fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="252fe-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="252fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="252fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="252fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="252fe-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="252fe-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="252fe-108">成员</span><span class="sxs-lookup"><span data-stu-id="252fe-108">Members</span></span>
|<span data-ttu-id="252fe-109">成员</span><span class="sxs-lookup"><span data-stu-id="252fe-109">Member</span></span>|<span data-ttu-id="252fe-110">值</span><span class="sxs-lookup"><span data-stu-id="252fe-110">Value</span></span>|<span data-ttu-id="252fe-111">说明</span><span class="sxs-lookup"><span data-stu-id="252fe-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="252fe-112">决</span><span class="sxs-lookup"><span data-stu-id="252fe-112">pending</span></span>|<span data-ttu-id="252fe-113">0</span><span class="sxs-lookup"><span data-stu-id="252fe-113">0</span></span>|<span data-ttu-id="252fe-114">请求正在等待处理或在处理</span><span class="sxs-lookup"><span data-stu-id="252fe-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="252fe-115">后</span><span class="sxs-lookup"><span data-stu-id="252fe-115">completed</span></span>|<span data-ttu-id="252fe-116">1</span><span class="sxs-lookup"><span data-stu-id="252fe-116">1</span></span>|<span data-ttu-id="252fe-117">请求已完成，且文件已上载到 Azure blob 以供下载。</span><span class="sxs-lookup"><span data-stu-id="252fe-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="252fe-118">未能</span><span class="sxs-lookup"><span data-stu-id="252fe-118">failed</span></span>|<span data-ttu-id="252fe-119">双面</span><span class="sxs-lookup"><span data-stu-id="252fe-119">2</span></span>|<span data-ttu-id="252fe-120">请求已完成处理且处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="252fe-120">Request finished processing and in error state.</span></span>|





