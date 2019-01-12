---
title: mobileAppContentFileUploadState 枚举类型
description: 包含上载请求状态属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 9a6f5a8f19ac874da58768fdd682f76530cb0dd1
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939600"
---
# <a name="mobileappcontentfileuploadstate-enum-type"></a><span data-ttu-id="0e355-103">mobileAppContentFileUploadState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0e355-103">mobileAppContentFileUploadState enum type</span></span>

> <span data-ttu-id="0e355-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e355-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e355-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e355-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e355-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e355-107">包含上载请求状态属性。</span><span class="sxs-lookup"><span data-stu-id="0e355-107">Contains properties for upload request states.</span></span>
## <a name="members"></a><span data-ttu-id="0e355-108">成员</span><span class="sxs-lookup"><span data-stu-id="0e355-108">Members</span></span>
|<span data-ttu-id="0e355-109">成员</span><span class="sxs-lookup"><span data-stu-id="0e355-109">Member</span></span>|<span data-ttu-id="0e355-110">值</span><span class="sxs-lookup"><span data-stu-id="0e355-110">Value</span></span>|<span data-ttu-id="0e355-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e355-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e355-112">success</span><span class="sxs-lookup"><span data-stu-id="0e355-112">success</span></span>|<span data-ttu-id="0e355-113">0</span><span class="sxs-lookup"><span data-stu-id="0e355-113">0</span></span>|<span data-ttu-id="0e355-114">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-114">Not yet documented</span></span>|
|<span data-ttu-id="0e355-115">transientError</span><span class="sxs-lookup"><span data-stu-id="0e355-115">transientError</span></span>|<span data-ttu-id="0e355-116">1</span><span class="sxs-lookup"><span data-stu-id="0e355-116">1</span></span>|<span data-ttu-id="0e355-117">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-117">Not yet documented</span></span>|
|<span data-ttu-id="0e355-118">error</span><span class="sxs-lookup"><span data-stu-id="0e355-118">error</span></span>|<span data-ttu-id="0e355-119">2</span><span class="sxs-lookup"><span data-stu-id="0e355-119">2</span></span>|<span data-ttu-id="0e355-120">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-120">Not yet documented</span></span>|
|<span data-ttu-id="0e355-121">unknown</span><span class="sxs-lookup"><span data-stu-id="0e355-121">unknown</span></span>|<span data-ttu-id="0e355-122">3</span><span class="sxs-lookup"><span data-stu-id="0e355-122">3</span></span>|<span data-ttu-id="0e355-123">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-123">Not yet documented</span></span>|
|<span data-ttu-id="0e355-124">azureStorageUriRequestSuccess</span><span class="sxs-lookup"><span data-stu-id="0e355-124">azureStorageUriRequestSuccess</span></span>|<span data-ttu-id="0e355-125">100</span><span class="sxs-lookup"><span data-stu-id="0e355-125">100</span></span>|<span data-ttu-id="0e355-126">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-126">Not yet documented</span></span>|
|<span data-ttu-id="0e355-127">azureStorageUriRequestPending</span><span class="sxs-lookup"><span data-stu-id="0e355-127">azureStorageUriRequestPending</span></span>|<span data-ttu-id="0e355-128">101</span><span class="sxs-lookup"><span data-stu-id="0e355-128">101</span></span>|<span data-ttu-id="0e355-129">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-129">Not yet documented</span></span>|
|<span data-ttu-id="0e355-130">azureStorageUriRequestFailed</span><span class="sxs-lookup"><span data-stu-id="0e355-130">azureStorageUriRequestFailed</span></span>|<span data-ttu-id="0e355-131">102</span><span class="sxs-lookup"><span data-stu-id="0e355-131">102</span></span>|<span data-ttu-id="0e355-132">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-132">Not yet documented</span></span>|
|<span data-ttu-id="0e355-133">azureStorageUriRequestTimedOut</span><span class="sxs-lookup"><span data-stu-id="0e355-133">azureStorageUriRequestTimedOut</span></span>|<span data-ttu-id="0e355-134">103</span><span class="sxs-lookup"><span data-stu-id="0e355-134">103</span></span>|<span data-ttu-id="0e355-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-135">Not yet documented</span></span>|
|<span data-ttu-id="0e355-136">azureStorageUriRenewalSuccess</span><span class="sxs-lookup"><span data-stu-id="0e355-136">azureStorageUriRenewalSuccess</span></span>|<span data-ttu-id="0e355-137">200</span><span class="sxs-lookup"><span data-stu-id="0e355-137">200</span></span>|<span data-ttu-id="0e355-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-138">Not yet documented</span></span>|
|<span data-ttu-id="0e355-139">azureStorageUriRenewalPending</span><span class="sxs-lookup"><span data-stu-id="0e355-139">azureStorageUriRenewalPending</span></span>|<span data-ttu-id="0e355-140">201</span><span class="sxs-lookup"><span data-stu-id="0e355-140">201</span></span>|<span data-ttu-id="0e355-141">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-141">Not yet documented</span></span>|
|<span data-ttu-id="0e355-142">azureStorageUriRenewalFailed</span><span class="sxs-lookup"><span data-stu-id="0e355-142">azureStorageUriRenewalFailed</span></span>|<span data-ttu-id="0e355-143">202</span><span class="sxs-lookup"><span data-stu-id="0e355-143">202</span></span>|<span data-ttu-id="0e355-144">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-144">Not yet documented</span></span>|
|<span data-ttu-id="0e355-145">azureStorageUriRenewalTimedOut</span><span class="sxs-lookup"><span data-stu-id="0e355-145">azureStorageUriRenewalTimedOut</span></span>|<span data-ttu-id="0e355-146">203</span><span class="sxs-lookup"><span data-stu-id="0e355-146">203</span></span>|<span data-ttu-id="0e355-147">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-147">Not yet documented</span></span>|
|<span data-ttu-id="0e355-148">commitFileSuccess</span><span class="sxs-lookup"><span data-stu-id="0e355-148">commitFileSuccess</span></span>|<span data-ttu-id="0e355-149">300</span><span class="sxs-lookup"><span data-stu-id="0e355-149">300</span></span>|<span data-ttu-id="0e355-150">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-150">Not yet documented</span></span>|
|<span data-ttu-id="0e355-151">commitFilePending</span><span class="sxs-lookup"><span data-stu-id="0e355-151">commitFilePending</span></span>|<span data-ttu-id="0e355-152">301</span><span class="sxs-lookup"><span data-stu-id="0e355-152">301</span></span>|<span data-ttu-id="0e355-153">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-153">Not yet documented</span></span>|
|<span data-ttu-id="0e355-154">commitFileFailed</span><span class="sxs-lookup"><span data-stu-id="0e355-154">commitFileFailed</span></span>|<span data-ttu-id="0e355-155">302</span><span class="sxs-lookup"><span data-stu-id="0e355-155">302</span></span>|<span data-ttu-id="0e355-156">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-156">Not yet documented</span></span>|
|<span data-ttu-id="0e355-157">commitFileTimedOut</span><span class="sxs-lookup"><span data-stu-id="0e355-157">commitFileTimedOut</span></span>|<span data-ttu-id="0e355-158">303</span><span class="sxs-lookup"><span data-stu-id="0e355-158">303</span></span>|<span data-ttu-id="0e355-159">尚未记录</span><span class="sxs-lookup"><span data-stu-id="0e355-159">Not yet documented</span></span>|





