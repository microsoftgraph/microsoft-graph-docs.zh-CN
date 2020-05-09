---
title: deviceManagementTemplateSubtype 枚举类型
description: Template 子类型
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 59771a3d456e6330a12d731ec7b13634a9dd9aba
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44177434"
---
# <a name="devicemanagementtemplatesubtype-enum-type"></a><span data-ttu-id="9e998-103">deviceManagementTemplateSubtype 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9e998-103">deviceManagementTemplateSubtype enum type</span></span>

<span data-ttu-id="9e998-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e998-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9e998-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9e998-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9e998-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9e998-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9e998-107">Template 子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-107">Template subtype</span></span>

## <a name="members"></a><span data-ttu-id="9e998-108">成员</span><span class="sxs-lookup"><span data-stu-id="9e998-108">Members</span></span>
|<span data-ttu-id="9e998-109">成员</span><span class="sxs-lookup"><span data-stu-id="9e998-109">Member</span></span>|<span data-ttu-id="9e998-110">值</span><span class="sxs-lookup"><span data-stu-id="9e998-110">Value</span></span>|<span data-ttu-id="9e998-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e998-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e998-112">无</span><span class="sxs-lookup"><span data-stu-id="9e998-112">none</span></span>|<span data-ttu-id="9e998-113">0</span><span class="sxs-lookup"><span data-stu-id="9e998-113">0</span></span>|<span data-ttu-id="9e998-114">模板没有子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-114">Template has no subtype</span></span>|
|<span data-ttu-id="9e998-115">firewall</span><span class="sxs-lookup"><span data-stu-id="9e998-115">firewall</span></span>|<span data-ttu-id="9e998-116">1</span><span class="sxs-lookup"><span data-stu-id="9e998-116">1</span></span>|<span data-ttu-id="9e998-117">终结点安全防火墙子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-117">Endpoint security firewall subtype</span></span>|
|<span data-ttu-id="9e998-118">diskEncryption</span><span class="sxs-lookup"><span data-stu-id="9e998-118">diskEncryption</span></span>|<span data-ttu-id="9e998-119">双面</span><span class="sxs-lookup"><span data-stu-id="9e998-119">2</span></span>|<span data-ttu-id="9e998-120">终结点安全磁盘加密子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-120">Endpoint security disk encryption subtype</span></span>|
|<span data-ttu-id="9e998-121">attackSurfaceReduction</span><span class="sxs-lookup"><span data-stu-id="9e998-121">attackSurfaceReduction</span></span>|<span data-ttu-id="9e998-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9e998-122">3</span></span>|<span data-ttu-id="9e998-123">终结点安全攻击面缩减子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-123">Endpoint security attack surface reduction subtype</span></span>|
|<span data-ttu-id="9e998-124">endpointDetectionReponse</span><span class="sxs-lookup"><span data-stu-id="9e998-124">endpointDetectionReponse</span></span>|<span data-ttu-id="9e998-125">4 </span><span class="sxs-lookup"><span data-stu-id="9e998-125">4</span></span>|<span data-ttu-id="9e998-126">终结点安全终结点检测和响应子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-126">Endpoint security endpoint detection and response subtype</span></span>|
|<span data-ttu-id="9e998-127">accountProtection</span><span class="sxs-lookup"><span data-stu-id="9e998-127">accountProtection</span></span>|<span data-ttu-id="9e998-128">5 </span><span class="sxs-lookup"><span data-stu-id="9e998-128">5</span></span>|<span data-ttu-id="9e998-129">Endpoint security 帐户保护子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-129">Endpoint security account protection subtype</span></span>|
|<span data-ttu-id="9e998-130">程序</span><span class="sxs-lookup"><span data-stu-id="9e998-130">antivirus</span></span>|<span data-ttu-id="9e998-131">6 </span><span class="sxs-lookup"><span data-stu-id="9e998-131">6</span></span>|<span data-ttu-id="9e998-132">Endpoint security anitivirus 子类型</span><span class="sxs-lookup"><span data-stu-id="9e998-132">Endpoint security anitivirus subtype</span></span>|



