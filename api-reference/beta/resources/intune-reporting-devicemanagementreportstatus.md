---
title: deviceManagementReportStatus 枚举类型
description: 与生成的报告相关联的可能状态
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: fe2895f73857bb73262aaa9e90894da7e8028d22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48079779"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="9a748-103">deviceManagementReportStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9a748-103">deviceManagementReportStatus enum type</span></span>

<span data-ttu-id="9a748-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9a748-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9a748-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9a748-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9a748-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9a748-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9a748-107">与生成的报告相关联的可能状态</span><span class="sxs-lookup"><span data-stu-id="9a748-107">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="9a748-108">成员</span><span class="sxs-lookup"><span data-stu-id="9a748-108">Members</span></span>
|<span data-ttu-id="9a748-109">成员</span><span class="sxs-lookup"><span data-stu-id="9a748-109">Member</span></span>|<span data-ttu-id="9a748-110">值</span><span class="sxs-lookup"><span data-stu-id="9a748-110">Value</span></span>|<span data-ttu-id="9a748-111">说明</span><span class="sxs-lookup"><span data-stu-id="9a748-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9a748-112">unknown</span><span class="sxs-lookup"><span data-stu-id="9a748-112">unknown</span></span>|<span data-ttu-id="9a748-113">0</span><span class="sxs-lookup"><span data-stu-id="9a748-113">0</span></span>|<span data-ttu-id="9a748-114">报告生成状态未知</span><span class="sxs-lookup"><span data-stu-id="9a748-114">Report generation status is unknown</span></span>|
|<span data-ttu-id="9a748-115">notStarted</span><span class="sxs-lookup"><span data-stu-id="9a748-115">notStarted</span></span>|<span data-ttu-id="9a748-116">1 </span><span class="sxs-lookup"><span data-stu-id="9a748-116">1</span></span>|<span data-ttu-id="9a748-117">尚未开始报告生成</span><span class="sxs-lookup"><span data-stu-id="9a748-117">Report generation has not started</span></span>|
|<span data-ttu-id="9a748-118">inProgress</span><span class="sxs-lookup"><span data-stu-id="9a748-118">inProgress</span></span>|<span data-ttu-id="9a748-119">2 </span><span class="sxs-lookup"><span data-stu-id="9a748-119">2</span></span>|<span data-ttu-id="9a748-120">正在生成报告</span><span class="sxs-lookup"><span data-stu-id="9a748-120">Report generation is in progress</span></span>|
|<span data-ttu-id="9a748-121">后</span><span class="sxs-lookup"><span data-stu-id="9a748-121">completed</span></span>|<span data-ttu-id="9a748-122">第三章</span><span class="sxs-lookup"><span data-stu-id="9a748-122">3</span></span>|<span data-ttu-id="9a748-123">报告生成已完成</span><span class="sxs-lookup"><span data-stu-id="9a748-123">Report generation is completed</span></span>|
|<span data-ttu-id="9a748-124">未能</span><span class="sxs-lookup"><span data-stu-id="9a748-124">failed</span></span>|<span data-ttu-id="9a748-125">4 </span><span class="sxs-lookup"><span data-stu-id="9a748-125">4</span></span>|<span data-ttu-id="9a748-126">报告生成失败</span><span class="sxs-lookup"><span data-stu-id="9a748-126">Report generation has failed</span></span>|






