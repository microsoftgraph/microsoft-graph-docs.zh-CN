---
title: vpnTrafficRuleAppType 枚举类型
description: 指示与 VPN 流量规则相关联的应用程序的类型。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: cad0ab3a49c6139707fb30c703cc670be6bc5f7e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358999"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="08564-103">vpnTrafficRuleAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="08564-103">vpnTrafficRuleAppType enum type</span></span>

<span data-ttu-id="08564-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08564-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08564-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08564-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08564-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08564-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08564-107">指示与 VPN 流量规则相关联的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="08564-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>

## <a name="members"></a><span data-ttu-id="08564-108">成员</span><span class="sxs-lookup"><span data-stu-id="08564-108">Members</span></span>
|<span data-ttu-id="08564-109">成员</span><span class="sxs-lookup"><span data-stu-id="08564-109">Member</span></span>|<span data-ttu-id="08564-110">值</span><span class="sxs-lookup"><span data-stu-id="08564-110">Value</span></span>|<span data-ttu-id="08564-111">说明</span><span class="sxs-lookup"><span data-stu-id="08564-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08564-112">无</span><span class="sxs-lookup"><span data-stu-id="08564-112">none</span></span>|<span data-ttu-id="08564-113">0</span><span class="sxs-lookup"><span data-stu-id="08564-113">0</span></span>|<span data-ttu-id="08564-114">流量规则不与应用关联。</span><span class="sxs-lookup"><span data-stu-id="08564-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="08564-115">desktop</span><span class="sxs-lookup"><span data-stu-id="08564-115">desktop</span></span>|<span data-ttu-id="08564-116">1</span><span class="sxs-lookup"><span data-stu-id="08564-116">1</span></span>|<span data-ttu-id="08564-117">流量规则与桌面应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="08564-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="08564-118">普遍</span><span class="sxs-lookup"><span data-stu-id="08564-118">universal</span></span>|<span data-ttu-id="08564-119">双面</span><span class="sxs-lookup"><span data-stu-id="08564-119">2</span></span>|<span data-ttu-id="08564-120">流量规则与通用应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="08564-120">The traffic rule is associated with a Universal app.</span></span>|



