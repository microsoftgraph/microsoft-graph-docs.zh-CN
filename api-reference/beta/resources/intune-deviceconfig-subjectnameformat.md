---
title: subjectNameFormat 枚举类型
description: 使用者名称格式选项。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 85a11e8690c360e405df2453229a039ea9f9b1dd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821334"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="521c6-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="521c6-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="521c6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="521c6-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="521c6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="521c6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="521c6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="521c6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="521c6-107">使用者名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="521c6-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="521c6-108">成员</span><span class="sxs-lookup"><span data-stu-id="521c6-108">Members</span></span>
|<span data-ttu-id="521c6-109">成员</span><span class="sxs-lookup"><span data-stu-id="521c6-109">Member</span></span>|<span data-ttu-id="521c6-110">值</span><span class="sxs-lookup"><span data-stu-id="521c6-110">Value</span></span>|<span data-ttu-id="521c6-111">Description</span><span class="sxs-lookup"><span data-stu-id="521c6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="521c6-112">commonName</span><span class="sxs-lookup"><span data-stu-id="521c6-112">commonName</span></span>|<span data-ttu-id="521c6-113">0</span><span class="sxs-lookup"><span data-stu-id="521c6-113">0</span></span>|<span data-ttu-id="521c6-114">公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-114">Common name.</span></span>|
|<span data-ttu-id="521c6-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="521c6-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="521c6-116">1</span><span class="sxs-lookup"><span data-stu-id="521c6-116">1</span></span>|<span data-ttu-id="521c6-117">包括电子邮件的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="521c6-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="521c6-118">commonNameAsEmail</span></span>|<span data-ttu-id="521c6-119">2</span><span class="sxs-lookup"><span data-stu-id="521c6-119">2</span></span>|<span data-ttu-id="521c6-120">作为电子邮件的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-120">Common Name As Email.</span></span>|
|<span data-ttu-id="521c6-121">自定义</span><span class="sxs-lookup"><span data-stu-id="521c6-121">custom</span></span>|<span data-ttu-id="521c6-122">3</span><span class="sxs-lookup"><span data-stu-id="521c6-122">3</span></span>|<span data-ttu-id="521c6-123">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="521c6-123">Custom subject name format.</span></span>|
|<span data-ttu-id="521c6-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="521c6-124">commonNameAsIMEI</span></span>|<span data-ttu-id="521c6-125">5</span><span class="sxs-lookup"><span data-stu-id="521c6-125">5</span></span>|<span data-ttu-id="521c6-126">作为 IMEI 的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="521c6-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="521c6-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="521c6-128">6</span><span class="sxs-lookup"><span data-stu-id="521c6-128">6</span></span>|<span data-ttu-id="521c6-129">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="521c6-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="521c6-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="521c6-131">7</span><span class="sxs-lookup"><span data-stu-id="521c6-131">7</span></span>|<span data-ttu-id="521c6-132">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="521c6-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="521c6-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="521c6-134">8</span><span class="sxs-lookup"><span data-stu-id="521c6-134">8</span></span>|<span data-ttu-id="521c6-135">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="521c6-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="521c6-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="521c6-137">9</span><span class="sxs-lookup"><span data-stu-id="521c6-137">9</span></span>|<span data-ttu-id="521c6-138">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="521c6-138">Common Name As Serial Number.</span></span>|





