---
title: groupPolicyMigrationReadiness 枚举类型
description: 指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d860844de50c58deace7f10821ca0b1a4591d00b
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722821"
---
# <a name="grouppolicymigrationreadiness-enum-type"></a><span data-ttu-id="81d4a-103">groupPolicyMigrationReadiness 枚举类型</span><span class="sxs-lookup"><span data-stu-id="81d4a-103">groupPolicyMigrationReadiness enum type</span></span>

<span data-ttu-id="81d4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="81d4a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="81d4a-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="81d4a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81d4a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="81d4a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81d4a-107">指示组策略对象文件是否已被覆盖并准备好进行 Intune 迁移。</span><span class="sxs-lookup"><span data-stu-id="81d4a-107">Indicates if the Group Policy Object file is covered and ready for Intune migration.</span></span>

## <a name="members"></a><span data-ttu-id="81d4a-108">成员</span><span class="sxs-lookup"><span data-stu-id="81d4a-108">Members</span></span>
|<span data-ttu-id="81d4a-109">成员</span><span class="sxs-lookup"><span data-stu-id="81d4a-109">Member</span></span>|<span data-ttu-id="81d4a-110">值</span><span class="sxs-lookup"><span data-stu-id="81d4a-110">Value</span></span>|<span data-ttu-id="81d4a-111">说明</span><span class="sxs-lookup"><span data-stu-id="81d4a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81d4a-112">无</span><span class="sxs-lookup"><span data-stu-id="81d4a-112">none</span></span>|<span data-ttu-id="81d4a-113">1</span><span class="sxs-lookup"><span data-stu-id="81d4a-113">1</span></span>|<span data-ttu-id="81d4a-114">无 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="81d4a-114">No Intune coverage</span></span>|
|<span data-ttu-id="81d4a-115">环</span><span class="sxs-lookup"><span data-stu-id="81d4a-115">partial</span></span>|<span data-ttu-id="81d4a-116">双面</span><span class="sxs-lookup"><span data-stu-id="81d4a-116">2</span></span>|<span data-ttu-id="81d4a-117">部分 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="81d4a-117">Partial Intune coverage</span></span>|
|<span data-ttu-id="81d4a-118">complete</span><span class="sxs-lookup"><span data-stu-id="81d4a-118">complete</span></span>|<span data-ttu-id="81d4a-119">第三章</span><span class="sxs-lookup"><span data-stu-id="81d4a-119">3</span></span>|<span data-ttu-id="81d4a-120">完成 Intune 覆盖范围</span><span class="sxs-lookup"><span data-stu-id="81d4a-120">Complete Intune coverage</span></span>|
|<span data-ttu-id="81d4a-121">error</span><span class="sxs-lookup"><span data-stu-id="81d4a-121">error</span></span>|<span data-ttu-id="81d4a-122">4 </span><span class="sxs-lookup"><span data-stu-id="81d4a-122">4</span></span>|<span data-ttu-id="81d4a-123">分析覆盖率时出错</span><span class="sxs-lookup"><span data-stu-id="81d4a-123">Error when analyzing coverage</span></span>|
|<span data-ttu-id="81d4a-124">notApplicable</span><span class="sxs-lookup"><span data-stu-id="81d4a-124">notApplicable</span></span>|<span data-ttu-id="81d4a-125">5 </span><span class="sxs-lookup"><span data-stu-id="81d4a-125">5</span></span>|<span data-ttu-id="81d4a-126">GPO 中没有组策略设置</span><span class="sxs-lookup"><span data-stu-id="81d4a-126">No Group Policy settings in GPO</span></span>|





