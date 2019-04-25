---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6202deb0a225da136216eddbb44818cb3ba3a3c5
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548675"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="44c07-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="44c07-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="44c07-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="44c07-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="44c07-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="44c07-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="44c07-106">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="44c07-106">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="44c07-107">成员</span><span class="sxs-lookup"><span data-stu-id="44c07-107">Members</span></span>
|<span data-ttu-id="44c07-108">成员</span><span class="sxs-lookup"><span data-stu-id="44c07-108">Member</span></span>|<span data-ttu-id="44c07-109">值</span><span class="sxs-lookup"><span data-stu-id="44c07-109">Value</span></span>|<span data-ttu-id="44c07-110">说明</span><span class="sxs-lookup"><span data-stu-id="44c07-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="44c07-111">commonName</span><span class="sxs-lookup"><span data-stu-id="44c07-111">commonName</span></span>|<span data-ttu-id="44c07-112">0</span><span class="sxs-lookup"><span data-stu-id="44c07-112">0</span></span>|<span data-ttu-id="44c07-113">公用名。</span><span class="sxs-lookup"><span data-stu-id="44c07-113">Common name.</span></span>|
|<span data-ttu-id="44c07-114">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="44c07-114">commonNameIncludingEmail</span></span>|<span data-ttu-id="44c07-115">1</span><span class="sxs-lookup"><span data-stu-id="44c07-115">1</span></span>|<span data-ttu-id="44c07-116">公用名称, 包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="44c07-116">Common Name Including Email.</span></span>|
|<span data-ttu-id="44c07-117">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="44c07-117">commonNameAsEmail</span></span>|<span data-ttu-id="44c07-118">2 </span><span class="sxs-lookup"><span data-stu-id="44c07-118">2</span></span>|<span data-ttu-id="44c07-119">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="44c07-119">Common Name As Email.</span></span>|
|<span data-ttu-id="44c07-120">自</span><span class="sxs-lookup"><span data-stu-id="44c07-120">custom</span></span>|<span data-ttu-id="44c07-121">3 </span><span class="sxs-lookup"><span data-stu-id="44c07-121">3</span></span>|<span data-ttu-id="44c07-122">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="44c07-122">Custom subject name format.</span></span>|
|<span data-ttu-id="44c07-123">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="44c07-123">commonNameAsIMEI</span></span>|<span data-ttu-id="44c07-124">5 </span><span class="sxs-lookup"><span data-stu-id="44c07-124">5</span></span>|<span data-ttu-id="44c07-125">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="44c07-125">Common Name As IMEI.</span></span>|
|<span data-ttu-id="44c07-126">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="44c07-126">commonNameAsSerialNumber</span></span>|<span data-ttu-id="44c07-127">6 </span><span class="sxs-lookup"><span data-stu-id="44c07-127">6</span></span>|<span data-ttu-id="44c07-128">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="44c07-128">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="44c07-129">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="44c07-129">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="44c07-130">7 </span><span class="sxs-lookup"><span data-stu-id="44c07-130">7</span></span>|<span data-ttu-id="44c07-131">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="44c07-131">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="44c07-132">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="44c07-132">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="44c07-133">8 </span><span class="sxs-lookup"><span data-stu-id="44c07-133">8</span></span>|<span data-ttu-id="44c07-134">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="44c07-134">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="44c07-135">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="44c07-135">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="44c07-136">9 </span><span class="sxs-lookup"><span data-stu-id="44c07-136">9</span></span>|<span data-ttu-id="44c07-137">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="44c07-137">Common Name As Serial Number.</span></span>|





