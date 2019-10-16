---
title: deviceManagementReportStatus 枚举类型
description: 与生成的报告相关联的可能状态
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: bbc348dc8b95d03f6811815efda293e68a695ea2
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539034"
---
# <a name="devicemanagementreportstatus-enum-type"></a><span data-ttu-id="a27f6-103">deviceManagementReportStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a27f6-103">deviceManagementReportStatus enum type</span></span>

> <span data-ttu-id="a27f6-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a27f6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a27f6-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a27f6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a27f6-106">与生成的报告相关联的可能状态</span><span class="sxs-lookup"><span data-stu-id="a27f6-106">Possible statuses associated with a generated report</span></span>

## <a name="members"></a><span data-ttu-id="a27f6-107">成员</span><span class="sxs-lookup"><span data-stu-id="a27f6-107">Members</span></span>
|<span data-ttu-id="a27f6-108">成员</span><span class="sxs-lookup"><span data-stu-id="a27f6-108">Member</span></span>|<span data-ttu-id="a27f6-109">值</span><span class="sxs-lookup"><span data-stu-id="a27f6-109">Value</span></span>|<span data-ttu-id="a27f6-110">说明</span><span class="sxs-lookup"><span data-stu-id="a27f6-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a27f6-111">unknown</span><span class="sxs-lookup"><span data-stu-id="a27f6-111">unknown</span></span>|<span data-ttu-id="a27f6-112">0</span><span class="sxs-lookup"><span data-stu-id="a27f6-112">0</span></span>|<span data-ttu-id="a27f6-113">报告生成状态未知</span><span class="sxs-lookup"><span data-stu-id="a27f6-113">Report generation status is unknown</span></span>|
|<span data-ttu-id="a27f6-114">notStarted</span><span class="sxs-lookup"><span data-stu-id="a27f6-114">notStarted</span></span>|<span data-ttu-id="a27f6-115">1</span><span class="sxs-lookup"><span data-stu-id="a27f6-115">1</span></span>|<span data-ttu-id="a27f6-116">尚未开始报告生成</span><span class="sxs-lookup"><span data-stu-id="a27f6-116">Report generation has not started</span></span>|
|<span data-ttu-id="a27f6-117">inProgress</span><span class="sxs-lookup"><span data-stu-id="a27f6-117">inProgress</span></span>|<span data-ttu-id="a27f6-118">双面</span><span class="sxs-lookup"><span data-stu-id="a27f6-118">2</span></span>|<span data-ttu-id="a27f6-119">正在生成报告</span><span class="sxs-lookup"><span data-stu-id="a27f6-119">Report generation is in progress</span></span>|
|<span data-ttu-id="a27f6-120">后</span><span class="sxs-lookup"><span data-stu-id="a27f6-120">completed</span></span>|<span data-ttu-id="a27f6-121">第三章</span><span class="sxs-lookup"><span data-stu-id="a27f6-121">3</span></span>|<span data-ttu-id="a27f6-122">报告生成已完成</span><span class="sxs-lookup"><span data-stu-id="a27f6-122">Report generation is completed</span></span>|
|<span data-ttu-id="a27f6-123">未能</span><span class="sxs-lookup"><span data-stu-id="a27f6-123">failed</span></span>|<span data-ttu-id="a27f6-124">4 </span><span class="sxs-lookup"><span data-stu-id="a27f6-124">4</span></span>|<span data-ttu-id="a27f6-125">报告生成失败</span><span class="sxs-lookup"><span data-stu-id="a27f6-125">Report generation has failed</span></span>|



