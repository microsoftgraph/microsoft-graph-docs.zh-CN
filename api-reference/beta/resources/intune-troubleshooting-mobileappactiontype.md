---
title: mobileAppActionType 枚举类型
description: 定义 Intune 应用程序的操作类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: c143a323db566c49003733a7592d380a46443440
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523350"
---
# <a name="mobileappactiontype-enum-type"></a><span data-ttu-id="0cf65-103">mobileAppActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0cf65-103">mobileAppActionType enum type</span></span>

<span data-ttu-id="0cf65-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0cf65-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0cf65-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0cf65-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cf65-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cf65-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cf65-107">定义 Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="0cf65-107">Defines the Action Types for an Intune Application.</span></span>

## <a name="members"></a><span data-ttu-id="0cf65-108">成员</span><span class="sxs-lookup"><span data-stu-id="0cf65-108">Members</span></span>
|<span data-ttu-id="0cf65-109">成员</span><span class="sxs-lookup"><span data-stu-id="0cf65-109">Member</span></span>|<span data-ttu-id="0cf65-110">值</span><span class="sxs-lookup"><span data-stu-id="0cf65-110">Value</span></span>|<span data-ttu-id="0cf65-111">说明</span><span class="sxs-lookup"><span data-stu-id="0cf65-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cf65-112">unknown</span><span class="sxs-lookup"><span data-stu-id="0cf65-112">unknown</span></span>|<span data-ttu-id="0cf65-113">0</span><span class="sxs-lookup"><span data-stu-id="0cf65-113">0</span></span>|<span data-ttu-id="0cf65-114">未知结果。</span><span class="sxs-lookup"><span data-stu-id="0cf65-114">Unknown result.</span></span>|
|<span data-ttu-id="0cf65-115">installCommandSent</span><span class="sxs-lookup"><span data-stu-id="0cf65-115">installCommandSent</span></span>|<span data-ttu-id="0cf65-116">1 </span><span class="sxs-lookup"><span data-stu-id="0cf65-116">1</span></span>|<span data-ttu-id="0cf65-117">已发送应用程序安装命令。</span><span class="sxs-lookup"><span data-stu-id="0cf65-117">Application install command was sent.</span></span>|
|<span data-ttu-id="0cf65-118">了</span><span class="sxs-lookup"><span data-stu-id="0cf65-118">installed</span></span>|<span data-ttu-id="0cf65-119">3 </span><span class="sxs-lookup"><span data-stu-id="0cf65-119">3</span></span>|<span data-ttu-id="0cf65-120">已安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="0cf65-120">Application installed.</span></span>|
|<span data-ttu-id="0cf65-121">#b0</span><span class="sxs-lookup"><span data-stu-id="0cf65-121">uninstalled</span></span>|<span data-ttu-id="0cf65-122">4 </span><span class="sxs-lookup"><span data-stu-id="0cf65-122">4</span></span>|<span data-ttu-id="0cf65-123">已卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="0cf65-123">Application uninstalled.</span></span>|
|<span data-ttu-id="0cf65-124">userRequestedInstall</span><span class="sxs-lookup"><span data-stu-id="0cf65-124">userRequestedInstall</span></span>|<span data-ttu-id="0cf65-125">5 </span><span class="sxs-lookup"><span data-stu-id="0cf65-125">5</span></span>|<span data-ttu-id="0cf65-126">用户请求安装</span><span class="sxs-lookup"><span data-stu-id="0cf65-126">User requested installation</span></span>|



