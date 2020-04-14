---
title: adminConsentState 枚举类型
description: 管理员同意状态。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a1bc441a395b0a86a7b74c425dd6ebd82c840fe6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43463441"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="9d9b6-103">adminConsentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9d9b6-103">adminConsentState enum type</span></span>

<span data-ttu-id="9d9b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9d9b6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9d9b6-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9d9b6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9d9b6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9d9b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9d9b6-107">管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="9d9b6-107">Admin consent state.</span></span>

## <a name="members"></a><span data-ttu-id="9d9b6-108">成员</span><span class="sxs-lookup"><span data-stu-id="9d9b6-108">Members</span></span>
|<span data-ttu-id="9d9b6-109">成员</span><span class="sxs-lookup"><span data-stu-id="9d9b6-109">Member</span></span>|<span data-ttu-id="9d9b6-110">值</span><span class="sxs-lookup"><span data-stu-id="9d9b6-110">Value</span></span>|<span data-ttu-id="9d9b6-111">说明</span><span class="sxs-lookup"><span data-stu-id="9d9b6-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9d9b6-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9d9b6-112">notConfigured</span></span>|<span data-ttu-id="9d9b6-113">0</span><span class="sxs-lookup"><span data-stu-id="9d9b6-113">0</span></span>|<span data-ttu-id="9d9b6-114">管理员未配置项目</span><span class="sxs-lookup"><span data-stu-id="9d9b6-114">Admin did not configure the item</span></span>|
|<span data-ttu-id="9d9b6-115">granted</span><span class="sxs-lookup"><span data-stu-id="9d9b6-115">granted</span></span>|<span data-ttu-id="9d9b6-116">1</span><span class="sxs-lookup"><span data-stu-id="9d9b6-116">1</span></span>|<span data-ttu-id="9d9b6-117">管理员授予的项目</span><span class="sxs-lookup"><span data-stu-id="9d9b6-117">Admin granted item</span></span>|
|<span data-ttu-id="9d9b6-118">notGranted</span><span class="sxs-lookup"><span data-stu-id="9d9b6-118">notGranted</span></span>|<span data-ttu-id="9d9b6-119">双面</span><span class="sxs-lookup"><span data-stu-id="9d9b6-119">2</span></span>|<span data-ttu-id="9d9b6-120">Admin deos 不授予项目</span><span class="sxs-lookup"><span data-stu-id="9d9b6-120">Admin deos not grant item</span></span>|



