---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 2acf8fd19bcbadcbe6cb2371bf357babd4889b7b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49267843"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="b15e3-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b15e3-103">appLogUploadState enum type</span></span>

<span data-ttu-id="b15e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b15e3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b15e3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b15e3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b15e3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b15e3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b15e3-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="b15e3-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="b15e3-108">成员</span><span class="sxs-lookup"><span data-stu-id="b15e3-108">Members</span></span>
|<span data-ttu-id="b15e3-109">成员</span><span class="sxs-lookup"><span data-stu-id="b15e3-109">Member</span></span>|<span data-ttu-id="b15e3-110">值</span><span class="sxs-lookup"><span data-stu-id="b15e3-110">Value</span></span>|<span data-ttu-id="b15e3-111">说明</span><span class="sxs-lookup"><span data-stu-id="b15e3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b15e3-112">决</span><span class="sxs-lookup"><span data-stu-id="b15e3-112">pending</span></span>|<span data-ttu-id="b15e3-113">0</span><span class="sxs-lookup"><span data-stu-id="b15e3-113">0</span></span>|<span data-ttu-id="b15e3-114">请求正在等待处理或在处理</span><span class="sxs-lookup"><span data-stu-id="b15e3-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="b15e3-115">后</span><span class="sxs-lookup"><span data-stu-id="b15e3-115">completed</span></span>|<span data-ttu-id="b15e3-116">1</span><span class="sxs-lookup"><span data-stu-id="b15e3-116">1</span></span>|<span data-ttu-id="b15e3-117">请求已完成，且文件已上载到 Azure blob 以供下载。</span><span class="sxs-lookup"><span data-stu-id="b15e3-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="b15e3-118">未能</span><span class="sxs-lookup"><span data-stu-id="b15e3-118">failed</span></span>|<span data-ttu-id="b15e3-119">双面</span><span class="sxs-lookup"><span data-stu-id="b15e3-119">2</span></span>|<span data-ttu-id="b15e3-120">请求已完成处理且处于错误状态。</span><span class="sxs-lookup"><span data-stu-id="b15e3-120">Request finished processing and in error state.</span></span>|




