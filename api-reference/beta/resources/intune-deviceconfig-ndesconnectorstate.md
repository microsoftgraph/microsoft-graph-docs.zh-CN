---
title: ndesConnectorState 枚举类型
description: Ndes 连接符的当前状态。
author: tfitzmac
ms.openlocfilehash: e52f1651ab5e829e1ebe3dca77fc5056d17bf13f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347472"
---
# <a name="ndesconnectorstate-enum-type"></a><span data-ttu-id="5d49e-103">ndesConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5d49e-103">ndesConnectorState enum type</span></span>

> <span data-ttu-id="5d49e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5d49e-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d49e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5d49e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d49e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5d49e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d49e-107">Ndes 连接符的当前状态。</span><span class="sxs-lookup"><span data-stu-id="5d49e-107">The current status of the Ndes Connector.</span></span>
## <a name="members"></a><span data-ttu-id="5d49e-108">成员</span><span class="sxs-lookup"><span data-stu-id="5d49e-108">Members</span></span>
|<span data-ttu-id="5d49e-109">成员</span><span class="sxs-lookup"><span data-stu-id="5d49e-109">Member</span></span>|<span data-ttu-id="5d49e-110">值</span><span class="sxs-lookup"><span data-stu-id="5d49e-110">Value</span></span>|<span data-ttu-id="5d49e-111">说明</span><span class="sxs-lookup"><span data-stu-id="5d49e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5d49e-112">无</span><span class="sxs-lookup"><span data-stu-id="5d49e-112">none</span></span>|<span data-ttu-id="5d49e-113">0</span><span class="sxs-lookup"><span data-stu-id="5d49e-113">0</span></span>|<span data-ttu-id="5d49e-114">状态为该连接器尚不可用。</span><span class="sxs-lookup"><span data-stu-id="5d49e-114">State not available yet for this connector.</span></span>|
|<span data-ttu-id="5d49e-115">活动</span><span class="sxs-lookup"><span data-stu-id="5d49e-115">active</span></span>|<span data-ttu-id="5d49e-116">1</span><span class="sxs-lookup"><span data-stu-id="5d49e-116">1</span></span>|<span data-ttu-id="5d49e-117">Ndes 连接器最近已连接</span><span class="sxs-lookup"><span data-stu-id="5d49e-117">Ndes connector has connected recently</span></span>|
|<span data-ttu-id="5d49e-118">非活动</span><span class="sxs-lookup"><span data-stu-id="5d49e-118">inactive</span></span>|<span data-ttu-id="5d49e-119">2</span><span class="sxs-lookup"><span data-stu-id="5d49e-119">2</span></span>|<span data-ttu-id="5d49e-120">Ndes 连接器最近没有活动</span><span class="sxs-lookup"><span data-stu-id="5d49e-120">No recent activity for the Ndes connector</span></span>|





