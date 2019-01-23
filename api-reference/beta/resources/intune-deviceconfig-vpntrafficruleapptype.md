---
title: vpnTrafficRuleAppType 枚举类型
description: 指示 VPN 流量规则关联的应用程序的类型。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 061cb5701830939576f5b9a649c73b4d44eada18
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396019"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="58051-103">vpnTrafficRuleAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="58051-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="58051-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="58051-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="58051-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="58051-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="58051-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58051-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58051-107">指示 VPN 流量规则关联的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="58051-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="58051-108">成员</span><span class="sxs-lookup"><span data-stu-id="58051-108">Members</span></span>
|<span data-ttu-id="58051-109">成员</span><span class="sxs-lookup"><span data-stu-id="58051-109">Member</span></span>|<span data-ttu-id="58051-110">值</span><span class="sxs-lookup"><span data-stu-id="58051-110">Value</span></span>|<span data-ttu-id="58051-111">说明</span><span class="sxs-lookup"><span data-stu-id="58051-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58051-112">无</span><span class="sxs-lookup"><span data-stu-id="58051-112">none</span></span>|<span data-ttu-id="58051-113">0</span><span class="sxs-lookup"><span data-stu-id="58051-113">0</span></span>|<span data-ttu-id="58051-114">通信规则不与应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="58051-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="58051-115">桌面</span><span class="sxs-lookup"><span data-stu-id="58051-115">desktop</span></span>|<span data-ttu-id="58051-116">1</span><span class="sxs-lookup"><span data-stu-id="58051-116">1</span></span>|<span data-ttu-id="58051-117">与桌面应用程序相关联的流量规则。</span><span class="sxs-lookup"><span data-stu-id="58051-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="58051-118">通用</span><span class="sxs-lookup"><span data-stu-id="58051-118">universal</span></span>|<span data-ttu-id="58051-119">2</span><span class="sxs-lookup"><span data-stu-id="58051-119">2</span></span>|<span data-ttu-id="58051-120">通信规则相关联的通用的应用程序。</span><span class="sxs-lookup"><span data-stu-id="58051-120">The traffic rule is associated with a Universal app.</span></span>|




