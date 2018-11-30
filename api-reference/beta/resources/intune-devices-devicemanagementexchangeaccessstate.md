---
title: deviceManagementExchangeAccessState 枚举类型
description: 设备 Exchange 访问状态。
ms.openlocfilehash: e075f3c52dc09d2c762552d3c6580d419f0616f8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044653"
---
# <a name="devicemanagementexchangeaccessstate-enum-type"></a><span data-ttu-id="c42ab-103">deviceManagementExchangeAccessState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c42ab-103">deviceManagementExchangeAccessState enum type</span></span>

> <span data-ttu-id="c42ab-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c42ab-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c42ab-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c42ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c42ab-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c42ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c42ab-107">设备 Exchange 访问状态。</span><span class="sxs-lookup"><span data-stu-id="c42ab-107">Device Exchange Access State.</span></span>
## <a name="members"></a><span data-ttu-id="c42ab-108">成员</span><span class="sxs-lookup"><span data-stu-id="c42ab-108">Members</span></span>
|<span data-ttu-id="c42ab-109">成员</span><span class="sxs-lookup"><span data-stu-id="c42ab-109">Member</span></span>|<span data-ttu-id="c42ab-110">值</span><span class="sxs-lookup"><span data-stu-id="c42ab-110">Value</span></span>|<span data-ttu-id="c42ab-111">说明</span><span class="sxs-lookup"><span data-stu-id="c42ab-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c42ab-112">无</span><span class="sxs-lookup"><span data-stu-id="c42ab-112">none</span></span>|<span data-ttu-id="c42ab-113">0</span><span class="sxs-lookup"><span data-stu-id="c42ab-113">0</span></span>|<span data-ttu-id="c42ab-114">从 Exchange 发现没有访问状态</span><span class="sxs-lookup"><span data-stu-id="c42ab-114">No access state discovered from Exchange</span></span>|
|<span data-ttu-id="c42ab-115">unknown</span><span class="sxs-lookup"><span data-stu-id="c42ab-115">unknown</span></span>|<span data-ttu-id="c42ab-116">1</span><span class="sxs-lookup"><span data-stu-id="c42ab-116">1</span></span>|<span data-ttu-id="c42ab-117">到 Exchange 的设备访问状态是未知</span><span class="sxs-lookup"><span data-stu-id="c42ab-117">Device access state to Exchange is unknown</span></span>|
|<span data-ttu-id="c42ab-118">允许</span><span class="sxs-lookup"><span data-stu-id="c42ab-118">allowed</span></span>|<span data-ttu-id="c42ab-119">2</span><span class="sxs-lookup"><span data-stu-id="c42ab-119">2</span></span>|<span data-ttu-id="c42ab-120">设备有权访问 Exchange</span><span class="sxs-lookup"><span data-stu-id="c42ab-120">Device has access to Exchange</span></span>|
|<span data-ttu-id="c42ab-121">已阻止</span><span class="sxs-lookup"><span data-stu-id="c42ab-121">blocked</span></span>|<span data-ttu-id="c42ab-122">3</span><span class="sxs-lookup"><span data-stu-id="c42ab-122">3</span></span>|<span data-ttu-id="c42ab-123">设备在 Exchange 中被阻止</span><span class="sxs-lookup"><span data-stu-id="c42ab-123">Device is Blocked in Exchange</span></span>|
|<span data-ttu-id="c42ab-124">隔离</span><span class="sxs-lookup"><span data-stu-id="c42ab-124">quarantined</span></span>|<span data-ttu-id="c42ab-125">4</span><span class="sxs-lookup"><span data-stu-id="c42ab-125">4</span></span>|<span data-ttu-id="c42ab-126">在 Exchange 隔离设备</span><span class="sxs-lookup"><span data-stu-id="c42ab-126">Device is Quarantined in Exchange</span></span>|





