---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e3f047571f0cd4874c9542fbc1dda7e83dfae4b6
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34964162"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="cdc5d-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cdc5d-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="cdc5d-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdc5d-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdc5d-106">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="cdc5d-107">成员</span><span class="sxs-lookup"><span data-stu-id="cdc5d-107">Members</span></span>
|<span data-ttu-id="cdc5d-108">成员</span><span class="sxs-lookup"><span data-stu-id="cdc5d-108">Member</span></span>|<span data-ttu-id="cdc5d-109">值</span><span class="sxs-lookup"><span data-stu-id="cdc5d-109">Value</span></span>|<span data-ttu-id="cdc5d-110">说明</span><span class="sxs-lookup"><span data-stu-id="cdc5d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdc5d-111">commonName</span><span class="sxs-lookup"><span data-stu-id="cdc5d-111">commonName</span></span>|<span data-ttu-id="cdc5d-112">0</span><span class="sxs-lookup"><span data-stu-id="cdc5d-112">0</span></span>|<span data-ttu-id="cdc5d-113">公用名。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-113">Common name.</span></span>|
|<span data-ttu-id="cdc5d-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="cdc5d-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="cdc5d-115">1</span><span class="sxs-lookup"><span data-stu-id="cdc5d-115">1</span></span>|<span data-ttu-id="cdc5d-116">公用名称, 包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="cdc5d-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="cdc5d-117">commonNameAsEmail</span></span>|<span data-ttu-id="cdc5d-118">双面</span><span class="sxs-lookup"><span data-stu-id="cdc5d-118">2</span></span>|<span data-ttu-id="cdc5d-119">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-119">Common Name As Email.</span></span>|
|<span data-ttu-id="cdc5d-120">自</span><span class="sxs-lookup"><span data-stu-id="cdc5d-120">custom</span></span>|<span data-ttu-id="cdc5d-121">第三章</span><span class="sxs-lookup"><span data-stu-id="cdc5d-121">3</span></span>|<span data-ttu-id="cdc5d-122">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-122">Custom subject name format.</span></span>|
|<span data-ttu-id="cdc5d-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="cdc5d-123">commonNameAsIMEI</span></span>|<span data-ttu-id="cdc5d-124">5</span><span class="sxs-lookup"><span data-stu-id="cdc5d-124">5</span></span>|<span data-ttu-id="cdc5d-125">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="cdc5d-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="cdc5d-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="cdc5d-127">型</span><span class="sxs-lookup"><span data-stu-id="cdc5d-127">6</span></span>|<span data-ttu-id="cdc5d-128">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cdc5d-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="cdc5d-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="cdc5d-130">步</span><span class="sxs-lookup"><span data-stu-id="cdc5d-130">7</span></span>|<span data-ttu-id="cdc5d-131">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cdc5d-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="cdc5d-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="cdc5d-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="cdc5d-133">8</span></span>|<span data-ttu-id="cdc5d-134">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cdc5d-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="cdc5d-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="cdc5d-136">第</span><span class="sxs-lookup"><span data-stu-id="cdc5d-136">9</span></span>|<span data-ttu-id="cdc5d-137">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdc5d-137">Common Name As Serial Number.</span></span>|





