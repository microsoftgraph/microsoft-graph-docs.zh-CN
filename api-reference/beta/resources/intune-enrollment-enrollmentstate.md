---
title: enrollmentState 枚举类型
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b71f41d459e3fdb50fd853c62a855b4591a8ca8e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29419105"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="fea84-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fea84-103">enrollmentState enum type</span></span>

> <span data-ttu-id="fea84-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fea84-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fea84-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fea84-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fea84-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fea84-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fea84-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="fea84-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="fea84-108">成员</span><span class="sxs-lookup"><span data-stu-id="fea84-108">Members</span></span>
|<span data-ttu-id="fea84-109">成员</span><span class="sxs-lookup"><span data-stu-id="fea84-109">Member</span></span>|<span data-ttu-id="fea84-110">值</span><span class="sxs-lookup"><span data-stu-id="fea84-110">Value</span></span>|<span data-ttu-id="fea84-111">说明</span><span class="sxs-lookup"><span data-stu-id="fea84-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fea84-112">unknown</span><span class="sxs-lookup"><span data-stu-id="fea84-112">unknown</span></span>|<span data-ttu-id="fea84-113">0</span><span class="sxs-lookup"><span data-stu-id="fea84-113">0</span></span>|<span data-ttu-id="fea84-114">设备注册状态是未知</span><span class="sxs-lookup"><span data-stu-id="fea84-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="fea84-115">注册</span><span class="sxs-lookup"><span data-stu-id="fea84-115">enrolled</span></span>|<span data-ttu-id="fea84-116">1</span><span class="sxs-lookup"><span data-stu-id="fea84-116">1</span></span>|<span data-ttu-id="fea84-117">注册设备。</span><span class="sxs-lookup"><span data-stu-id="fea84-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="fea84-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="fea84-118">pendingReset</span></span>|<span data-ttu-id="fea84-119">2</span><span class="sxs-lookup"><span data-stu-id="fea84-119">2</span></span>|<span data-ttu-id="fea84-120">注册但它通过注册配置文件中注册的注册的配置文件是不同的已分配的配置文件。</span><span class="sxs-lookup"><span data-stu-id="fea84-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="fea84-121">failed</span><span class="sxs-lookup"><span data-stu-id="fea84-121">failed</span></span>|<span data-ttu-id="fea84-122">3</span><span class="sxs-lookup"><span data-stu-id="fea84-122">3</span></span>|<span data-ttu-id="fea84-123">未注册，并且没有注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="fea84-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="fea84-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="fea84-124">notContacted</span></span>|<span data-ttu-id="fea84-125">4</span><span class="sxs-lookup"><span data-stu-id="fea84-125">4</span></span>|<span data-ttu-id="fea84-126">导入但未注册设备。</span><span class="sxs-lookup"><span data-stu-id="fea84-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="fea84-127">已阻止</span><span class="sxs-lookup"><span data-stu-id="fea84-127">blocked</span></span>|<span data-ttu-id="fea84-128">5</span><span class="sxs-lookup"><span data-stu-id="fea84-128">5</span></span>|<span data-ttu-id="fea84-129">设备注册为 userless，但阻止移动到用户注册，因为应用程序安装失败。</span><span class="sxs-lookup"><span data-stu-id="fea84-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




