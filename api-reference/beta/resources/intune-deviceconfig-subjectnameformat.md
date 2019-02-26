---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6f12068576ff78d74f2e1b6119a2030ff7835a7d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158553"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="d4aea-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d4aea-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="d4aea-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4aea-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4aea-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4aea-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4aea-106">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="d4aea-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="d4aea-107">成员</span><span class="sxs-lookup"><span data-stu-id="d4aea-107">Members</span></span>
|<span data-ttu-id="d4aea-108">成员</span><span class="sxs-lookup"><span data-stu-id="d4aea-108">Member</span></span>|<span data-ttu-id="d4aea-109">值</span><span class="sxs-lookup"><span data-stu-id="d4aea-109">Value</span></span>|<span data-ttu-id="d4aea-110">说明</span><span class="sxs-lookup"><span data-stu-id="d4aea-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4aea-111">commonName</span><span class="sxs-lookup"><span data-stu-id="d4aea-111">commonName</span></span>|<span data-ttu-id="d4aea-112">0</span><span class="sxs-lookup"><span data-stu-id="d4aea-112">0</span></span>|<span data-ttu-id="d4aea-113">公用名。</span><span class="sxs-lookup"><span data-stu-id="d4aea-113">Common name.</span></span>|
|<span data-ttu-id="d4aea-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="d4aea-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="d4aea-115">1</span><span class="sxs-lookup"><span data-stu-id="d4aea-115">1</span></span>|<span data-ttu-id="d4aea-116">公用名称, 包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="d4aea-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="d4aea-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="d4aea-117">commonNameAsEmail</span></span>|<span data-ttu-id="d4aea-118">双面</span><span class="sxs-lookup"><span data-stu-id="d4aea-118">2</span></span>|<span data-ttu-id="d4aea-119">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="d4aea-119">Common Name As Email.</span></span>|
|<span data-ttu-id="d4aea-120">自定义</span><span class="sxs-lookup"><span data-stu-id="d4aea-120">custom</span></span>|<span data-ttu-id="d4aea-121">第三章</span><span class="sxs-lookup"><span data-stu-id="d4aea-121">3</span></span>|<span data-ttu-id="d4aea-122">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="d4aea-122">Custom subject name format.</span></span>|
|<span data-ttu-id="d4aea-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="d4aea-123">commonNameAsIMEI</span></span>|<span data-ttu-id="d4aea-124">5</span><span class="sxs-lookup"><span data-stu-id="d4aea-124">5</span></span>|<span data-ttu-id="d4aea-125">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="d4aea-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="d4aea-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="d4aea-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="d4aea-127">型</span><span class="sxs-lookup"><span data-stu-id="d4aea-127">6</span></span>|<span data-ttu-id="d4aea-128">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="d4aea-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="d4aea-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="d4aea-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="d4aea-130">步</span><span class="sxs-lookup"><span data-stu-id="d4aea-130">7</span></span>|<span data-ttu-id="d4aea-131">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="d4aea-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="d4aea-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="d4aea-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="d4aea-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="d4aea-133">8</span></span>|<span data-ttu-id="d4aea-134">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="d4aea-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="d4aea-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="d4aea-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="d4aea-136">第</span><span class="sxs-lookup"><span data-stu-id="d4aea-136">9</span></span>|<span data-ttu-id="d4aea-137">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="d4aea-137">Common Name As Serial Number.</span></span>|




