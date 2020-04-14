---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 5d615df720a99a88077fa593394308ae816c17c1
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43401981"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="e416c-103">remediationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e416c-103">remediationState enum type</span></span>

<span data-ttu-id="e416c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e416c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e416c-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e416c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e416c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e416c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e416c-107">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="e416c-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="e416c-108">成员</span><span class="sxs-lookup"><span data-stu-id="e416c-108">Members</span></span>
|<span data-ttu-id="e416c-109">成员</span><span class="sxs-lookup"><span data-stu-id="e416c-109">Member</span></span>|<span data-ttu-id="e416c-110">值</span><span class="sxs-lookup"><span data-stu-id="e416c-110">Value</span></span>|<span data-ttu-id="e416c-111">说明</span><span class="sxs-lookup"><span data-stu-id="e416c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e416c-112">unknown</span><span class="sxs-lookup"><span data-stu-id="e416c-112">unknown</span></span>|<span data-ttu-id="e416c-113">0</span><span class="sxs-lookup"><span data-stu-id="e416c-113">0</span></span>|<span data-ttu-id="e416c-114">未知结果。</span><span class="sxs-lookup"><span data-stu-id="e416c-114">Unknown result.</span></span>|
|<span data-ttu-id="e416c-115">跳过</span><span class="sxs-lookup"><span data-stu-id="e416c-115">skipped</span></span>|<span data-ttu-id="e416c-116">1</span><span class="sxs-lookup"><span data-stu-id="e416c-116">1</span></span>|<span data-ttu-id="e416c-117">跳过了修正脚本执行</span><span class="sxs-lookup"><span data-stu-id="e416c-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="e416c-118">success</span><span class="sxs-lookup"><span data-stu-id="e416c-118">success</span></span>|<span data-ttu-id="e416c-119">双面</span><span class="sxs-lookup"><span data-stu-id="e416c-119">2</span></span>|<span data-ttu-id="e416c-120">已成功执行修正脚本并修正了设备状态</span><span class="sxs-lookup"><span data-stu-id="e416c-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="e416c-121">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="e416c-121">remediationFailed</span></span>|<span data-ttu-id="e416c-122">第三章</span><span class="sxs-lookup"><span data-stu-id="e416c-122">3</span></span>|<span data-ttu-id="e416c-123">已成功执行修正脚本，但未能修正设备状态</span><span class="sxs-lookup"><span data-stu-id="e416c-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="e416c-124">scriptError</span><span class="sxs-lookup"><span data-stu-id="e416c-124">scriptError</span></span>|<span data-ttu-id="e416c-125">4 </span><span class="sxs-lookup"><span data-stu-id="e416c-125">4</span></span>|<span data-ttu-id="e416c-126">遇到了修正脚本执行和错误或超时</span><span class="sxs-lookup"><span data-stu-id="e416c-126">Remediation script execution encountered and error or timed out</span></span>|



