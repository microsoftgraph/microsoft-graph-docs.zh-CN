---
title: deviceManagementReportStatus 枚举类型
description: 与生成的报告相关联的可能状态
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 9f7ab2225d862dc14d1687e286cc71681988f0f8
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43453192"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="d071b-103">deviceManagementReportStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d071b-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="d071b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d071b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d071b-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d071b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d071b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d071b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d071b-107">与生成的报告相关联的可能状态</span><span class="sxs-lookup"><span data-stu-id="d071b-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="d071b-108">成员</span><span class="sxs-lookup"><span data-stu-id="d071b-108">Members</span></span>
|<span data-ttu-id="d071b-109">成员</span><span class="sxs-lookup"><span data-stu-id="d071b-109">Member</span></span>|<span data-ttu-id="d071b-110">值</span><span class="sxs-lookup"><span data-stu-id="d071b-110">Value</span></span>|<span data-ttu-id="d071b-111">说明</span><span class="sxs-lookup"><span data-stu-id="d071b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d071b-112">unknown</span><span class="sxs-lookup"><span data-stu-id="d071b-112">unknown</span></span>|<span data-ttu-id="d071b-113">0</span><span class="sxs-lookup"><span data-stu-id="d071b-113">0</span></span>|<span data-ttu-id="d071b-114">报告生成状态未知</span><span class="sxs-lookup"><span data-stu-id="d071b-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="d071b-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="d071b-115">notStarted</span></span>|<span data-ttu-id="d071b-116">1</span><span class="sxs-lookup"><span data-stu-id="d071b-116">1</span></span>|<span data-ttu-id="d071b-117">尚未开始报告生成</span><span class="sxs-lookup"><span data-stu-id="d071b-117">Report generation has not started</span></span>|
|<span data-ttu-id="d071b-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="d071b-118">inProgress</span></span>|<span data-ttu-id="d071b-119">双面</span><span class="sxs-lookup"><span data-stu-id="d071b-119">2</span></span>|<span data-ttu-id="d071b-120">正在生成报告</span><span class="sxs-lookup"><span data-stu-id="d071b-120">Report generation is in progress</span></span>|
|<span data-ttu-id="d071b-121">后</span><span class="sxs-lookup"><span data-stu-id="d071b-121">completed</span></span>|<span data-ttu-id="d071b-122">第三章</span><span class="sxs-lookup"><span data-stu-id="d071b-122">3</span></span>|<span data-ttu-id="d071b-123">报告生成已完成</span><span class="sxs-lookup"><span data-stu-id="d071b-123">Report generation is completed</span></span>|
|<span data-ttu-id="d071b-124">未能</span><span class="sxs-lookup"><span data-stu-id="d071b-124">failed</span></span>|<span data-ttu-id="d071b-125">4 </span><span class="sxs-lookup"><span data-stu-id="d071b-125">4</span></span>|<span data-ttu-id="d071b-126">报告生成失败</span><span class="sxs-lookup"><span data-stu-id="d071b-126">Report generation has failed</span></span>|



