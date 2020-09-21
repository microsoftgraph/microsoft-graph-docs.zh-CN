---
title: groupPolicyUploadedDefinitionFileStatus 枚举类型
description: 组策略上载的定义文件状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 70430e74d332baf0b1c81a41d2098883688464ea
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030610"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="11acf-103">groupPolicyUploadedDefinitionFileStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="11acf-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="11acf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11acf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11acf-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11acf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11acf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11acf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11acf-107">组策略上载的定义文件状态的类型。</span><span class="sxs-lookup"><span data-stu-id="11acf-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="11acf-108">成员</span><span class="sxs-lookup"><span data-stu-id="11acf-108">Members</span></span>
|<span data-ttu-id="11acf-109">成员</span><span class="sxs-lookup"><span data-stu-id="11acf-109">Member</span></span>|<span data-ttu-id="11acf-110">值</span><span class="sxs-lookup"><span data-stu-id="11acf-110">Value</span></span>|<span data-ttu-id="11acf-111">说明</span><span class="sxs-lookup"><span data-stu-id="11acf-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="11acf-112">无</span><span class="sxs-lookup"><span data-stu-id="11acf-112">none</span></span>|<span data-ttu-id="11acf-113">0</span><span class="sxs-lookup"><span data-stu-id="11acf-113">0</span></span>|<span data-ttu-id="11acf-114">组策略上传的定义文件上载状态无效。</span><span class="sxs-lookup"><span data-stu-id="11acf-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="11acf-115">uploadInProgress</span><span class="sxs-lookup"><span data-stu-id="11acf-115">uploadInProgress</span></span>|<span data-ttu-id="11acf-116">1 </span><span class="sxs-lookup"><span data-stu-id="11acf-116">1</span></span>|<span data-ttu-id="11acf-117">组策略上传的定义文件上载正在进行中。</span><span class="sxs-lookup"><span data-stu-id="11acf-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="11acf-118">可用</span><span class="sxs-lookup"><span data-stu-id="11acf-118">available</span></span>|<span data-ttu-id="11acf-119">2 </span><span class="sxs-lookup"><span data-stu-id="11acf-119">2</span></span>|<span data-ttu-id="11acf-120">组策略已上载的定义文件可用。</span><span class="sxs-lookup"><span data-stu-id="11acf-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="11acf-121">赋予</span><span class="sxs-lookup"><span data-stu-id="11acf-121">assigned</span></span>|<span data-ttu-id="11acf-122">第三章</span><span class="sxs-lookup"><span data-stu-id="11acf-122">3</span></span>|<span data-ttu-id="11acf-123">组策略已上载分配给策略的定义文件。</span><span class="sxs-lookup"><span data-stu-id="11acf-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="11acf-124">removalInProgress</span><span class="sxs-lookup"><span data-stu-id="11acf-124">removalInProgress</span></span>|<span data-ttu-id="11acf-125">4 </span><span class="sxs-lookup"><span data-stu-id="11acf-125">4</span></span>|<span data-ttu-id="11acf-126">组策略上传的定义文件正在删除。</span><span class="sxs-lookup"><span data-stu-id="11acf-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="11acf-127">uploadFailed</span><span class="sxs-lookup"><span data-stu-id="11acf-127">uploadFailed</span></span>|<span data-ttu-id="11acf-128">5 </span><span class="sxs-lookup"><span data-stu-id="11acf-128">5</span></span>|<span data-ttu-id="11acf-129">组策略上载的定义文件上载失败。</span><span class="sxs-lookup"><span data-stu-id="11acf-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="11acf-130">removalFailed</span><span class="sxs-lookup"><span data-stu-id="11acf-130">removalFailed</span></span>|<span data-ttu-id="11acf-131">6 </span><span class="sxs-lookup"><span data-stu-id="11acf-131">6</span></span>|<span data-ttu-id="11acf-132">组策略上传的定义文件删除失败。</span><span class="sxs-lookup"><span data-stu-id="11acf-132">Group Policy uploaded definition file removal failed.</span></span>|






