---
title: vppTokenSyncStatus 枚举类型
description: 可能与 Apple Volume Purchase Program 令牌关联的同步状态。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 7af4ed87234dc588a9d0969d2ed347adaa4d29da
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037226"
---
# <a name="vpptokensyncstatus-enum-type"></a><span data-ttu-id="07297-103">vppTokenSyncStatus 枚举类型</span><span class="sxs-lookup"><span data-stu-id="07297-103">vppTokenSyncStatus enum type</span></span>

> <span data-ttu-id="07297-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07297-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07297-105">可能与 Apple Volume Purchase Program 令牌关联的同步状态。</span><span class="sxs-lookup"><span data-stu-id="07297-105">Possible sync statuses associated with an Apple Volume Purchase Program token.</span></span>

## <a name="members"></a><span data-ttu-id="07297-106">成员</span><span class="sxs-lookup"><span data-stu-id="07297-106">Members</span></span>
|<span data-ttu-id="07297-107">成员</span><span class="sxs-lookup"><span data-stu-id="07297-107">Member</span></span>|<span data-ttu-id="07297-108">值</span><span class="sxs-lookup"><span data-stu-id="07297-108">Value</span></span>|<span data-ttu-id="07297-109">说明</span><span class="sxs-lookup"><span data-stu-id="07297-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07297-110">无</span><span class="sxs-lookup"><span data-stu-id="07297-110">none</span></span>|<span data-ttu-id="07297-111">0</span><span class="sxs-lookup"><span data-stu-id="07297-111">0</span></span>|<span data-ttu-id="07297-112">默认状态。</span><span class="sxs-lookup"><span data-stu-id="07297-112">Default status.</span></span>|
|<span data-ttu-id="07297-113">inProgress</span><span class="sxs-lookup"><span data-stu-id="07297-113">inProgress</span></span>|<span data-ttu-id="07297-114">1</span><span class="sxs-lookup"><span data-stu-id="07297-114">1</span></span>|<span data-ttu-id="07297-115">上次同步进行中。</span><span class="sxs-lookup"><span data-stu-id="07297-115">Last Sync in progress.</span></span>|
|<span data-ttu-id="07297-116">后</span><span class="sxs-lookup"><span data-stu-id="07297-116">completed</span></span>|<span data-ttu-id="07297-117">双面</span><span class="sxs-lookup"><span data-stu-id="07297-117">2</span></span>|<span data-ttu-id="07297-118">上次同步成功完成。</span><span class="sxs-lookup"><span data-stu-id="07297-118">Last Sync completed successfully.</span></span>|
|<span data-ttu-id="07297-119">未能</span><span class="sxs-lookup"><span data-stu-id="07297-119">failed</span></span>|<span data-ttu-id="07297-120">第三章</span><span class="sxs-lookup"><span data-stu-id="07297-120">3</span></span>|<span data-ttu-id="07297-121">上次同步失败。</span><span class="sxs-lookup"><span data-stu-id="07297-121">Last Sync failed.</span></span>|



