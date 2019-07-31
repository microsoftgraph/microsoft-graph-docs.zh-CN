---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f6a86028f9f024156431b8f6e126eaf5ddadcd6d
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35969623"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="cdd22-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cdd22-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="cdd22-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cdd22-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cdd22-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cdd22-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cdd22-106">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="cdd22-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="cdd22-107">成员</span><span class="sxs-lookup"><span data-stu-id="cdd22-107">Members</span></span>
|<span data-ttu-id="cdd22-108">成员</span><span class="sxs-lookup"><span data-stu-id="cdd22-108">Member</span></span>|<span data-ttu-id="cdd22-109">值</span><span class="sxs-lookup"><span data-stu-id="cdd22-109">Value</span></span>|<span data-ttu-id="cdd22-110">说明</span><span class="sxs-lookup"><span data-stu-id="cdd22-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cdd22-111">commonName</span><span class="sxs-lookup"><span data-stu-id="cdd22-111">commonName</span></span>|<span data-ttu-id="cdd22-112">0</span><span class="sxs-lookup"><span data-stu-id="cdd22-112">0</span></span>|<span data-ttu-id="cdd22-113">公用名。</span><span class="sxs-lookup"><span data-stu-id="cdd22-113">Common name.</span></span>|
|<span data-ttu-id="cdd22-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="cdd22-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="cdd22-115">1</span><span class="sxs-lookup"><span data-stu-id="cdd22-115">1</span></span>|<span data-ttu-id="cdd22-116">公用名称, 包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cdd22-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="cdd22-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="cdd22-117">commonNameAsEmail</span></span>|<span data-ttu-id="cdd22-118">双面</span><span class="sxs-lookup"><span data-stu-id="cdd22-118">2</span></span>|<span data-ttu-id="cdd22-119">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="cdd22-119">Common Name As Email.</span></span>|
|<span data-ttu-id="cdd22-120">自</span><span class="sxs-lookup"><span data-stu-id="cdd22-120">custom</span></span>|<span data-ttu-id="cdd22-121">第三章</span><span class="sxs-lookup"><span data-stu-id="cdd22-121">3</span></span>|<span data-ttu-id="cdd22-122">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="cdd22-122">Custom subject name format.</span></span>|
|<span data-ttu-id="cdd22-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="cdd22-123">commonNameAsIMEI</span></span>|<span data-ttu-id="cdd22-124">5</span><span class="sxs-lookup"><span data-stu-id="cdd22-124">5</span></span>|<span data-ttu-id="cdd22-125">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdd22-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="cdd22-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="cdd22-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="cdd22-127">型</span><span class="sxs-lookup"><span data-stu-id="cdd22-127">6</span></span>|<span data-ttu-id="cdd22-128">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdd22-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cdd22-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="cdd22-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="cdd22-130">步</span><span class="sxs-lookup"><span data-stu-id="cdd22-130">7</span></span>|<span data-ttu-id="cdd22-131">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdd22-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cdd22-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="cdd22-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="cdd22-133">utf-8</span><span class="sxs-lookup"><span data-stu-id="cdd22-133">8</span></span>|<span data-ttu-id="cdd22-134">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdd22-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cdd22-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="cdd22-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="cdd22-136">第</span><span class="sxs-lookup"><span data-stu-id="cdd22-136">9</span></span>|<span data-ttu-id="cdd22-137">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cdd22-137">Common Name As Serial Number.</span></span>|





