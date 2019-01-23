---
title: appLogUploadState 枚举类型
description: AppLogUploadStatus
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 58dcc0d4a15370d6449772d917e8994f0eb9e7bd
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431396"
---
# <a name="apploguploadstate-enum-type"></a><span data-ttu-id="e976f-103">appLogUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e976f-103">appLogUploadState enum type</span></span>

> <span data-ttu-id="e976f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e976f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e976f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e976f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e976f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e976f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e976f-107">AppLogUploadStatus</span><span class="sxs-lookup"><span data-stu-id="e976f-107">AppLogUploadStatus</span></span>

## <a name="members"></a><span data-ttu-id="e976f-108">成员</span><span class="sxs-lookup"><span data-stu-id="e976f-108">Members</span></span>
|<span data-ttu-id="e976f-109">成员</span><span class="sxs-lookup"><span data-stu-id="e976f-109">Member</span></span>|<span data-ttu-id="e976f-110">值</span><span class="sxs-lookup"><span data-stu-id="e976f-110">Value</span></span>|<span data-ttu-id="e976f-111">说明</span><span class="sxs-lookup"><span data-stu-id="e976f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e976f-112">挂起</span><span class="sxs-lookup"><span data-stu-id="e976f-112">pending</span></span>|<span data-ttu-id="e976f-113">0</span><span class="sxs-lookup"><span data-stu-id="e976f-113">0</span></span>|<span data-ttu-id="e976f-114">正在等待处理请求或将其在处理</span><span class="sxs-lookup"><span data-stu-id="e976f-114">Request is waiting to be processed or under processing</span></span>|
|<span data-ttu-id="e976f-115">完成</span><span class="sxs-lookup"><span data-stu-id="e976f-115">completed</span></span>|<span data-ttu-id="e976f-116">1</span><span class="sxs-lookup"><span data-stu-id="e976f-116">1</span></span>|<span data-ttu-id="e976f-117">文件上载到下载 Azure blob 完成请求。</span><span class="sxs-lookup"><span data-stu-id="e976f-117">Request is completed with file uploaded to Azure blob for download.</span></span>|
|<span data-ttu-id="e976f-118">failed</span><span class="sxs-lookup"><span data-stu-id="e976f-118">failed</span></span>|<span data-ttu-id="e976f-119">2</span><span class="sxs-lookup"><span data-stu-id="e976f-119">2</span></span>|<span data-ttu-id="e976f-120">请求完成处理和错误状态。</span><span class="sxs-lookup"><span data-stu-id="e976f-120">Request finished processing and in error state.</span></span>|




