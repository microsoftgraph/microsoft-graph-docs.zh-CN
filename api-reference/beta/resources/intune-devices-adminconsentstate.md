---
title: adminConsentState 枚举类型
description: 管理员同意状态。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 31ad2e2cbec6accdb7d1f9ced4dc152510b2289f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27964240"
---
# <a name="adminconsentstate-enum-type"></a><span data-ttu-id="989d0-103">adminConsentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="989d0-103">adminConsentState enum type</span></span>

> <span data-ttu-id="989d0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="989d0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="989d0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="989d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="989d0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="989d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="989d0-107">管理员同意状态。</span><span class="sxs-lookup"><span data-stu-id="989d0-107">Admin consent state.</span></span>
## <a name="members"></a><span data-ttu-id="989d0-108">成员</span><span class="sxs-lookup"><span data-stu-id="989d0-108">Members</span></span>
|<span data-ttu-id="989d0-109">成员</span><span class="sxs-lookup"><span data-stu-id="989d0-109">Member</span></span>|<span data-ttu-id="989d0-110">值</span><span class="sxs-lookup"><span data-stu-id="989d0-110">Value</span></span>|<span data-ttu-id="989d0-111">Description</span><span class="sxs-lookup"><span data-stu-id="989d0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="989d0-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="989d0-112">notConfigured</span></span>|<span data-ttu-id="989d0-113">0</span><span class="sxs-lookup"><span data-stu-id="989d0-113">0</span></span>|<span data-ttu-id="989d0-114">管理未配置项目</span><span class="sxs-lookup"><span data-stu-id="989d0-114">Admin did not configure the item</span></span>|
|<span data-ttu-id="989d0-115">授予</span><span class="sxs-lookup"><span data-stu-id="989d0-115">granted</span></span>|<span data-ttu-id="989d0-116">1</span><span class="sxs-lookup"><span data-stu-id="989d0-116">1</span></span>|<span data-ttu-id="989d0-117">管理员授予项目</span><span class="sxs-lookup"><span data-stu-id="989d0-117">Admin granted item</span></span>|
|<span data-ttu-id="989d0-118">带来</span><span class="sxs-lookup"><span data-stu-id="989d0-118">notGranted</span></span>|<span data-ttu-id="989d0-119">2</span><span class="sxs-lookup"><span data-stu-id="989d0-119">2</span></span>|<span data-ttu-id="989d0-120">管理 deos 不会授予对项目</span><span class="sxs-lookup"><span data-stu-id="989d0-120">Admin deos not grant item</span></span>|





