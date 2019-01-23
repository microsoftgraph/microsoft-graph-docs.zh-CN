---
title: adminConsentState 枚举类型
description: 管理员同意状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be144dae700c1555a3641f821402e90c58c1673c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421891"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="95974-103">adminConsentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="95974-103">adminConsentState enum type</span></span>

> <span data-ttu-id="95974-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="95974-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="95974-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="95974-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="95974-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95974-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95974-107">管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="95974-107">Admin consent state.</span></span>

## <a name="members"></a><span data-ttu-id="95974-108">成员</span><span class="sxs-lookup"><span data-stu-id="95974-108">Members</span></span>
|<span data-ttu-id="95974-109">成员</span><span class="sxs-lookup"><span data-stu-id="95974-109">Member</span></span>|<span data-ttu-id="95974-110">值</span><span class="sxs-lookup"><span data-stu-id="95974-110">Value</span></span>|<span data-ttu-id="95974-111">说明</span><span class="sxs-lookup"><span data-stu-id="95974-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95974-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="95974-112">notConfigured</span></span>|<span data-ttu-id="95974-113">0</span><span class="sxs-lookup"><span data-stu-id="95974-113">0</span></span>|<span data-ttu-id="95974-114">管理未配置项目</span><span class="sxs-lookup"><span data-stu-id="95974-114">Admin did not configure the item</span></span>|
|<span data-ttu-id="95974-115">granted</span><span class="sxs-lookup"><span data-stu-id="95974-115">granted</span></span>|<span data-ttu-id="95974-116">1</span><span class="sxs-lookup"><span data-stu-id="95974-116">1</span></span>|<span data-ttu-id="95974-117">管理员授予项目</span><span class="sxs-lookup"><span data-stu-id="95974-117">Admin granted item</span></span>|
|<span data-ttu-id="95974-118">带来</span><span class="sxs-lookup"><span data-stu-id="95974-118">notGranted</span></span>|<span data-ttu-id="95974-119">2</span><span class="sxs-lookup"><span data-stu-id="95974-119">2</span></span>|<span data-ttu-id="95974-120">管理 deos 不会授予对项目</span><span class="sxs-lookup"><span data-stu-id="95974-120">Admin deos not grant item</span></span>|




