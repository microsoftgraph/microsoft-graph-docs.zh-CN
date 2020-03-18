---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: f785c9bbd3a4d84433e80d686269029e22105e1a
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42787465"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="f188a-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f188a-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="f188a-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f188a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f188a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f188a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f188a-106">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="f188a-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="f188a-107">成员</span><span class="sxs-lookup"><span data-stu-id="f188a-107">Members</span></span>
|<span data-ttu-id="f188a-108">成员</span><span class="sxs-lookup"><span data-stu-id="f188a-108">Member</span></span>|<span data-ttu-id="f188a-109">值</span><span class="sxs-lookup"><span data-stu-id="f188a-109">Value</span></span>|<span data-ttu-id="f188a-110">说明</span><span class="sxs-lookup"><span data-stu-id="f188a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f188a-111">commonName</span><span class="sxs-lookup"><span data-stu-id="f188a-111">commonName</span></span>|<span data-ttu-id="f188a-112">0</span><span class="sxs-lookup"><span data-stu-id="f188a-112">0</span></span>|<span data-ttu-id="f188a-113">公用名。</span><span class="sxs-lookup"><span data-stu-id="f188a-113">Common name.</span></span>|
|<span data-ttu-id="f188a-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="f188a-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="f188a-115">1</span><span class="sxs-lookup"><span data-stu-id="f188a-115">1</span></span>|<span data-ttu-id="f188a-116">公用名称，包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="f188a-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="f188a-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="f188a-117">commonNameAsEmail</span></span>|<span data-ttu-id="f188a-118">双面</span><span class="sxs-lookup"><span data-stu-id="f188a-118">2</span></span>|<span data-ttu-id="f188a-119">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="f188a-119">Common Name As Email.</span></span>|
|<span data-ttu-id="f188a-120">自</span><span class="sxs-lookup"><span data-stu-id="f188a-120">custom</span></span>|<span data-ttu-id="f188a-121">第三章</span><span class="sxs-lookup"><span data-stu-id="f188a-121">3</span></span>|<span data-ttu-id="f188a-122">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="f188a-122">Custom subject name format.</span></span>|
|<span data-ttu-id="f188a-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="f188a-123">commonNameAsIMEI</span></span>|<span data-ttu-id="f188a-124">5 </span><span class="sxs-lookup"><span data-stu-id="f188a-124">5</span></span>|<span data-ttu-id="f188a-125">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="f188a-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="f188a-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="f188a-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="f188a-127">6 </span><span class="sxs-lookup"><span data-stu-id="f188a-127">6</span></span>|<span data-ttu-id="f188a-128">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="f188a-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="f188a-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="f188a-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="f188a-130">7 </span><span class="sxs-lookup"><span data-stu-id="f188a-130">7</span></span>|<span data-ttu-id="f188a-131">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="f188a-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="f188a-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="f188a-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="f188a-133">8 </span><span class="sxs-lookup"><span data-stu-id="f188a-133">8</span></span>|<span data-ttu-id="f188a-134">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="f188a-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="f188a-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="f188a-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="f188a-136">9 </span><span class="sxs-lookup"><span data-stu-id="f188a-136">9</span></span>|<span data-ttu-id="f188a-137">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="f188a-137">Common Name As Serial Number.</span></span>|



