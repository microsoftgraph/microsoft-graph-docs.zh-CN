---
title: deviceAndAppManagementAssignmentFilterType 枚举类型
description: 表示工作分配筛选器的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 6a2b9f9e2f01cb4ca7d5a0f1a1d51d00e985369c
ms.sourcegitcommit: fe1b4d098af604cc34596f595e799911ea672532
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/07/2021
ms.locfileid: "51611780"
---
# <a name="deviceandappmanagementassignmentfiltertype-enum-type"></a><span data-ttu-id="6be96-103">deviceAndAppManagementAssignmentFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="6be96-103">deviceAndAppManagementAssignmentFilterType enum type</span></span>

<span data-ttu-id="6be96-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6be96-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6be96-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6be96-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6be96-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6be96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6be96-107">表示工作分配筛选器的类型。</span><span class="sxs-lookup"><span data-stu-id="6be96-107">Represents type of the assignment filter.</span></span>

## <a name="members"></a><span data-ttu-id="6be96-108">成员</span><span class="sxs-lookup"><span data-stu-id="6be96-108">Members</span></span>
|<span data-ttu-id="6be96-109">成员</span><span class="sxs-lookup"><span data-stu-id="6be96-109">Member</span></span>|<span data-ttu-id="6be96-110">值</span><span class="sxs-lookup"><span data-stu-id="6be96-110">Value</span></span>|<span data-ttu-id="6be96-111">Description</span><span class="sxs-lookup"><span data-stu-id="6be96-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6be96-112">无</span><span class="sxs-lookup"><span data-stu-id="6be96-112">none</span></span>|<span data-ttu-id="6be96-113">0</span><span class="sxs-lookup"><span data-stu-id="6be96-113">0</span></span>|<span data-ttu-id="6be96-114">默认值。</span><span class="sxs-lookup"><span data-stu-id="6be96-114">Default value.</span></span> <span data-ttu-id="6be96-115">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="6be96-115">Do not use.</span></span>|
|<span data-ttu-id="6be96-116">include</span><span class="sxs-lookup"><span data-stu-id="6be96-116">include</span></span>|<span data-ttu-id="6be96-117">1</span><span class="sxs-lookup"><span data-stu-id="6be96-117">1</span></span>|<span data-ttu-id="6be96-118">指示筛选器内规则匹配将为设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="6be96-118">Indicates in-filter, rule matching will offer the payload to devices.</span></span>|
|<span data-ttu-id="6be96-119">exclude</span><span class="sxs-lookup"><span data-stu-id="6be96-119">exclude</span></span>|<span data-ttu-id="6be96-120">2</span><span class="sxs-lookup"><span data-stu-id="6be96-120">2</span></span>|<span data-ttu-id="6be96-121">指示未筛选，规则匹配不会向设备提供有效负载。</span><span class="sxs-lookup"><span data-stu-id="6be96-121">Indicates out-filter, rule matching will not offer the payload to devices.</span></span>|




