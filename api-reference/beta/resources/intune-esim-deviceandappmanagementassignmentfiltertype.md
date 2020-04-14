---
title: deviceAndAppManagementAssignmentFilterType 枚举类型
description: 表示工作分配筛选器的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 4e1febcc506de1248f519be5cd1c2d40fca9dc15
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358100"
---
# <a name="deviceandappmanagementassignmentfiltertype-enum-type"></a><span data-ttu-id="ec4c0-103">deviceAndAppManagementAssignmentFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ec4c0-103">deviceAndAppManagementAssignmentFilterType enum type</span></span>

<span data-ttu-id="ec4c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ec4c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ec4c0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec4c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec4c0-107">表示工作分配筛选器的类型。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-107">Represents type of the assignment filter.</span></span>

## <a name="members"></a><span data-ttu-id="ec4c0-108">成员</span><span class="sxs-lookup"><span data-stu-id="ec4c0-108">Members</span></span>
|<span data-ttu-id="ec4c0-109">成员</span><span class="sxs-lookup"><span data-stu-id="ec4c0-109">Member</span></span>|<span data-ttu-id="ec4c0-110">值</span><span class="sxs-lookup"><span data-stu-id="ec4c0-110">Value</span></span>|<span data-ttu-id="ec4c0-111">说明</span><span class="sxs-lookup"><span data-stu-id="ec4c0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec4c0-112">无</span><span class="sxs-lookup"><span data-stu-id="ec4c0-112">none</span></span>|<span data-ttu-id="ec4c0-113">0</span><span class="sxs-lookup"><span data-stu-id="ec4c0-113">0</span></span>|<span data-ttu-id="ec4c0-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-114">Default value.</span></span> <span data-ttu-id="ec4c0-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-115">Do not use.</span></span>|
|<span data-ttu-id="ec4c0-116">含</span><span class="sxs-lookup"><span data-stu-id="ec4c0-116">include</span></span>|<span data-ttu-id="ec4c0-117">1</span><span class="sxs-lookup"><span data-stu-id="ec4c0-117">1</span></span>|<span data-ttu-id="ec4c0-118">指示筛选器中的规则匹配将向设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-118">Indicates in-filter, rule matching will offer the payload to devices.</span></span>|
|<span data-ttu-id="ec4c0-119">排除</span><span class="sxs-lookup"><span data-stu-id="ec4c0-119">exclude</span></span>|<span data-ttu-id="ec4c0-120">双面</span><span class="sxs-lookup"><span data-stu-id="ec4c0-120">2</span></span>|<span data-ttu-id="ec4c0-121">指示 out 筛选器，规则匹配将不会向设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="ec4c0-121">Indicates out-filter, rule matching will not offer the payload to devices.</span></span>|



