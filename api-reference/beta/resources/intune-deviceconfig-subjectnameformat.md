---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 519558ff2e56b823ac5c889fb8d383f547a61daf
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529362"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="cfe67-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cfe67-103">subjectNameFormat enum type</span></span>

<span data-ttu-id="cfe67-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="cfe67-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cfe67-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cfe67-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cfe67-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cfe67-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cfe67-107">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="cfe67-107">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="cfe67-108">成员</span><span class="sxs-lookup"><span data-stu-id="cfe67-108">Members</span></span>
|<span data-ttu-id="cfe67-109">成员</span><span class="sxs-lookup"><span data-stu-id="cfe67-109">Member</span></span>|<span data-ttu-id="cfe67-110">值</span><span class="sxs-lookup"><span data-stu-id="cfe67-110">Value</span></span>|<span data-ttu-id="cfe67-111">说明</span><span class="sxs-lookup"><span data-stu-id="cfe67-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfe67-112">commonName</span><span class="sxs-lookup"><span data-stu-id="cfe67-112">commonName</span></span>|<span data-ttu-id="cfe67-113">0</span><span class="sxs-lookup"><span data-stu-id="cfe67-113">0</span></span>|<span data-ttu-id="cfe67-114">公用名。</span><span class="sxs-lookup"><span data-stu-id="cfe67-114">Common name.</span></span>|
|<span data-ttu-id="cfe67-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="cfe67-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="cfe67-116">1 </span><span class="sxs-lookup"><span data-stu-id="cfe67-116">1</span></span>|<span data-ttu-id="cfe67-117">公用名称，包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="cfe67-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="cfe67-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="cfe67-118">commonNameAsEmail</span></span>|<span data-ttu-id="cfe67-119">2 </span><span class="sxs-lookup"><span data-stu-id="cfe67-119">2</span></span>|<span data-ttu-id="cfe67-120">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="cfe67-120">Common Name As Email.</span></span>|
|<span data-ttu-id="cfe67-121">自</span><span class="sxs-lookup"><span data-stu-id="cfe67-121">custom</span></span>|<span data-ttu-id="cfe67-122">3 </span><span class="sxs-lookup"><span data-stu-id="cfe67-122">3</span></span>|<span data-ttu-id="cfe67-123">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="cfe67-123">Custom subject name format.</span></span>|
|<span data-ttu-id="cfe67-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="cfe67-124">commonNameAsIMEI</span></span>|<span data-ttu-id="cfe67-125">5 </span><span class="sxs-lookup"><span data-stu-id="cfe67-125">5</span></span>|<span data-ttu-id="cfe67-126">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cfe67-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="cfe67-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="cfe67-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="cfe67-128">6 </span><span class="sxs-lookup"><span data-stu-id="cfe67-128">6</span></span>|<span data-ttu-id="cfe67-129">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cfe67-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cfe67-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="cfe67-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="cfe67-131">7 </span><span class="sxs-lookup"><span data-stu-id="cfe67-131">7</span></span>|<span data-ttu-id="cfe67-132">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cfe67-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cfe67-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="cfe67-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="cfe67-134">8 </span><span class="sxs-lookup"><span data-stu-id="cfe67-134">8</span></span>|<span data-ttu-id="cfe67-135">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cfe67-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="cfe67-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="cfe67-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="cfe67-137">9 </span><span class="sxs-lookup"><span data-stu-id="cfe67-137">9</span></span>|<span data-ttu-id="cfe67-138">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="cfe67-138">Common Name As Serial Number.</span></span>|



