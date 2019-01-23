---
title: sharedPCAllowedAccountType 枚举类型
description: 允许共享 PC 的帐户的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1f3948cd149e8779cc06d2d24bfaa6119fcb08ae
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399302"
---
# <a name="sharedpcallowedaccounttype-enum-type"></a><span data-ttu-id="d585e-103">sharedPCAllowedAccountType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d585e-103">sharedPCAllowedAccountType enum type</span></span>

> <span data-ttu-id="d585e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="d585e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d585e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d585e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d585e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d585e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d585e-107">允许共享 PC 的帐户的类型。</span><span class="sxs-lookup"><span data-stu-id="d585e-107">Type of accounts that are allowed to share the PC.</span></span>

## <a name="members"></a><span data-ttu-id="d585e-108">成员</span><span class="sxs-lookup"><span data-stu-id="d585e-108">Members</span></span>
|<span data-ttu-id="d585e-109">成员</span><span class="sxs-lookup"><span data-stu-id="d585e-109">Member</span></span>|<span data-ttu-id="d585e-110">值</span><span class="sxs-lookup"><span data-stu-id="d585e-110">Value</span></span>|<span data-ttu-id="d585e-111">说明</span><span class="sxs-lookup"><span data-stu-id="d585e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d585e-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="d585e-112">notConfigured</span></span>|<span data-ttu-id="d585e-113">0</span><span class="sxs-lookup"><span data-stu-id="d585e-113">0</span></span>|<span data-ttu-id="d585e-114">未配置。</span><span class="sxs-lookup"><span data-stu-id="d585e-114">Not configured.</span></span> <span data-ttu-id="d585e-115">默认值。</span><span class="sxs-lookup"><span data-stu-id="d585e-115">Default value.</span></span>|
|<span data-ttu-id="d585e-116">来宾</span><span class="sxs-lookup"><span data-stu-id="d585e-116">guest</span></span>|<span data-ttu-id="d585e-117">1</span><span class="sxs-lookup"><span data-stu-id="d585e-117">1</span></span>|<span data-ttu-id="d585e-118">仅来宾帐户。</span><span class="sxs-lookup"><span data-stu-id="d585e-118">Only guest accounts.</span></span>|
|<span data-ttu-id="d585e-119">domain</span><span class="sxs-lookup"><span data-stu-id="d585e-119">domain</span></span>|<span data-ttu-id="d585e-120">2</span><span class="sxs-lookup"><span data-stu-id="d585e-120">2</span></span>|<span data-ttu-id="d585e-121">只能加入域的帐户。</span><span class="sxs-lookup"><span data-stu-id="d585e-121">Only domain-joined accounts.</span></span>|




