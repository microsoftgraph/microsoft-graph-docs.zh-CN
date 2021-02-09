---
title: deviceAndAppManagementAssignmentFilterType 枚举类型
description: 表示工作分配筛选器的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6a2b9f9e2f01cb4ca7d5a0f1a1d51d00e985369c
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155858"
---
# <a name="deviceandappmanagementassignmentfiltertype-enum-type"></a><span data-ttu-id="2100b-103">deviceAndAppManagementAssignmentFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="2100b-103">deviceAndAppManagementAssignmentFilterType enum type</span></span>

<span data-ttu-id="2100b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2100b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2100b-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2100b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2100b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2100b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2100b-107">表示工作分配筛选器的类型。</span><span class="sxs-lookup"><span data-stu-id="2100b-107">Represents type of the assignment filter.</span></span>

## <a name="members"></a><span data-ttu-id="2100b-108">成员</span><span class="sxs-lookup"><span data-stu-id="2100b-108">Members</span></span>
|<span data-ttu-id="2100b-109">成员</span><span class="sxs-lookup"><span data-stu-id="2100b-109">Member</span></span>|<span data-ttu-id="2100b-110">值</span><span class="sxs-lookup"><span data-stu-id="2100b-110">Value</span></span>|<span data-ttu-id="2100b-111">说明</span><span class="sxs-lookup"><span data-stu-id="2100b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2100b-112">无</span><span class="sxs-lookup"><span data-stu-id="2100b-112">none</span></span>|<span data-ttu-id="2100b-113">0</span><span class="sxs-lookup"><span data-stu-id="2100b-113">0</span></span>|<span data-ttu-id="2100b-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="2100b-114">Default value.</span></span> <span data-ttu-id="2100b-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="2100b-115">Do not use.</span></span>|
|<span data-ttu-id="2100b-116">include</span><span class="sxs-lookup"><span data-stu-id="2100b-116">include</span></span>|<span data-ttu-id="2100b-117">1 </span><span class="sxs-lookup"><span data-stu-id="2100b-117">1</span></span>|<span data-ttu-id="2100b-118">指示筛选器内规则匹配将为设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="2100b-118">Indicates in-filter, rule matching will offer the payload to devices.</span></span>|
|<span data-ttu-id="2100b-119">exclude</span><span class="sxs-lookup"><span data-stu-id="2100b-119">exclude</span></span>|<span data-ttu-id="2100b-120">2 </span><span class="sxs-lookup"><span data-stu-id="2100b-120">2</span></span>|<span data-ttu-id="2100b-121">指示筛选外，规则匹配不会向设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="2100b-121">Indicates out-filter, rule matching will not offer the payload to devices.</span></span>|




