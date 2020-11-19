---
title: remediationState 枚举类型
description: 指示设备管理脚本的执行状态的类型。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 90e930d6b8955671abb494839bafe6cac16438f0
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49230875"
---
# <a name="remediationstate-enum-type"></a><span data-ttu-id="7bc3e-103">remediationState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="7bc3e-103">remediationState enum type</span></span>

<span data-ttu-id="7bc3e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7bc3e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7bc3e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7bc3e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7bc3e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7bc3e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7bc3e-107">指示设备管理脚本的执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="7bc3e-107">Indicates the type of execution status of the device management script.</span></span>

## <a name="members"></a><span data-ttu-id="7bc3e-108">成员</span><span class="sxs-lookup"><span data-stu-id="7bc3e-108">Members</span></span>
|<span data-ttu-id="7bc3e-109">成员</span><span class="sxs-lookup"><span data-stu-id="7bc3e-109">Member</span></span>|<span data-ttu-id="7bc3e-110">值</span><span class="sxs-lookup"><span data-stu-id="7bc3e-110">Value</span></span>|<span data-ttu-id="7bc3e-111">说明</span><span class="sxs-lookup"><span data-stu-id="7bc3e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7bc3e-112">unknown</span><span class="sxs-lookup"><span data-stu-id="7bc3e-112">unknown</span></span>|<span data-ttu-id="7bc3e-113">0</span><span class="sxs-lookup"><span data-stu-id="7bc3e-113">0</span></span>|<span data-ttu-id="7bc3e-114">未知结果。</span><span class="sxs-lookup"><span data-stu-id="7bc3e-114">Unknown result.</span></span>|
|<span data-ttu-id="7bc3e-115">跳过</span><span class="sxs-lookup"><span data-stu-id="7bc3e-115">skipped</span></span>|<span data-ttu-id="7bc3e-116">1</span><span class="sxs-lookup"><span data-stu-id="7bc3e-116">1</span></span>|<span data-ttu-id="7bc3e-117">跳过了修正脚本执行</span><span class="sxs-lookup"><span data-stu-id="7bc3e-117">Remediation script execution was skipped</span></span>|
|<span data-ttu-id="7bc3e-118">success</span><span class="sxs-lookup"><span data-stu-id="7bc3e-118">success</span></span>|<span data-ttu-id="7bc3e-119">双面</span><span class="sxs-lookup"><span data-stu-id="7bc3e-119">2</span></span>|<span data-ttu-id="7bc3e-120">已成功执行修正脚本并修正了设备状态</span><span class="sxs-lookup"><span data-stu-id="7bc3e-120">Remediation script executed successfully and remediated the device state</span></span>|
|<span data-ttu-id="7bc3e-121">remediationFailed</span><span class="sxs-lookup"><span data-stu-id="7bc3e-121">remediationFailed</span></span>|<span data-ttu-id="7bc3e-122">第三章</span><span class="sxs-lookup"><span data-stu-id="7bc3e-122">3</span></span>|<span data-ttu-id="7bc3e-123">已成功执行修正脚本，但未能修正设备状态</span><span class="sxs-lookup"><span data-stu-id="7bc3e-123">Remediation script executed successfully but failed to remediated the device state</span></span>|
|<span data-ttu-id="7bc3e-124">scriptError</span><span class="sxs-lookup"><span data-stu-id="7bc3e-124">scriptError</span></span>|<span data-ttu-id="7bc3e-125">4 </span><span class="sxs-lookup"><span data-stu-id="7bc3e-125">4</span></span>|<span data-ttu-id="7bc3e-126">遇到了修正脚本执行和错误或超时</span><span class="sxs-lookup"><span data-stu-id="7bc3e-126">Remediation script execution encountered and error or timed out</span></span>|




