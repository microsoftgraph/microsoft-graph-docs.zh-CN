---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: b359842d7fb266803fdb758d32ca51e6a4b78b97
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37529086"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="143da-103">remediationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="143da-103">remediationState enum type</span></span>

> <span data-ttu-id="143da-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="143da-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="143da-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="143da-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="143da-106">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="143da-106">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="143da-107">成员</span><span class="sxs-lookup"><span data-stu-id="143da-107">Members</span></span>
|<span data-ttu-id="143da-108">成员</span><span class="sxs-lookup"><span data-stu-id="143da-108">Member</span></span>|<span data-ttu-id="143da-109">值</span><span class="sxs-lookup"><span data-stu-id="143da-109">Value</span></span>|<span data-ttu-id="143da-110">说明</span><span class="sxs-lookup"><span data-stu-id="143da-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="143da-111">unknown</span><span class="sxs-lookup"><span data-stu-id="143da-111">unknown</span></span>|<span data-ttu-id="143da-112">0</span><span class="sxs-lookup"><span data-stu-id="143da-112">0</span></span>|<span data-ttu-id="143da-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="143da-113">Unknown result.</span></span>|
|<span data-ttu-id="143da-114">跳过</span><span class="sxs-lookup"><span data-stu-id="143da-114">skipped</span></span>|<span data-ttu-id="143da-115">1</span><span class="sxs-lookup"><span data-stu-id="143da-115">1</span></span>|<span data-ttu-id="143da-116">跳过了修正脚本执行</span><span class="sxs-lookup"><span data-stu-id="143da-116">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="143da-117">success</span><span class="sxs-lookup"><span data-stu-id="143da-117">success</span></span>|<span data-ttu-id="143da-118">双面</span><span class="sxs-lookup"><span data-stu-id="143da-118">2</span></span>|<span data-ttu-id="143da-119">已成功执行修正脚本并修正了设备状态</span><span class="sxs-lookup"><span data-stu-id="143da-119">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="143da-120">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="143da-120">remediationFailed</span></span>|<span data-ttu-id="143da-121">第三章</span><span class="sxs-lookup"><span data-stu-id="143da-121">3</span></span>|<span data-ttu-id="143da-122">已成功执行修正脚本，但未能修正设备状态</span><span class="sxs-lookup"><span data-stu-id="143da-122">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="143da-123">scriptError</span><span class="sxs-lookup"><span data-stu-id="143da-123">scriptError</span></span>|<span data-ttu-id="143da-124">4 </span><span class="sxs-lookup"><span data-stu-id="143da-124">4</span></span>|<span data-ttu-id="143da-125">遇到了修正脚本执行和错误或超时</span><span class="sxs-lookup"><span data-stu-id="143da-125">Remediation script execution encountered and error or timed out</span></span>|



