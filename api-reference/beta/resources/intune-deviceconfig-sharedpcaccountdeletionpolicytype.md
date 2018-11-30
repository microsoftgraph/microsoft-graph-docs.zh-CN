---
title: sharedPCAccountDeletionPolicyType 枚举类型
description: 当共享 PC 上删除帐户可能值。
ms.openlocfilehash: bf58a865dcb970760c4cf5284533cd833fcf9304
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045378"
---
# <a name="sharedpcaccountdeletionpolicytype-enum-type"></a><span data-ttu-id="f18b1-103">sharedPCAccountDeletionPolicyType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="f18b1-103">sharedPCAccountDeletionPolicyType enum type</span></span>

> <span data-ttu-id="f18b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f18b1-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f18b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f18b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f18b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f18b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f18b1-107">当共享 PC 上删除帐户可能值。</span><span class="sxs-lookup"><span data-stu-id="f18b1-107">Possible values for when accounts are deleted on a shared PC.</span></span>
## <a name="members"></a><span data-ttu-id="f18b1-108">成员</span><span class="sxs-lookup"><span data-stu-id="f18b1-108">Members</span></span>
|<span data-ttu-id="f18b1-109">成员</span><span class="sxs-lookup"><span data-stu-id="f18b1-109">Member</span></span>|<span data-ttu-id="f18b1-110">值</span><span class="sxs-lookup"><span data-stu-id="f18b1-110">Value</span></span>|<span data-ttu-id="f18b1-111">说明</span><span class="sxs-lookup"><span data-stu-id="f18b1-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f18b1-112">立即</span><span class="sxs-lookup"><span data-stu-id="f18b1-112">immediate</span></span>|<span data-ttu-id="f18b1-113">0</span><span class="sxs-lookup"><span data-stu-id="f18b1-113">0</span></span>|<span data-ttu-id="f18b1-114">立即删除。</span><span class="sxs-lookup"><span data-stu-id="f18b1-114">Delete immediately.</span></span>|
|<span data-ttu-id="f18b1-115">diskSpaceThreshold</span><span class="sxs-lookup"><span data-stu-id="f18b1-115">diskSpaceThreshold</span></span>|<span data-ttu-id="f18b1-116">1</span><span class="sxs-lookup"><span data-stu-id="f18b1-116">1</span></span>|<span data-ttu-id="f18b1-117">删除在磁盘空间阈值。</span><span class="sxs-lookup"><span data-stu-id="f18b1-117">Delete at disk space threshold.</span></span>|
|<span data-ttu-id="f18b1-118">diskSpaceThresholdOrInactiveThreshold</span><span class="sxs-lookup"><span data-stu-id="f18b1-118">diskSpaceThresholdOrInactiveThreshold</span></span>|<span data-ttu-id="f18b1-119">2</span><span class="sxs-lookup"><span data-stu-id="f18b1-119">2</span></span>|<span data-ttu-id="f18b1-120">删除在磁盘空间阈值或非活动状态的阈值。</span><span class="sxs-lookup"><span data-stu-id="f18b1-120">Delete at disk space threshold or inactive threshold.</span></span>|





