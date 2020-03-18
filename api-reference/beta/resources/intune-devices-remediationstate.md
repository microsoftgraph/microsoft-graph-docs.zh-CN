---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cd940bbe2256baa7954e67ba9469ac00740f4ad1
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42783912"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="21da2-103">remediationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="21da2-103">remediationState enum type</span></span>

> <span data-ttu-id="21da2-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="21da2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="21da2-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="21da2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="21da2-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="21da2-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="21da2-107">成员</span><span class="sxs-lookup"><span data-stu-id="21da2-107">Members</span></span>
|<span data-ttu-id="21da2-108">成员</span><span class="sxs-lookup"><span data-stu-id="21da2-108">Member</span></span>|<span data-ttu-id="21da2-109">值</span><span class="sxs-lookup"><span data-stu-id="21da2-109">Value</span></span>|<span data-ttu-id="21da2-110">说明</span><span class="sxs-lookup"><span data-stu-id="21da2-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="21da2-111">unknown</span><span class="sxs-lookup"><span data-stu-id="21da2-111">unknown</span></span>|<span data-ttu-id="21da2-112">0</span><span class="sxs-lookup"><span data-stu-id="21da2-112">0</span></span>|<span data-ttu-id="21da2-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="21da2-113">Unknown result.</span></span>|
|<span data-ttu-id="21da2-114">跳过</span><span class="sxs-lookup"><span data-stu-id="21da2-114">skipped</span></span>|<span data-ttu-id="21da2-115">1</span><span class="sxs-lookup"><span data-stu-id="21da2-115">1</span></span>|<span data-ttu-id="21da2-116">跳过了修正脚本执行</span><span class="sxs-lookup"><span data-stu-id="21da2-116">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="21da2-117">success</span><span class="sxs-lookup"><span data-stu-id="21da2-117">success</span></span>|<span data-ttu-id="21da2-118">双面</span><span class="sxs-lookup"><span data-stu-id="21da2-118">2</span></span>|<span data-ttu-id="21da2-119">已成功执行修正脚本并修正了设备状态</span><span class="sxs-lookup"><span data-stu-id="21da2-119">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="21da2-120">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="21da2-120">remediationFailed</span></span>|<span data-ttu-id="21da2-121">第三章</span><span class="sxs-lookup"><span data-stu-id="21da2-121">3</span></span>|<span data-ttu-id="21da2-122">已成功执行修正脚本，但未能修正设备状态</span><span class="sxs-lookup"><span data-stu-id="21da2-122">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="21da2-123">scriptError</span><span class="sxs-lookup"><span data-stu-id="21da2-123">scriptError</span></span>|<span data-ttu-id="21da2-124">4 </span><span class="sxs-lookup"><span data-stu-id="21da2-124">4</span></span>|<span data-ttu-id="21da2-125">遇到了修正脚本执行和错误或超时</span><span class="sxs-lookup"><span data-stu-id="21da2-125">Remediation script execution encountered and error or timed out</span></span>|



