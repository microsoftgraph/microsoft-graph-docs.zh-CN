---
title: ndesConnectorState 枚举类型
description: Ndes 连接符的当前状态。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a9cfb0ec31bccd853b3ff2b2965c83fb6813a82e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409382"
---
# <a name="ndesconnectorstate-enum-type"></a><span data-ttu-id="e61f5-103">ndesConnectorState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e61f5-103">ndesConnectorState enum type</span></span>

> <span data-ttu-id="e61f5-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e61f5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e61f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e61f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e61f5-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e61f5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e61f5-107">Ndes 连接符的当前状态。</span><span class="sxs-lookup"><span data-stu-id="e61f5-107">The current status of the Ndes Connector.</span></span>

## <a name="members"></a><span data-ttu-id="e61f5-108">成员</span><span class="sxs-lookup"><span data-stu-id="e61f5-108">Members</span></span>
|<span data-ttu-id="e61f5-109">成员</span><span class="sxs-lookup"><span data-stu-id="e61f5-109">Member</span></span>|<span data-ttu-id="e61f5-110">值</span><span class="sxs-lookup"><span data-stu-id="e61f5-110">Value</span></span>|<span data-ttu-id="e61f5-111">说明</span><span class="sxs-lookup"><span data-stu-id="e61f5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e61f5-112">无</span><span class="sxs-lookup"><span data-stu-id="e61f5-112">none</span></span>|<span data-ttu-id="e61f5-113">0</span><span class="sxs-lookup"><span data-stu-id="e61f5-113">0</span></span>|<span data-ttu-id="e61f5-114">状态为该连接器尚不可用。</span><span class="sxs-lookup"><span data-stu-id="e61f5-114">State not available yet for this connector.</span></span>|
|<span data-ttu-id="e61f5-115">活动</span><span class="sxs-lookup"><span data-stu-id="e61f5-115">active</span></span>|<span data-ttu-id="e61f5-116">1</span><span class="sxs-lookup"><span data-stu-id="e61f5-116">1</span></span>|<span data-ttu-id="e61f5-117">Ndes 连接器最近已连接</span><span class="sxs-lookup"><span data-stu-id="e61f5-117">Ndes connector has connected recently</span></span>|
|<span data-ttu-id="e61f5-118">非活动</span><span class="sxs-lookup"><span data-stu-id="e61f5-118">inactive</span></span>|<span data-ttu-id="e61f5-119">2</span><span class="sxs-lookup"><span data-stu-id="e61f5-119">2</span></span>|<span data-ttu-id="e61f5-120">Ndes 连接器最近没有活动</span><span class="sxs-lookup"><span data-stu-id="e61f5-120">No recent activity for the Ndes connector</span></span>|




