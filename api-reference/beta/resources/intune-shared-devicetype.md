---
title: deviceType 枚举类型
description: 设备类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 31342399cad690b3f95dcbc8494998de455cdaa7
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29400618"
---
# <a name="devicetype-enum-type"></a><span data-ttu-id="b1373-103">deviceType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b1373-103">deviceType enum type</span></span>

> <span data-ttu-id="b1373-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b1373-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b1373-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b1373-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b1373-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b1373-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b1373-107">设备类型。</span><span class="sxs-lookup"><span data-stu-id="b1373-107">Device type.</span></span>

## <a name="members"></a><span data-ttu-id="b1373-108">成员</span><span class="sxs-lookup"><span data-stu-id="b1373-108">Members</span></span>
|<span data-ttu-id="b1373-109">成员</span><span class="sxs-lookup"><span data-stu-id="b1373-109">Member</span></span>|<span data-ttu-id="b1373-110">值</span><span class="sxs-lookup"><span data-stu-id="b1373-110">Value</span></span>|<span data-ttu-id="b1373-111">说明</span><span class="sxs-lookup"><span data-stu-id="b1373-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b1373-112">桌面</span><span class="sxs-lookup"><span data-stu-id="b1373-112">desktop</span></span>|<span data-ttu-id="b1373-113">0</span><span class="sxs-lookup"><span data-stu-id="b1373-113">0</span></span>|<span data-ttu-id="b1373-114">桌面。</span><span class="sxs-lookup"><span data-stu-id="b1373-114">Desktop.</span></span>|
|<span data-ttu-id="b1373-115">windowsRT</span><span class="sxs-lookup"><span data-stu-id="b1373-115">windowsRT</span></span>|<span data-ttu-id="b1373-116">1</span><span class="sxs-lookup"><span data-stu-id="b1373-116">1</span></span>|<span data-ttu-id="b1373-117">WindowsRT。</span><span class="sxs-lookup"><span data-stu-id="b1373-117">WindowsRT.</span></span>|
|<span data-ttu-id="b1373-118">winMO6</span><span class="sxs-lookup"><span data-stu-id="b1373-118">winMO6</span></span>|<span data-ttu-id="b1373-119">2</span><span class="sxs-lookup"><span data-stu-id="b1373-119">2</span></span>|<span data-ttu-id="b1373-120">WinMO6。</span><span class="sxs-lookup"><span data-stu-id="b1373-120">WinMO6.</span></span>|
|<span data-ttu-id="b1373-121">nokia</span><span class="sxs-lookup"><span data-stu-id="b1373-121">nokia</span></span>|<span data-ttu-id="b1373-122">3</span><span class="sxs-lookup"><span data-stu-id="b1373-122">3</span></span>|<span data-ttu-id="b1373-123">Nokia。</span><span class="sxs-lookup"><span data-stu-id="b1373-123">Nokia.</span></span>|
|<span data-ttu-id="b1373-124">windowsPhone</span><span class="sxs-lookup"><span data-stu-id="b1373-124">windowsPhone</span></span>|<span data-ttu-id="b1373-125">4</span><span class="sxs-lookup"><span data-stu-id="b1373-125">4</span></span>|<span data-ttu-id="b1373-126">Windows phone。</span><span class="sxs-lookup"><span data-stu-id="b1373-126">Windows phone.</span></span>|
|<span data-ttu-id="b1373-127">mac</span><span class="sxs-lookup"><span data-stu-id="b1373-127">mac</span></span>|<span data-ttu-id="b1373-128">5</span><span class="sxs-lookup"><span data-stu-id="b1373-128">5</span></span>|<span data-ttu-id="b1373-129">Mac。</span><span class="sxs-lookup"><span data-stu-id="b1373-129">Mac.</span></span>|
|<span data-ttu-id="b1373-130">winCE</span><span class="sxs-lookup"><span data-stu-id="b1373-130">winCE</span></span>|<span data-ttu-id="b1373-131">6</span><span class="sxs-lookup"><span data-stu-id="b1373-131">6</span></span>|<span data-ttu-id="b1373-132">WinCE。</span><span class="sxs-lookup"><span data-stu-id="b1373-132">WinCE.</span></span>|
|<span data-ttu-id="b1373-133">winEmbedded</span><span class="sxs-lookup"><span data-stu-id="b1373-133">winEmbedded</span></span>|<span data-ttu-id="b1373-134">7</span><span class="sxs-lookup"><span data-stu-id="b1373-134">7</span></span>|<span data-ttu-id="b1373-135">WinEmbedded。</span><span class="sxs-lookup"><span data-stu-id="b1373-135">WinEmbedded.</span></span>|
|<span data-ttu-id="b1373-136">iPhone</span><span class="sxs-lookup"><span data-stu-id="b1373-136">iPhone</span></span>|<span data-ttu-id="b1373-137">8</span><span class="sxs-lookup"><span data-stu-id="b1373-137">8</span></span>|<span data-ttu-id="b1373-138">iPhone。</span><span class="sxs-lookup"><span data-stu-id="b1373-138">iPhone.</span></span>|
|<span data-ttu-id="b1373-139">iPad</span><span class="sxs-lookup"><span data-stu-id="b1373-139">iPad</span></span>|<span data-ttu-id="b1373-140">9</span><span class="sxs-lookup"><span data-stu-id="b1373-140">9</span></span>|<span data-ttu-id="b1373-141">iPad。</span><span class="sxs-lookup"><span data-stu-id="b1373-141">iPad.</span></span>|
|<span data-ttu-id="b1373-142">iPod</span><span class="sxs-lookup"><span data-stu-id="b1373-142">iPod</span></span>|<span data-ttu-id="b1373-143">10</span><span class="sxs-lookup"><span data-stu-id="b1373-143">10</span></span>|<span data-ttu-id="b1373-144">iPodTouch。</span><span class="sxs-lookup"><span data-stu-id="b1373-144">iPodTouch.</span></span>|
|<span data-ttu-id="b1373-145">android</span><span class="sxs-lookup"><span data-stu-id="b1373-145">android</span></span>|<span data-ttu-id="b1373-146">11</span><span class="sxs-lookup"><span data-stu-id="b1373-146">11</span></span>|<span data-ttu-id="b1373-147">Android。</span><span class="sxs-lookup"><span data-stu-id="b1373-147">Android.</span></span>|
|<span data-ttu-id="b1373-148">iSocConsumer</span><span class="sxs-lookup"><span data-stu-id="b1373-148">iSocConsumer</span></span>|<span data-ttu-id="b1373-149">12</span><span class="sxs-lookup"><span data-stu-id="b1373-149">12</span></span>|<span data-ttu-id="b1373-150">iSocConsumer。</span><span class="sxs-lookup"><span data-stu-id="b1373-150">iSocConsumer.</span></span>|
|<span data-ttu-id="b1373-151">unix</span><span class="sxs-lookup"><span data-stu-id="b1373-151">unix</span></span>|<span data-ttu-id="b1373-152">13</span><span class="sxs-lookup"><span data-stu-id="b1373-152">13</span></span>|<span data-ttu-id="b1373-153">Unix。</span><span class="sxs-lookup"><span data-stu-id="b1373-153">Unix.</span></span>|
|<span data-ttu-id="b1373-154">macMDM</span><span class="sxs-lookup"><span data-stu-id="b1373-154">macMDM</span></span>|<span data-ttu-id="b1373-155">14</span><span class="sxs-lookup"><span data-stu-id="b1373-155">14</span></span>|<span data-ttu-id="b1373-156">Mac OS X 客户端使用内置 MDM 代理。</span><span class="sxs-lookup"><span data-stu-id="b1373-156">Mac OS X client using built in MDM agent.</span></span>|
|<span data-ttu-id="b1373-157">holoLens</span><span class="sxs-lookup"><span data-stu-id="b1373-157">holoLens</span></span>|<span data-ttu-id="b1373-158">15</span><span class="sxs-lookup"><span data-stu-id="b1373-158">15</span></span>|<span data-ttu-id="b1373-159">表示花哨 goggles Windows 10。</span><span class="sxs-lookup"><span data-stu-id="b1373-159">Representing the fancy Windows 10 goggles.</span></span>|
|<span data-ttu-id="b1373-160">surfaceHub</span><span class="sxs-lookup"><span data-stu-id="b1373-160">surfaceHub</span></span>|<span data-ttu-id="b1373-161">16</span><span class="sxs-lookup"><span data-stu-id="b1373-161">16</span></span>|<span data-ttu-id="b1373-162">曲面集线器设备。</span><span class="sxs-lookup"><span data-stu-id="b1373-162">Surface HUB device.</span></span>|
|<span data-ttu-id="b1373-163">androidForWork</span><span class="sxs-lookup"><span data-stu-id="b1373-163">androidForWork</span></span>|<span data-ttu-id="b1373-164">17</span><span class="sxs-lookup"><span data-stu-id="b1373-164">17</span></span>|<span data-ttu-id="b1373-165">Android 工作设备。</span><span class="sxs-lookup"><span data-stu-id="b1373-165">Android for work device.</span></span>|
|<span data-ttu-id="b1373-166">androidEnterprise</span><span class="sxs-lookup"><span data-stu-id="b1373-166">androidEnterprise</span></span>|<span data-ttu-id="b1373-167">18</span><span class="sxs-lookup"><span data-stu-id="b1373-167">18</span></span>|<span data-ttu-id="b1373-168">Android 企业设备。</span><span class="sxs-lookup"><span data-stu-id="b1373-168">Android enterprise device.</span></span>|
|<span data-ttu-id="b1373-169">blackberry</span><span class="sxs-lookup"><span data-stu-id="b1373-169">blackberry</span></span>|<span data-ttu-id="b1373-170">100</span><span class="sxs-lookup"><span data-stu-id="b1373-170">100</span></span>|<span data-ttu-id="b1373-171">Blackberry。</span><span class="sxs-lookup"><span data-stu-id="b1373-171">Blackberry.</span></span>|
|<span data-ttu-id="b1373-172">棕榈</span><span class="sxs-lookup"><span data-stu-id="b1373-172">palm</span></span>|<span data-ttu-id="b1373-173">101</span><span class="sxs-lookup"><span data-stu-id="b1373-173">101</span></span>|<span data-ttu-id="b1373-174">棕榈。</span><span class="sxs-lookup"><span data-stu-id="b1373-174">Palm.</span></span>|
|<span data-ttu-id="b1373-175">unknown</span><span class="sxs-lookup"><span data-stu-id="b1373-175">unknown</span></span>|<span data-ttu-id="b1373-176">255</span><span class="sxs-lookup"><span data-stu-id="b1373-176">255</span></span>|<span data-ttu-id="b1373-177">表示的设备类型是未知。</span><span class="sxs-lookup"><span data-stu-id="b1373-177">Represents that the device type is unknown.</span></span>|




