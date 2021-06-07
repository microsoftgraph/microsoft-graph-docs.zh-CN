---
title: deviceManagementReportStatus 枚举类型
description: 与生成的报告关联的可能状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: b448d95d4aa25717e313d92f8b2a4e035228cf1a
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751851"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="c3186-103">deviceManagementReportStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c3186-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="c3186-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3186-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3186-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3186-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3186-106">与生成的报告关联的可能状态</span><span class="sxs-lookup"><span data-stu-id="c3186-106">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="c3186-107">成员</span><span class="sxs-lookup"><span data-stu-id="c3186-107">Members</span></span>
|<span data-ttu-id="c3186-108">成员</span><span class="sxs-lookup"><span data-stu-id="c3186-108">Member</span></span>|<span data-ttu-id="c3186-109">值</span><span class="sxs-lookup"><span data-stu-id="c3186-109">Value</span></span>|<span data-ttu-id="c3186-110">说明</span><span class="sxs-lookup"><span data-stu-id="c3186-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3186-111">unknown</span><span class="sxs-lookup"><span data-stu-id="c3186-111">unknown</span></span>|<span data-ttu-id="c3186-112">0</span><span class="sxs-lookup"><span data-stu-id="c3186-112">0</span></span>|<span data-ttu-id="c3186-113">报告生成状态未知</span><span class="sxs-lookup"><span data-stu-id="c3186-113">Report generation status is unknown</span></span>|
|<span data-ttu-id="c3186-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="c3186-114">notStarted</span></span>|<span data-ttu-id="c3186-115">1</span><span class="sxs-lookup"><span data-stu-id="c3186-115">1</span></span>|<span data-ttu-id="c3186-116">报告生成尚未启动</span><span class="sxs-lookup"><span data-stu-id="c3186-116">Report generation has not started</span></span>|
|<span data-ttu-id="c3186-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="c3186-117">inProgress</span></span>|<span data-ttu-id="c3186-118">2</span><span class="sxs-lookup"><span data-stu-id="c3186-118">2</span></span>|<span data-ttu-id="c3186-119">报告生成正在进行中</span><span class="sxs-lookup"><span data-stu-id="c3186-119">Report generation is in progress</span></span>|
|<span data-ttu-id="c3186-120">已完成</span><span class="sxs-lookup"><span data-stu-id="c3186-120">completed</span></span>|<span data-ttu-id="c3186-121">3</span><span class="sxs-lookup"><span data-stu-id="c3186-121">3</span></span>|<span data-ttu-id="c3186-122">报告生成已完成</span><span class="sxs-lookup"><span data-stu-id="c3186-122">Report generation is completed</span></span>|
|<span data-ttu-id="c3186-123">failed</span><span class="sxs-lookup"><span data-stu-id="c3186-123">failed</span></span>|<span data-ttu-id="c3186-124">4 </span><span class="sxs-lookup"><span data-stu-id="c3186-124">4</span></span>|<span data-ttu-id="c3186-125">报告生成失败</span><span class="sxs-lookup"><span data-stu-id="c3186-125">Report generation has failed</span></span>|




