---
title: deviceManagementReportStatus 枚举类型
description: 与生成的报告相关联的可能状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: eb85ade317129c1bae790dff43b42d5c839d45d6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49287674"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="b07ef-103">deviceManagementReportStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b07ef-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="b07ef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b07ef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b07ef-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b07ef-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b07ef-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b07ef-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b07ef-107">与生成的报告相关联的可能状态</span><span class="sxs-lookup"><span data-stu-id="b07ef-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="b07ef-108">成员</span><span class="sxs-lookup"><span data-stu-id="b07ef-108">Members</span></span>
|<span data-ttu-id="b07ef-109">成员</span><span class="sxs-lookup"><span data-stu-id="b07ef-109">Member</span></span>|<span data-ttu-id="b07ef-110">值</span><span class="sxs-lookup"><span data-stu-id="b07ef-110">Value</span></span>|<span data-ttu-id="b07ef-111">Description</span><span class="sxs-lookup"><span data-stu-id="b07ef-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b07ef-112">unknown</span><span class="sxs-lookup"><span data-stu-id="b07ef-112">unknown</span></span>|<span data-ttu-id="b07ef-113">0</span><span class="sxs-lookup"><span data-stu-id="b07ef-113">0</span></span>|<span data-ttu-id="b07ef-114">报告生成状态未知</span><span class="sxs-lookup"><span data-stu-id="b07ef-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="b07ef-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="b07ef-115">notStarted</span></span>|<span data-ttu-id="b07ef-116">1</span><span class="sxs-lookup"><span data-stu-id="b07ef-116">1</span></span>|<span data-ttu-id="b07ef-117">尚未开始报告生成</span><span class="sxs-lookup"><span data-stu-id="b07ef-117">Report generation has not started</span></span>|
|<span data-ttu-id="b07ef-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="b07ef-118">inProgress</span></span>|<span data-ttu-id="b07ef-119">双面</span><span class="sxs-lookup"><span data-stu-id="b07ef-119">2</span></span>|<span data-ttu-id="b07ef-120">正在生成报告</span><span class="sxs-lookup"><span data-stu-id="b07ef-120">Report generation is in progress</span></span>|
|<span data-ttu-id="b07ef-121">后</span><span class="sxs-lookup"><span data-stu-id="b07ef-121">completed</span></span>|<span data-ttu-id="b07ef-122">第三章</span><span class="sxs-lookup"><span data-stu-id="b07ef-122">3</span></span>|<span data-ttu-id="b07ef-123">报告生成已完成</span><span class="sxs-lookup"><span data-stu-id="b07ef-123">Report generation is completed</span></span>|
|<span data-ttu-id="b07ef-124">未能</span><span class="sxs-lookup"><span data-stu-id="b07ef-124">failed</span></span>|<span data-ttu-id="b07ef-125">4 </span><span class="sxs-lookup"><span data-stu-id="b07ef-125">4</span></span>|<span data-ttu-id="b07ef-126">报告生成失败</span><span class="sxs-lookup"><span data-stu-id="b07ef-126">Report generation has failed</span></span>|




