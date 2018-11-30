---
title: subjectNameFormat 枚举类型
description: 使用者名称格式选项。
ms.openlocfilehash: 7299558011c471f02e5c1149da6ac23183faa150
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041641"
---
# <a name="subjectnameformat-enum-type"></a><span data-ttu-id="997a4-103">subjectNameFormat 枚举类型</span><span class="sxs-lookup"><span data-stu-id="997a4-103">subjectNameFormat enum type</span></span>

> <span data-ttu-id="997a4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="997a4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="997a4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="997a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="997a4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="997a4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="997a4-107">使用者名称格式选项。</span><span class="sxs-lookup"><span data-stu-id="997a4-107">Subject Name Format Options.</span></span>
## <a name="members"></a><span data-ttu-id="997a4-108">成员</span><span class="sxs-lookup"><span data-stu-id="997a4-108">Members</span></span>
|<span data-ttu-id="997a4-109">成员</span><span class="sxs-lookup"><span data-stu-id="997a4-109">Member</span></span>|<span data-ttu-id="997a4-110">值</span><span class="sxs-lookup"><span data-stu-id="997a4-110">Value</span></span>|<span data-ttu-id="997a4-111">说明</span><span class="sxs-lookup"><span data-stu-id="997a4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="997a4-112">commonName</span><span class="sxs-lookup"><span data-stu-id="997a4-112">commonName</span></span>|<span data-ttu-id="997a4-113">0</span><span class="sxs-lookup"><span data-stu-id="997a4-113">0</span></span>|<span data-ttu-id="997a4-114">公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-114">Common name.</span></span>|
|<span data-ttu-id="997a4-115">commonNameIncludingEmail</span><span class="sxs-lookup"><span data-stu-id="997a4-115">commonNameIncludingEmail</span></span>|<span data-ttu-id="997a4-116">1</span><span class="sxs-lookup"><span data-stu-id="997a4-116">1</span></span>|<span data-ttu-id="997a4-117">包括电子邮件的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-117">Common Name Including Email.</span></span>|
|<span data-ttu-id="997a4-118">commonNameAsEmail</span><span class="sxs-lookup"><span data-stu-id="997a4-118">commonNameAsEmail</span></span>|<span data-ttu-id="997a4-119">2</span><span class="sxs-lookup"><span data-stu-id="997a4-119">2</span></span>|<span data-ttu-id="997a4-120">作为电子邮件的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-120">Common Name As Email.</span></span>|
|<span data-ttu-id="997a4-121">自定义</span><span class="sxs-lookup"><span data-stu-id="997a4-121">custom</span></span>|<span data-ttu-id="997a4-122">3</span><span class="sxs-lookup"><span data-stu-id="997a4-122">3</span></span>|<span data-ttu-id="997a4-123">自定义主题名称格式。</span><span class="sxs-lookup"><span data-stu-id="997a4-123">Custom subject name format.</span></span>|
|<span data-ttu-id="997a4-124">commonNameAsIMEI</span><span class="sxs-lookup"><span data-stu-id="997a4-124">commonNameAsIMEI</span></span>|<span data-ttu-id="997a4-125">5</span><span class="sxs-lookup"><span data-stu-id="997a4-125">5</span></span>|<span data-ttu-id="997a4-126">作为 IMEI 的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-126">Common Name As IMEI.</span></span>|
|<span data-ttu-id="997a4-127">commonNameAsSerialNumber</span><span class="sxs-lookup"><span data-stu-id="997a4-127">commonNameAsSerialNumber</span></span>|<span data-ttu-id="997a4-128">6</span><span class="sxs-lookup"><span data-stu-id="997a4-128">6</span></span>|<span data-ttu-id="997a4-129">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-129">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="997a4-130">commonNameAsAadDeviceId</span><span class="sxs-lookup"><span data-stu-id="997a4-130">commonNameAsAadDeviceId</span></span>|<span data-ttu-id="997a4-131">7</span><span class="sxs-lookup"><span data-stu-id="997a4-131">7</span></span>|<span data-ttu-id="997a4-132">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-132">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="997a4-133">commonNameAsIntuneDeviceId</span><span class="sxs-lookup"><span data-stu-id="997a4-133">commonNameAsIntuneDeviceId</span></span>|<span data-ttu-id="997a4-134">8</span><span class="sxs-lookup"><span data-stu-id="997a4-134">8</span></span>|<span data-ttu-id="997a4-135">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-135">Common Name As Serial Number.</span></span>|
|<span data-ttu-id="997a4-136">commonNameAsDurableDeviceId</span><span class="sxs-lookup"><span data-stu-id="997a4-136">commonNameAsDurableDeviceId</span></span>|<span data-ttu-id="997a4-137">9</span><span class="sxs-lookup"><span data-stu-id="997a4-137">9</span></span>|<span data-ttu-id="997a4-138">序列号作为的公用名。</span><span class="sxs-lookup"><span data-stu-id="997a4-138">Common Name As Serial Number.</span></span>|





