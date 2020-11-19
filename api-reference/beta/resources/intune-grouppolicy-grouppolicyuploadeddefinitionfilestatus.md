---
title: groupPolicyUploadedDefinitionFileStatus 枚举类型
description: 组策略上载的定义文件状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6afafd9f6e35d248b69c3b7ddbb24c20e60d0eeb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298083"
---
# <a name="grouppolicyuploadeddefinitionfilestatus-enum-type"></a><span data-ttu-id="9496b-103">groupPolicyUploadedDefinitionFileStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9496b-103">groupPolicyUploadedDefinitionFileStatus enum type</span></span>

<span data-ttu-id="9496b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9496b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9496b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9496b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9496b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9496b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9496b-107">组策略上载的定义文件状态的类型。</span><span class="sxs-lookup"><span data-stu-id="9496b-107">Type of Group Policy uploaded definition file status.</span></span>

## <a name="members"></a><span data-ttu-id="9496b-108">成员</span><span class="sxs-lookup"><span data-stu-id="9496b-108">Members</span></span>
|<span data-ttu-id="9496b-109">成员</span><span class="sxs-lookup"><span data-stu-id="9496b-109">Member</span></span>|<span data-ttu-id="9496b-110">值</span><span class="sxs-lookup"><span data-stu-id="9496b-110">Value</span></span>|<span data-ttu-id="9496b-111">Description</span><span class="sxs-lookup"><span data-stu-id="9496b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9496b-112">无</span><span class="sxs-lookup"><span data-stu-id="9496b-112">none</span></span>|<span data-ttu-id="9496b-113">0</span><span class="sxs-lookup"><span data-stu-id="9496b-113">0</span></span>|<span data-ttu-id="9496b-114">组策略上传的定义文件上载状态无效。</span><span class="sxs-lookup"><span data-stu-id="9496b-114">Group Policy uploaded definition file invalid upload status.</span></span>|
|<span data-ttu-id="9496b-115">uploadInProgress</span><span class="sxs-lookup"><span data-stu-id="9496b-115">uploadInProgress</span></span>|<span data-ttu-id="9496b-116">1</span><span class="sxs-lookup"><span data-stu-id="9496b-116">1</span></span>|<span data-ttu-id="9496b-117">组策略上传的定义文件上载正在进行中。</span><span class="sxs-lookup"><span data-stu-id="9496b-117">Group Policy uploaded definition file upload in progress.</span></span>|
|<span data-ttu-id="9496b-118">可用</span><span class="sxs-lookup"><span data-stu-id="9496b-118">available</span></span>|<span data-ttu-id="9496b-119">双面</span><span class="sxs-lookup"><span data-stu-id="9496b-119">2</span></span>|<span data-ttu-id="9496b-120">组策略已上载的定义文件可用。</span><span class="sxs-lookup"><span data-stu-id="9496b-120">Group Policy uploaded definition file available.</span></span>|
|<span data-ttu-id="9496b-121">赋予</span><span class="sxs-lookup"><span data-stu-id="9496b-121">assigned</span></span>|<span data-ttu-id="9496b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9496b-122">3</span></span>|<span data-ttu-id="9496b-123">组策略已上载分配给策略的定义文件。</span><span class="sxs-lookup"><span data-stu-id="9496b-123">Group Policy uploaded definition file assigned to policy.</span></span>|
|<span data-ttu-id="9496b-124">removalInProgress</span><span class="sxs-lookup"><span data-stu-id="9496b-124">removalInProgress</span></span>|<span data-ttu-id="9496b-125">4 </span><span class="sxs-lookup"><span data-stu-id="9496b-125">4</span></span>|<span data-ttu-id="9496b-126">组策略上传的定义文件正在删除。</span><span class="sxs-lookup"><span data-stu-id="9496b-126">Group Policy uploaded definition file removal in progress.</span></span>|
|<span data-ttu-id="9496b-127">uploadFailed</span><span class="sxs-lookup"><span data-stu-id="9496b-127">uploadFailed</span></span>|<span data-ttu-id="9496b-128">5 </span><span class="sxs-lookup"><span data-stu-id="9496b-128">5</span></span>|<span data-ttu-id="9496b-129">组策略上载的定义文件上载失败。</span><span class="sxs-lookup"><span data-stu-id="9496b-129">Group Policy uploaded definition file upload failed.</span></span>|
|<span data-ttu-id="9496b-130">removalFailed</span><span class="sxs-lookup"><span data-stu-id="9496b-130">removalFailed</span></span>|<span data-ttu-id="9496b-131">6 </span><span class="sxs-lookup"><span data-stu-id="9496b-131">6</span></span>|<span data-ttu-id="9496b-132">组策略上传的定义文件删除失败。</span><span class="sxs-lookup"><span data-stu-id="9496b-132">Group Policy uploaded definition file removal failed.</span></span>|




