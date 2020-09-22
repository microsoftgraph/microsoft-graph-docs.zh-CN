---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f3a39e8155c6cb18291ee233574c592f3ce964ca
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060831"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="21fd5-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21fd5-103">appLogUploadState enum type</span></span>

<span data-ttu-id="21fd5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="21fd5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="21fd5-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21fd5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21fd5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21fd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21fd5-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="21fd5-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="21fd5-108">成员</span><span class="sxs-lookup"><span data-stu-id="21fd5-108">Members</span></span>
|<span data-ttu-id="21fd5-109">成员</span><span class="sxs-lookup"><span data-stu-id="21fd5-109">Member</span></span>|<span data-ttu-id="21fd5-110">值</span><span class="sxs-lookup"><span data-stu-id="21fd5-110">Value</span></span>|<span data-ttu-id="21fd5-111">说明</span><span class="sxs-lookup"><span data-stu-id="21fd5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21fd5-112">决</span><span class="sxs-lookup"><span data-stu-id="21fd5-112">pending</span></span>|<span data-ttu-id="21fd5-113">0</span><span class="sxs-lookup"><span data-stu-id="21fd5-113">0</span></span>|<span data-ttu-id="21fd5-114">请求正在等待处理或在处理</span><span class="sxs-lookup"><span data-stu-id="21fd5-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="21fd5-115">后</span><span class="sxs-lookup"><span data-stu-id="21fd5-115">completed</span></span>|<span data-ttu-id="21fd5-116">1 </span><span class="sxs-lookup"><span data-stu-id="21fd5-116">1</span></span>|<span data-ttu-id="21fd5-117">请求已完成，且文件已上载到 Azure blob 以供下载。</span><span class="sxs-lookup"><span data-stu-id="21fd5-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="21fd5-118">未能</span><span class="sxs-lookup"><span data-stu-id="21fd5-118">failed</span></span>|<span data-ttu-id="21fd5-119">2 </span><span class="sxs-lookup"><span data-stu-id="21fd5-119">2</span></span>|<span data-ttu-id="21fd5-120">请求已完成处理且处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="21fd5-120">Request finished processing and in error state.</span></span>|






