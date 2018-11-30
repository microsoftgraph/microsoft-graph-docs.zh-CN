---
title: windowsSModeConfiguration 枚举类型
description: 可能的选项，可配置 S 模式解除锁定
ms.openlocfilehash: b96e601927adc90c3daadc9658a8fdcb71661d3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046634"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="87898-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="87898-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="87898-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="87898-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="87898-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="87898-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="87898-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="87898-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87898-107">可能的选项，可配置 S 模式解除锁定</span><span class="sxs-lookup"><span data-stu-id="87898-107">The possible options to configure S mode unlock</span></span>
## <a name="members"></a><span data-ttu-id="87898-108">成员</span><span class="sxs-lookup"><span data-stu-id="87898-108">Members</span></span>
|<span data-ttu-id="87898-109">成员</span><span class="sxs-lookup"><span data-stu-id="87898-109">Member</span></span>|<span data-ttu-id="87898-110">值</span><span class="sxs-lookup"><span data-stu-id="87898-110">Value</span></span>|<span data-ttu-id="87898-111">说明</span><span class="sxs-lookup"><span data-stu-id="87898-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87898-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="87898-112">noRestriction</span></span>|<span data-ttu-id="87898-113">0</span><span class="sxs-lookup"><span data-stu-id="87898-113">0</span></span>|<span data-ttu-id="87898-114">此选项将删除所有限制解锁 S 模式的默认设置</span><span class="sxs-lookup"><span data-stu-id="87898-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="87898-115">阻止</span><span class="sxs-lookup"><span data-stu-id="87898-115">block</span></span>|<span data-ttu-id="87898-116">1</span><span class="sxs-lookup"><span data-stu-id="87898-116">1</span></span>|<span data-ttu-id="87898-117">此选项将阻止用户解锁设备从 S 模式</span><span class="sxs-lookup"><span data-stu-id="87898-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="87898-118">解除锁定</span><span class="sxs-lookup"><span data-stu-id="87898-118">unlock</span></span>|<span data-ttu-id="87898-119">2</span><span class="sxs-lookup"><span data-stu-id="87898-119">2</span></span>|<span data-ttu-id="87898-120">此选项将解锁设备从 S 模式</span><span class="sxs-lookup"><span data-stu-id="87898-120">This option will unlock the device from S mode</span></span>|





