---
title: enrollmentState 枚举类型
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: 53b0ccc5f4605d888a056c8093e7d286441bc244
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756427"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="e3844-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e3844-103">enrollmentState enum type</span></span>

<span data-ttu-id="e3844-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e3844-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e3844-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e3844-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3844-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e3844-106">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="e3844-107">成员</span><span class="sxs-lookup"><span data-stu-id="e3844-107">Members</span></span>
|<span data-ttu-id="e3844-108">成员</span><span class="sxs-lookup"><span data-stu-id="e3844-108">Member</span></span>|<span data-ttu-id="e3844-109">值</span><span class="sxs-lookup"><span data-stu-id="e3844-109">Value</span></span>|<span data-ttu-id="e3844-110">说明</span><span class="sxs-lookup"><span data-stu-id="e3844-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3844-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e3844-111">unknown</span></span>|<span data-ttu-id="e3844-112">0</span><span class="sxs-lookup"><span data-stu-id="e3844-112">0</span></span>|<span data-ttu-id="e3844-113">设备注册状态未知</span><span class="sxs-lookup"><span data-stu-id="e3844-113">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="e3844-114">enrolled</span><span class="sxs-lookup"><span data-stu-id="e3844-114">enrolled</span></span>|<span data-ttu-id="e3844-115">1</span><span class="sxs-lookup"><span data-stu-id="e3844-115">1</span></span>|<span data-ttu-id="e3844-116">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="e3844-116">Device is Enrolled.</span></span>|
|<span data-ttu-id="e3844-117">pendingReset</span><span class="sxs-lookup"><span data-stu-id="e3844-117">pendingReset</span></span>|<span data-ttu-id="e3844-118">2</span><span class="sxs-lookup"><span data-stu-id="e3844-118">2</span></span>|<span data-ttu-id="e3844-119">已注册，但通过注册配置文件注册，并且已注册的配置文件与分配的配置文件不同。</span><span class="sxs-lookup"><span data-stu-id="e3844-119">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="e3844-120">failed</span><span class="sxs-lookup"><span data-stu-id="e3844-120">failed</span></span>|<span data-ttu-id="e3844-121">3</span><span class="sxs-lookup"><span data-stu-id="e3844-121">3</span></span>|<span data-ttu-id="e3844-122">未注册，并且存在注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="e3844-122">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="e3844-123">notContacted</span><span class="sxs-lookup"><span data-stu-id="e3844-123">notContacted</span></span>|<span data-ttu-id="e3844-124">4 </span><span class="sxs-lookup"><span data-stu-id="e3844-124">4</span></span>|<span data-ttu-id="e3844-125">设备已导入，但没有注册。</span><span class="sxs-lookup"><span data-stu-id="e3844-125">Device is imported but not enrolled.</span></span>|




