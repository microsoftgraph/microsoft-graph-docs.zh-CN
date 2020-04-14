---
title: subjectNameFormat 枚举类型
description: 主题名称格式选项。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 68c48ebff2e65832997bc6685bdae58c29bc5a37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43412690"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="22159-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="22159-103">subjectNameFormat enum type</span></span>

<span data-ttu-id="22159-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="22159-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="22159-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="22159-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="22159-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="22159-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22159-107">主题名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="22159-107">Subject Name Format Options.</span></span>

## <a name="members"></a><span data-ttu-id="22159-108">成员</span><span class="sxs-lookup"><span data-stu-id="22159-108">Members</span></span>
|<span data-ttu-id="22159-109">成员</span><span class="sxs-lookup"><span data-stu-id="22159-109">Member</span></span>|<span data-ttu-id="22159-110">值</span><span class="sxs-lookup"><span data-stu-id="22159-110">Value</span></span>|<span data-ttu-id="22159-111">说明</span><span class="sxs-lookup"><span data-stu-id="22159-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22159-112">commonName</span><span class="sxs-lookup"><span data-stu-id="22159-112">commonName</span></span>|<span data-ttu-id="22159-113">0</span><span class="sxs-lookup"><span data-stu-id="22159-113">0</span></span>|<span data-ttu-id="22159-114">公用名。</span><span class="sxs-lookup"><span data-stu-id="22159-114">Common name.</span></span>|
|<span data-ttu-id="22159-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="22159-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="22159-116">1</span><span class="sxs-lookup"><span data-stu-id="22159-116">1</span></span>|<span data-ttu-id="22159-117">公用名称，包括电子邮件。</span><span class="sxs-lookup"><span data-stu-id="22159-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="22159-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="22159-118">commonNameAsEmail</span></span>|<span data-ttu-id="22159-119">双面</span><span class="sxs-lookup"><span data-stu-id="22159-119">2</span></span>|<span data-ttu-id="22159-120">电子邮件的常见名称。</span><span class="sxs-lookup"><span data-stu-id="22159-120">Common Name As Email.</span></span>|
|<span data-ttu-id="22159-121">自</span><span class="sxs-lookup"><span data-stu-id="22159-121">custom</span></span>|<span data-ttu-id="22159-122">第三章</span><span class="sxs-lookup"><span data-stu-id="22159-122">3</span></span>|<span data-ttu-id="22159-123">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="22159-123">Custom subject name format.</span></span>|
|<span data-ttu-id="22159-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="22159-124">commonNameAsIMEI</span></span>|<span data-ttu-id="22159-125">5 </span><span class="sxs-lookup"><span data-stu-id="22159-125">5</span></span>|<span data-ttu-id="22159-126">作为 IMEI 的常用名称。</span><span class="sxs-lookup"><span data-stu-id="22159-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="22159-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="22159-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="22159-128">6 </span><span class="sxs-lookup"><span data-stu-id="22159-128">6</span></span>|<span data-ttu-id="22159-129">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="22159-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="22159-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="22159-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="22159-131">7 </span><span class="sxs-lookup"><span data-stu-id="22159-131">7</span></span>|<span data-ttu-id="22159-132">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="22159-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="22159-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="22159-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="22159-134">8 </span><span class="sxs-lookup"><span data-stu-id="22159-134">8</span></span>|<span data-ttu-id="22159-135">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="22159-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="22159-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="22159-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="22159-137">9 </span><span class="sxs-lookup"><span data-stu-id="22159-137">9</span></span>|<span data-ttu-id="22159-138">作为序列号的常用名称。</span><span class="sxs-lookup"><span data-stu-id="22159-138">Common Name As Serial Number.</span></span>|



