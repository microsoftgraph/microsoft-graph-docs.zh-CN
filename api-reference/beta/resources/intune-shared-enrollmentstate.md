---
title: enrollmentState 枚举类型
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: d208f8a4d1097d6698be3175a0b5ae86cf1918d4
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866795"
---
# <a name="enrollmentstate-enum-type"></a><span data-ttu-id="b71a3-103">enrollmentState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b71a3-103">enrollmentState enum type</span></span>

<span data-ttu-id="b71a3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b71a3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b71a3-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b71a3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b71a3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b71a3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b71a3-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="b71a3-107">Not yet documented</span></span>

## <a name="members"></a><span data-ttu-id="b71a3-108">成员</span><span class="sxs-lookup"><span data-stu-id="b71a3-108">Members</span></span>
|<span data-ttu-id="b71a3-109">成员</span><span class="sxs-lookup"><span data-stu-id="b71a3-109">Member</span></span>|<span data-ttu-id="b71a3-110">值</span><span class="sxs-lookup"><span data-stu-id="b71a3-110">Value</span></span>|<span data-ttu-id="b71a3-111">说明</span><span class="sxs-lookup"><span data-stu-id="b71a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b71a3-112">unknown</span><span class="sxs-lookup"><span data-stu-id="b71a3-112">unknown</span></span>|<span data-ttu-id="b71a3-113">0</span><span class="sxs-lookup"><span data-stu-id="b71a3-113">0</span></span>|<span data-ttu-id="b71a3-114">设备注册状态未知</span><span class="sxs-lookup"><span data-stu-id="b71a3-114">Device enrollment state is unknown</span></span>|
|<span data-ttu-id="b71a3-115">enrolled</span><span class="sxs-lookup"><span data-stu-id="b71a3-115">enrolled</span></span>|<span data-ttu-id="b71a3-116">1</span><span class="sxs-lookup"><span data-stu-id="b71a3-116">1</span></span>|<span data-ttu-id="b71a3-117">设备已注册。</span><span class="sxs-lookup"><span data-stu-id="b71a3-117">Device is Enrolled.</span></span>|
|<span data-ttu-id="b71a3-118">pendingReset</span><span class="sxs-lookup"><span data-stu-id="b71a3-118">pendingReset</span></span>|<span data-ttu-id="b71a3-119">2</span><span class="sxs-lookup"><span data-stu-id="b71a3-119">2</span></span>|<span data-ttu-id="b71a3-120">已注册，但通过注册配置文件注册，并且已注册的配置文件与分配的配置文件不同。</span><span class="sxs-lookup"><span data-stu-id="b71a3-120">Enrolled but it's enrolled via enrollment profile and the enrolled profile is different from the assigned profile.</span></span>|
|<span data-ttu-id="b71a3-121">failed</span><span class="sxs-lookup"><span data-stu-id="b71a3-121">failed</span></span>|<span data-ttu-id="b71a3-122">3</span><span class="sxs-lookup"><span data-stu-id="b71a3-122">3</span></span>|<span data-ttu-id="b71a3-123">未注册，并且存在注册失败记录。</span><span class="sxs-lookup"><span data-stu-id="b71a3-123">Not enrolled and there is enrollment failure record.</span></span>|
|<span data-ttu-id="b71a3-124">notContacted</span><span class="sxs-lookup"><span data-stu-id="b71a3-124">notContacted</span></span>|<span data-ttu-id="b71a3-125">4 </span><span class="sxs-lookup"><span data-stu-id="b71a3-125">4</span></span>|<span data-ttu-id="b71a3-126">设备已导入，但没有注册。</span><span class="sxs-lookup"><span data-stu-id="b71a3-126">Device is imported but not enrolled.</span></span>|
|<span data-ttu-id="b71a3-127">blocked</span><span class="sxs-lookup"><span data-stu-id="b71a3-127">blocked</span></span>|<span data-ttu-id="b71a3-128">5 </span><span class="sxs-lookup"><span data-stu-id="b71a3-128">5</span></span>|<span data-ttu-id="b71a3-129">设备以无用户状态注册，但因应用安装失败，无法移动到用户注册。</span><span class="sxs-lookup"><span data-stu-id="b71a3-129">Device is enrolled as userless, but is blocked from moving to user enrollment because the app failed to install.</span></span>|




