---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6202deb0a225da136216eddbb44818cb3ba3a3c5
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31789729"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="90814-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="90814-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="90814-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="90814-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="90814-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="90814-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90814-106">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="90814-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="90814-107">成员</span><span class="sxs-lookup"><span data-stu-id="90814-107">Members</span></span>
|<span data-ttu-id="90814-108">成员</span><span class="sxs-lookup"><span data-stu-id="90814-108">Member</span></span>|<span data-ttu-id="90814-109">值</span><span class="sxs-lookup"><span data-stu-id="90814-109">Value</span></span>|<span data-ttu-id="90814-110">说明</span><span class="sxs-lookup"><span data-stu-id="90814-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="90814-111">commonName</span><span class="sxs-lookup"><span data-stu-id="90814-111">commonName</span></span>|<span data-ttu-id="90814-112">0</span><span class="sxs-lookup"><span data-stu-id="90814-112">0</span></span>|<span data-ttu-id="90814-113">公用名。</span><span class="sxs-lookup"><span data-stu-id="90814-113">Common name.</span></span>|
|<span data-ttu-id="90814-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="90814-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="90814-115">1</span><span class="sxs-lookup"><span data-stu-id="90814-115">1</span></span>|<span data-ttu-id="90814-116">公用名称, 包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="90814-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="90814-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="90814-117">commonNameAsEmail</span></span>|<span data-ttu-id="90814-118">双面</span><span class="sxs-lookup"><span data-stu-id="90814-118">2</span></span>|<span data-ttu-id="90814-119">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="90814-119">Common Name As Email.</span></span>|
|<span data-ttu-id="90814-120">自</span><span class="sxs-lookup"><span data-stu-id="90814-120">custom</span></span>|<span data-ttu-id="90814-121">第三章</span><span class="sxs-lookup"><span data-stu-id="90814-121">3</span></span>|<span data-ttu-id="90814-122">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="90814-122">Custom subject name format.</span></span>|
|<span data-ttu-id="90814-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="90814-123">commonNameAsIMEI</span></span>|<span data-ttu-id="90814-124">5</span><span class="sxs-lookup"><span data-stu-id="90814-124">5</span></span>|<span data-ttu-id="90814-125">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="90814-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="90814-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="90814-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="90814-127">型</span><span class="sxs-lookup"><span data-stu-id="90814-127">6</span></span>|<span data-ttu-id="90814-128">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="90814-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="90814-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="90814-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="90814-130">步</span><span class="sxs-lookup"><span data-stu-id="90814-130">7</span></span>|<span data-ttu-id="90814-131">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="90814-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="90814-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="90814-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="90814-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="90814-133">8</span></span>|<span data-ttu-id="90814-134">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="90814-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="90814-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="90814-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="90814-136">第</span><span class="sxs-lookup"><span data-stu-id="90814-136">9</span></span>|<span data-ttu-id="90814-137">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="90814-137">Common Name As Serial Number.</span></span>|





