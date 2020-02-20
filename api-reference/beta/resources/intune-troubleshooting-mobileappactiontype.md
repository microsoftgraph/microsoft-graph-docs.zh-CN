---
title: mobileAppActionType 枚举类型
description: 定义 Intune 应用程序的操作类型。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a33bab80a8d988ad2f57f0b98c42cf8eca8662da
ms.sourcegitcommit: 5cf98ba275547e5659df4af1eeeff0ba484b0e67
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/20/2020
ms.locfileid: "42159064"
---
# <a name="mobileappactiontype-enum-type"></a><span data-ttu-id="e1a19-103">mobileAppActionType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="e1a19-103">mobileAppActionType enum type</span></span>

> <span data-ttu-id="e1a19-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e1a19-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e1a19-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e1a19-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1a19-106">定义 Intune 应用程序的操作类型。</span><span class="sxs-lookup"><span data-stu-id="e1a19-106">Defines the Action Types for an Intune Application.</span></span>

## <a name="members"></a><span data-ttu-id="e1a19-107">成员</span><span class="sxs-lookup"><span data-stu-id="e1a19-107">Members</span></span>
|<span data-ttu-id="e1a19-108">成员</span><span class="sxs-lookup"><span data-stu-id="e1a19-108">Member</span></span>|<span data-ttu-id="e1a19-109">值</span><span class="sxs-lookup"><span data-stu-id="e1a19-109">Value</span></span>|<span data-ttu-id="e1a19-110">说明</span><span class="sxs-lookup"><span data-stu-id="e1a19-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1a19-111">unknown</span><span class="sxs-lookup"><span data-stu-id="e1a19-111">unknown</span></span>|<span data-ttu-id="e1a19-112">0</span><span class="sxs-lookup"><span data-stu-id="e1a19-112">0</span></span>|<span data-ttu-id="e1a19-113">未知结果。</span><span class="sxs-lookup"><span data-stu-id="e1a19-113">Unknown result.</span></span>|
|<span data-ttu-id="e1a19-114">installCommandSent</span><span class="sxs-lookup"><span data-stu-id="e1a19-114">installCommandSent</span></span>|<span data-ttu-id="e1a19-115">1</span><span class="sxs-lookup"><span data-stu-id="e1a19-115">1</span></span>|<span data-ttu-id="e1a19-116">已发送应用程序安装命令。</span><span class="sxs-lookup"><span data-stu-id="e1a19-116">Application install command was sent.</span></span>|
|<span data-ttu-id="e1a19-117">了</span><span class="sxs-lookup"><span data-stu-id="e1a19-117">installed</span></span>|<span data-ttu-id="e1a19-118">第三章</span><span class="sxs-lookup"><span data-stu-id="e1a19-118">3</span></span>|<span data-ttu-id="e1a19-119">已安装应用程序。</span><span class="sxs-lookup"><span data-stu-id="e1a19-119">Application installed.</span></span>|
|<span data-ttu-id="e1a19-120">#b0</span><span class="sxs-lookup"><span data-stu-id="e1a19-120">uninstalled</span></span>|<span data-ttu-id="e1a19-121">4</span><span class="sxs-lookup"><span data-stu-id="e1a19-121">4</span></span>|<span data-ttu-id="e1a19-122">已卸载应用程序。</span><span class="sxs-lookup"><span data-stu-id="e1a19-122">Application uninstalled.</span></span>|
|<span data-ttu-id="e1a19-123">userRequestedInstall</span><span class="sxs-lookup"><span data-stu-id="e1a19-123">userRequestedInstall</span></span>|<span data-ttu-id="e1a19-124">5</span><span class="sxs-lookup"><span data-stu-id="e1a19-124">5</span></span>|<span data-ttu-id="e1a19-125">用户请求安装</span><span class="sxs-lookup"><span data-stu-id="e1a19-125">User requested installation</span></span>|



