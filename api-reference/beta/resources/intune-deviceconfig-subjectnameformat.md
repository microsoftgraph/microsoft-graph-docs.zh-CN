---
title: subjectNameFormat 枚举类型
description: 使用者名称格式选项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 22bbc03da6fd3e48925634704e78ffb22abef3bc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410327"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="84968-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="84968-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="84968-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="84968-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="84968-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="84968-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84968-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84968-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84968-107">使用者名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="84968-107">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="84968-108">成员</span><span class="sxs-lookup"><span data-stu-id="84968-108">Members</span></span>
|<span data-ttu-id="84968-109">成员</span><span class="sxs-lookup"><span data-stu-id="84968-109">Member</span></span>|<span data-ttu-id="84968-110">值</span><span class="sxs-lookup"><span data-stu-id="84968-110">Value</span></span>|<span data-ttu-id="84968-111">说明</span><span class="sxs-lookup"><span data-stu-id="84968-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84968-112">commonName</span><span class="sxs-lookup"><span data-stu-id="84968-112">commonName</span></span>|<span data-ttu-id="84968-113">0</span><span class="sxs-lookup"><span data-stu-id="84968-113">0</span></span>|<span data-ttu-id="84968-114">公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-114">Common name.</span></span>|
|<span data-ttu-id="84968-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="84968-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="84968-116">1</span><span class="sxs-lookup"><span data-stu-id="84968-116">1</span></span>|<span data-ttu-id="84968-117">包括电子邮件的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="84968-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="84968-118">commonNameAsEmail</span></span>|<span data-ttu-id="84968-119">2</span><span class="sxs-lookup"><span data-stu-id="84968-119">2</span></span>|<span data-ttu-id="84968-120">作为电子邮件的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-120">Common Name As Email.</span></span>|
|<span data-ttu-id="84968-121">自定义</span><span class="sxs-lookup"><span data-stu-id="84968-121">custom</span></span>|<span data-ttu-id="84968-122">3</span><span class="sxs-lookup"><span data-stu-id="84968-122">3</span></span>|<span data-ttu-id="84968-123">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="84968-123">Custom subject name format.</span></span>|
|<span data-ttu-id="84968-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="84968-124">commonNameAsIMEI</span></span>|<span data-ttu-id="84968-125">5</span><span class="sxs-lookup"><span data-stu-id="84968-125">5</span></span>|<span data-ttu-id="84968-126">作为 IMEI 的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="84968-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="84968-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="84968-128">6</span><span class="sxs-lookup"><span data-stu-id="84968-128">6</span></span>|<span data-ttu-id="84968-129">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="84968-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="84968-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="84968-131">7</span><span class="sxs-lookup"><span data-stu-id="84968-131">7</span></span>|<span data-ttu-id="84968-132">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="84968-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="84968-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="84968-134">8</span><span class="sxs-lookup"><span data-stu-id="84968-134">8</span></span>|<span data-ttu-id="84968-135">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="84968-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="84968-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="84968-137">9</span><span class="sxs-lookup"><span data-stu-id="84968-137">9</span></span>|<span data-ttu-id="84968-138">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="84968-138">Common Name As Serial Number.</span></span>|




