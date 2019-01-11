---
title: vpnTrafficRuleAppType 枚举类型
description: 指示 VPN 流量规则关联的应用程序的类型。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 71e0af722c690188b3bb0e9dc33327f443cc9086
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27835810"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="d0444-103">vpnTrafficRuleAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="d0444-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="d0444-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d0444-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d0444-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d0444-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d0444-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d0444-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0444-107">指示 VPN 流量规则关联的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="d0444-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>
## <a name="members"></a><span data-ttu-id="d0444-108">成员</span><span class="sxs-lookup"><span data-stu-id="d0444-108">Members</span></span>
|<span data-ttu-id="d0444-109">成员</span><span class="sxs-lookup"><span data-stu-id="d0444-109">Member</span></span>|<span data-ttu-id="d0444-110">值</span><span class="sxs-lookup"><span data-stu-id="d0444-110">Value</span></span>|<span data-ttu-id="d0444-111">Description</span><span class="sxs-lookup"><span data-stu-id="d0444-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0444-112">无</span><span class="sxs-lookup"><span data-stu-id="d0444-112">none</span></span>|<span data-ttu-id="d0444-113">0</span><span class="sxs-lookup"><span data-stu-id="d0444-113">0</span></span>|<span data-ttu-id="d0444-114">通信规则不与应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="d0444-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="d0444-115">桌面</span><span class="sxs-lookup"><span data-stu-id="d0444-115">desktop</span></span>|<span data-ttu-id="d0444-116">1</span><span class="sxs-lookup"><span data-stu-id="d0444-116">1</span></span>|<span data-ttu-id="d0444-117">与桌面应用程序相关联的流量规则。</span><span class="sxs-lookup"><span data-stu-id="d0444-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="d0444-118">通用</span><span class="sxs-lookup"><span data-stu-id="d0444-118">universal</span></span>|<span data-ttu-id="d0444-119">2</span><span class="sxs-lookup"><span data-stu-id="d0444-119">2</span></span>|<span data-ttu-id="d0444-120">通信规则相关联的通用的应用程序。</span><span class="sxs-lookup"><span data-stu-id="d0444-120">The traffic rule is associated with a Universal app.</span></span>|





