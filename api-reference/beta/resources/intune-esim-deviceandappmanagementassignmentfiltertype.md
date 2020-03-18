---
title: deviceAndAppManagementAssignmentFilterType 枚举类型
description: 表示工作分配筛选器的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 29b79504dd327d70bec6d973cd08a3f265fb1ab1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783324"
---
# <a name="deviceandappmanagementassignmentfiltertype-enum-type"></a><span data-ttu-id="d82a8-103">deviceAndAppManagementAssignmentFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d82a8-103">deviceAndAppManagementAssignmentFilterType enum type</span></span>

> <span data-ttu-id="d82a8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d82a8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d82a8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d82a8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d82a8-106">表示工作分配筛选器的类型。</span><span class="sxs-lookup"><span data-stu-id="d82a8-106">Represents type of the assignment filter.</span></span>

## <a name="members"></a><span data-ttu-id="d82a8-107">成员</span><span class="sxs-lookup"><span data-stu-id="d82a8-107">Members</span></span>
|<span data-ttu-id="d82a8-108">成员</span><span class="sxs-lookup"><span data-stu-id="d82a8-108">Member</span></span>|<span data-ttu-id="d82a8-109">值</span><span class="sxs-lookup"><span data-stu-id="d82a8-109">Value</span></span>|<span data-ttu-id="d82a8-110">说明</span><span class="sxs-lookup"><span data-stu-id="d82a8-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d82a8-111">无</span><span class="sxs-lookup"><span data-stu-id="d82a8-111">none</span></span>|<span data-ttu-id="d82a8-112">0</span><span class="sxs-lookup"><span data-stu-id="d82a8-112">0</span></span>|<span data-ttu-id="d82a8-113">默认值。</span><span class="sxs-lookup"><span data-stu-id="d82a8-113">Default value.</span></span> <span data-ttu-id="d82a8-114">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="d82a8-114">Do not use.</span></span>|
|<span data-ttu-id="d82a8-115">含</span><span class="sxs-lookup"><span data-stu-id="d82a8-115">include</span></span>|<span data-ttu-id="d82a8-116">1</span><span class="sxs-lookup"><span data-stu-id="d82a8-116">1</span></span>|<span data-ttu-id="d82a8-117">指示筛选器中的规则匹配将向设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="d82a8-117">Indicates in-filter, rule matching will offer the payload to devices.</span></span>|
|<span data-ttu-id="d82a8-118">排除</span><span class="sxs-lookup"><span data-stu-id="d82a8-118">exclude</span></span>|<span data-ttu-id="d82a8-119">双面</span><span class="sxs-lookup"><span data-stu-id="d82a8-119">2</span></span>|<span data-ttu-id="d82a8-120">指示 out 筛选器，规则匹配将不会向设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="d82a8-120">Indicates out-filter, rule matching will not offer the payload to devices.</span></span>|



