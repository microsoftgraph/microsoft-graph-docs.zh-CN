---
title: windowsSModeConfiguration 枚举类型
description: 可能的选项，可配置 S 模式解除锁定
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9e37bd51be1b5476e8b4590b92b3caeeed92ac45
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27830735"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="9bb17-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9bb17-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="9bb17-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="9bb17-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9bb17-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="9bb17-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9bb17-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9bb17-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bb17-107">可能的选项，可配置 S 模式解除锁定</span><span class="sxs-lookup"><span data-stu-id="9bb17-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="9bb17-108">成员</span><span class="sxs-lookup"><span data-stu-id="9bb17-108">Members</span></span>
|<span data-ttu-id="9bb17-109">成员</span><span class="sxs-lookup"><span data-stu-id="9bb17-109">Member</span></span>|<span data-ttu-id="9bb17-110">值</span><span class="sxs-lookup"><span data-stu-id="9bb17-110">Value</span></span>|<span data-ttu-id="9bb17-111">Description</span><span class="sxs-lookup"><span data-stu-id="9bb17-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bb17-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="9bb17-112">noRestriction</span></span>|<span data-ttu-id="9bb17-113">0</span><span class="sxs-lookup"><span data-stu-id="9bb17-113">0</span></span>|<span data-ttu-id="9bb17-114">此选项将删除所有限制解锁 S 模式的默认设置</span><span class="sxs-lookup"><span data-stu-id="9bb17-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="9bb17-115">阻止</span><span class="sxs-lookup"><span data-stu-id="9bb17-115">block</span></span>|<span data-ttu-id="9bb17-116">1</span><span class="sxs-lookup"><span data-stu-id="9bb17-116">1</span></span>|<span data-ttu-id="9bb17-117">此选项将阻止用户解锁设备从 S 模式</span><span class="sxs-lookup"><span data-stu-id="9bb17-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="9bb17-118">解除锁定</span><span class="sxs-lookup"><span data-stu-id="9bb17-118">unlock</span></span>|<span data-ttu-id="9bb17-119">2</span><span class="sxs-lookup"><span data-stu-id="9bb17-119">2</span></span>|<span data-ttu-id="9bb17-120">此选项将解锁设备从 S 模式</span><span class="sxs-lookup"><span data-stu-id="9bb17-120">This option will unlock the device from S mode</span></span>|





