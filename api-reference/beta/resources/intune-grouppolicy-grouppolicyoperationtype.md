---
title: groupPolicyOperationType 枚举类型
description: 组策略操作的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 3319ddb45c59a829b3275b889aa54a4f8ec4bb8b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49259653"
---
# <a name="grouppolicyoperationtype-enum-type"></a><span data-ttu-id="5f6bc-103">groupPolicyOperationType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5f6bc-103">groupPolicyOperationType enum type</span></span>

<span data-ttu-id="5f6bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f6bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f6bc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f6bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f6bc-107">组策略操作的类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-107">Type of Group Policy operation.</span></span>

## <a name="members"></a><span data-ttu-id="5f6bc-108">成员</span><span class="sxs-lookup"><span data-stu-id="5f6bc-108">Members</span></span>
|<span data-ttu-id="5f6bc-109">成员</span><span class="sxs-lookup"><span data-stu-id="5f6bc-109">Member</span></span>|<span data-ttu-id="5f6bc-110">值</span><span class="sxs-lookup"><span data-stu-id="5f6bc-110">Value</span></span>|<span data-ttu-id="5f6bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f6bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f6bc-112">无</span><span class="sxs-lookup"><span data-stu-id="5f6bc-112">none</span></span>|<span data-ttu-id="5f6bc-113">0</span><span class="sxs-lookup"><span data-stu-id="5f6bc-113">0</span></span>|<span data-ttu-id="5f6bc-114">组策略操作类型无效。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-114">Group Policy invalid operation type.</span></span>|
|<span data-ttu-id="5f6bc-115">[</span><span class="sxs-lookup"><span data-stu-id="5f6bc-115">upload</span></span>|<span data-ttu-id="5f6bc-116">1</span><span class="sxs-lookup"><span data-stu-id="5f6bc-116">1</span></span>|<span data-ttu-id="5f6bc-117">组策略上载操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-117">Group Policy upload operation type.</span></span>|
|<span data-ttu-id="5f6bc-118">uploadNewVersion</span><span class="sxs-lookup"><span data-stu-id="5f6bc-118">uploadNewVersion</span></span>|<span data-ttu-id="5f6bc-119">双面</span><span class="sxs-lookup"><span data-stu-id="5f6bc-119">2</span></span>|<span data-ttu-id="5f6bc-120">组策略上载新版本操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-120">Group Policy upload new version operation type.</span></span>|
|<span data-ttu-id="5f6bc-121">addLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="5f6bc-121">addLanguageFiles</span></span>|<span data-ttu-id="5f6bc-122">第三章</span><span class="sxs-lookup"><span data-stu-id="5f6bc-122">3</span></span>|<span data-ttu-id="5f6bc-123">组策略添加新语言 (ADML) 文件操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-123">Group Policy add new language(ADML) files operation type.</span></span>|
|<span data-ttu-id="5f6bc-124">removeLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="5f6bc-124">removeLanguageFiles</span></span>|<span data-ttu-id="5f6bc-125">4 </span><span class="sxs-lookup"><span data-stu-id="5f6bc-125">4</span></span>|<span data-ttu-id="5f6bc-126">组策略删除语言 (ADML) 文件操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-126">Group Policy remove language(ADML) files operation type.</span></span>|
|<span data-ttu-id="5f6bc-127">updateLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="5f6bc-127">updateLanguageFiles</span></span>|<span data-ttu-id="5f6bc-128">5 </span><span class="sxs-lookup"><span data-stu-id="5f6bc-128">5</span></span>|<span data-ttu-id="5f6bc-129">组策略更新语言 (ADML) 文件操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-129">Group Policy update language(ADML) files operation type.</span></span>|
|<span data-ttu-id="5f6bc-130">删除</span><span class="sxs-lookup"><span data-stu-id="5f6bc-130">remove</span></span>|<span data-ttu-id="5f6bc-131">6 </span><span class="sxs-lookup"><span data-stu-id="5f6bc-131">6</span></span>|<span data-ttu-id="5f6bc-132">组策略删除上载的文件操作类型。</span><span class="sxs-lookup"><span data-stu-id="5f6bc-132">Group Policy remove uploaded file operation type.</span></span>|




