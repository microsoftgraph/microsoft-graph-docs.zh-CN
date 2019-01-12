---
title: vpnTrafficRuleAppType 枚举类型
description: 指示 VPN 流量规则关联的应用程序的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 6adf30f981bcb3ee4d57410a63419b29ac4184cd
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937739"
---
# <a name="vpntrafficruleapptype-enum-type"></a><span data-ttu-id="a655f-103">vpnTrafficRuleAppType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="a655f-103">vpnTrafficRuleAppType enum type</span></span>

> <span data-ttu-id="a655f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a655f-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a655f-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a655f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a655f-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a655f-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a655f-107">指示 VPN 流量规则关联的应用程序的类型。</span><span class="sxs-lookup"><span data-stu-id="a655f-107">Indicates the type of app that a VPN traffic rule is associated with.</span></span>
## <a name="members"></a><span data-ttu-id="a655f-108">成员</span><span class="sxs-lookup"><span data-stu-id="a655f-108">Members</span></span>
|<span data-ttu-id="a655f-109">成员</span><span class="sxs-lookup"><span data-stu-id="a655f-109">Member</span></span>|<span data-ttu-id="a655f-110">值</span><span class="sxs-lookup"><span data-stu-id="a655f-110">Value</span></span>|<span data-ttu-id="a655f-111">Description</span><span class="sxs-lookup"><span data-stu-id="a655f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a655f-112">无</span><span class="sxs-lookup"><span data-stu-id="a655f-112">none</span></span>|<span data-ttu-id="a655f-113">0</span><span class="sxs-lookup"><span data-stu-id="a655f-113">0</span></span>|<span data-ttu-id="a655f-114">通信规则不与应用程序相关联。</span><span class="sxs-lookup"><span data-stu-id="a655f-114">The traffic rule is not associated with an app.</span></span>|
|<span data-ttu-id="a655f-115">桌面</span><span class="sxs-lookup"><span data-stu-id="a655f-115">desktop</span></span>|<span data-ttu-id="a655f-116">1</span><span class="sxs-lookup"><span data-stu-id="a655f-116">1</span></span>|<span data-ttu-id="a655f-117">与桌面应用程序相关联的流量规则。</span><span class="sxs-lookup"><span data-stu-id="a655f-117">The traffic rule is associated with a desktop app.</span></span>|
|<span data-ttu-id="a655f-118">通用</span><span class="sxs-lookup"><span data-stu-id="a655f-118">universal</span></span>|<span data-ttu-id="a655f-119">2</span><span class="sxs-lookup"><span data-stu-id="a655f-119">2</span></span>|<span data-ttu-id="a655f-120">通信规则相关联的通用的应用程序。</span><span class="sxs-lookup"><span data-stu-id="a655f-120">The traffic rule is associated with a Universal app.</span></span>|





