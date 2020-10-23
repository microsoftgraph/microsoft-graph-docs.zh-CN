---
title: deviceManagementTemplateSubtype 枚举类型
description: Template 子类型
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 4ed25a4700e28c3b1824b4b76d760343ced48774
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48734201"
---
# <a name="devicemanagementtemplatesubtype-enum-type"></a><span data-ttu-id="a7914-103">deviceManagementTemplateSubtype 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a7914-103">deviceManagementTemplateSubtype enum type</span></span>

<span data-ttu-id="a7914-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7914-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a7914-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a7914-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a7914-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a7914-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a7914-107">Template 子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-107">Template subtype</span></span>

## <a name="members"></a><span data-ttu-id="a7914-108">成员</span><span class="sxs-lookup"><span data-stu-id="a7914-108">Members</span></span>
|<span data-ttu-id="a7914-109">成员</span><span class="sxs-lookup"><span data-stu-id="a7914-109">Member</span></span>|<span data-ttu-id="a7914-110">值</span><span class="sxs-lookup"><span data-stu-id="a7914-110">Value</span></span>|<span data-ttu-id="a7914-111">说明</span><span class="sxs-lookup"><span data-stu-id="a7914-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7914-112">无</span><span class="sxs-lookup"><span data-stu-id="a7914-112">none</span></span>|<span data-ttu-id="a7914-113">0</span><span class="sxs-lookup"><span data-stu-id="a7914-113">0</span></span>|<span data-ttu-id="a7914-114">模板没有子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-114">Template has no subtype</span></span>|
|<span data-ttu-id="a7914-115">firewall</span><span class="sxs-lookup"><span data-stu-id="a7914-115">firewall</span></span>|<span data-ttu-id="a7914-116">1</span><span class="sxs-lookup"><span data-stu-id="a7914-116">1</span></span>|<span data-ttu-id="a7914-117">终结点安全防火墙子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-117">Endpoint security firewall subtype</span></span>|
|<span data-ttu-id="a7914-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="a7914-118">diskEncryption</span></span>|<span data-ttu-id="a7914-119">双面</span><span class="sxs-lookup"><span data-stu-id="a7914-119">2</span></span>|<span data-ttu-id="a7914-120">终结点安全磁盘加密子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-120">Endpoint security disk encryption subtype</span></span>|
|<span data-ttu-id="a7914-121">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="a7914-121">attackSurfaceReduction</span></span>|<span data-ttu-id="a7914-122">第三章</span><span class="sxs-lookup"><span data-stu-id="a7914-122">3</span></span>|<span data-ttu-id="a7914-123">终结点安全攻击面缩减子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-123">Endpoint security attack surface reduction subtype</span></span>|
|<span data-ttu-id="a7914-124">endpointDetectionReponse</span><span class="sxs-lookup"><span data-stu-id="a7914-124">endpointDetectionReponse</span></span>|<span data-ttu-id="a7914-125">4 </span><span class="sxs-lookup"><span data-stu-id="a7914-125">4</span></span>|<span data-ttu-id="a7914-126">终结点安全终结点检测和响应子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-126">Endpoint security endpoint detection and response subtype</span></span>|
|<span data-ttu-id="a7914-127">accountProtection</span><span class="sxs-lookup"><span data-stu-id="a7914-127">accountProtection</span></span>|<span data-ttu-id="a7914-128">5 </span><span class="sxs-lookup"><span data-stu-id="a7914-128">5</span></span>|<span data-ttu-id="a7914-129">Endpoint security 帐户保护子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-129">Endpoint security account protection subtype</span></span>|
|<span data-ttu-id="a7914-130">程序</span><span class="sxs-lookup"><span data-stu-id="a7914-130">antivirus</span></span>|<span data-ttu-id="a7914-131">6 </span><span class="sxs-lookup"><span data-stu-id="a7914-131">6</span></span>|<span data-ttu-id="a7914-132">Endpoint security anitivirus 子类型</span><span class="sxs-lookup"><span data-stu-id="a7914-132">Endpoint security anitivirus subtype</span></span>|





