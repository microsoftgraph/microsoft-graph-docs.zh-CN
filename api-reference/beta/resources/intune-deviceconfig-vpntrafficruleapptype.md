---
title: vpnTrafficRuleAppType 枚举类型
description: 指示与 VPN 流量规则相关联的应用程序的类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1762e952bbebfc985f9af9694bfb14e0bdd7d19f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367545"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="4a505-103">vpnTrafficRuleAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="4a505-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="4a505-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4a505-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4a505-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4a505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a505-106">指示与 VPN 流量规则相关联的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="4a505-106">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="4a505-107">成员</span><span class="sxs-lookup"><span data-stu-id="4a505-107">Members</span></span>
|<span data-ttu-id="4a505-108">成员</span><span class="sxs-lookup"><span data-stu-id="4a505-108">Member</span></span>|<span data-ttu-id="4a505-109">值</span><span class="sxs-lookup"><span data-stu-id="4a505-109">Value</span></span>|<span data-ttu-id="4a505-110">说明</span><span class="sxs-lookup"><span data-stu-id="4a505-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a505-111">无</span><span class="sxs-lookup"><span data-stu-id="4a505-111">none</span></span>|<span data-ttu-id="4a505-112">0</span><span class="sxs-lookup"><span data-stu-id="4a505-112">0</span></span>|<span data-ttu-id="4a505-113">流量规则不与应用关联。</span><span class="sxs-lookup"><span data-stu-id="4a505-113">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="4a505-114">desktop</span><span class="sxs-lookup"><span data-stu-id="4a505-114">desktop</span></span>|<span data-ttu-id="4a505-115">1</span><span class="sxs-lookup"><span data-stu-id="4a505-115">1</span></span>|<span data-ttu-id="4a505-116">流量规则与桌面应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="4a505-116">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="4a505-117">普遍</span><span class="sxs-lookup"><span data-stu-id="4a505-117">universal</span></span>|<span data-ttu-id="4a505-118">双面</span><span class="sxs-lookup"><span data-stu-id="4a505-118">2</span></span>|<span data-ttu-id="4a505-119">流量规则与通用应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="4a505-119">The traffic rule is associated with a Universal app.</span></span>|



