---
title: windowsSModeConfiguration 枚举类型
description: 可能的选项，可配置 S 模式解除锁定
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 858be5b3a55fbbf4454aa576785ba793f501079c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415465"
---
# <a name="windowssmodeconfiguration-enum-type"></a><span data-ttu-id="c562f-103">windowsSModeConfiguration 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c562f-103">windowsSModeConfiguration enum type</span></span>

> <span data-ttu-id="c562f-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="c562f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c562f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c562f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c562f-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c562f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c562f-107">可能的选项，可配置 S 模式解除锁定</span><span class="sxs-lookup"><span data-stu-id="c562f-107">The possible options to configure S mode unlock</span></span>

## <a name="members"></a><span data-ttu-id="c562f-108">成员</span><span class="sxs-lookup"><span data-stu-id="c562f-108">Members</span></span>
|<span data-ttu-id="c562f-109">成员</span><span class="sxs-lookup"><span data-stu-id="c562f-109">Member</span></span>|<span data-ttu-id="c562f-110">值</span><span class="sxs-lookup"><span data-stu-id="c562f-110">Value</span></span>|<span data-ttu-id="c562f-111">说明</span><span class="sxs-lookup"><span data-stu-id="c562f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c562f-112">noRestriction</span><span class="sxs-lookup"><span data-stu-id="c562f-112">noRestriction</span></span>|<span data-ttu-id="c562f-113">0</span><span class="sxs-lookup"><span data-stu-id="c562f-113">0</span></span>|<span data-ttu-id="c562f-114">此选项将删除所有限制解锁 S 模式的默认设置</span><span class="sxs-lookup"><span data-stu-id="c562f-114">This option will remove all restrictions to unlock S mode - default</span></span>|
|<span data-ttu-id="c562f-115">阻止</span><span class="sxs-lookup"><span data-stu-id="c562f-115">block</span></span>|<span data-ttu-id="c562f-116">1</span><span class="sxs-lookup"><span data-stu-id="c562f-116">1</span></span>|<span data-ttu-id="c562f-117">此选项将阻止用户解锁设备从 S 模式</span><span class="sxs-lookup"><span data-stu-id="c562f-117">This option will block the user to unlock the device from S mode</span></span>|
|<span data-ttu-id="c562f-118">解除锁定</span><span class="sxs-lookup"><span data-stu-id="c562f-118">unlock</span></span>|<span data-ttu-id="c562f-119">2</span><span class="sxs-lookup"><span data-stu-id="c562f-119">2</span></span>|<span data-ttu-id="c562f-120">此选项将解锁设备从 S 模式</span><span class="sxs-lookup"><span data-stu-id="c562f-120">This option will unlock the device from S mode</span></span>|




