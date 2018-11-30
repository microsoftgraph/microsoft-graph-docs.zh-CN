---
title: deviceManagementExchangeAccessLevel 枚举类型
description: Exchange 中的访问级别。
ms.openlocfilehash: 2d45dab4cecc65fa7514eef178b134da05e466d0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27045519"
---
# <a name="devicemanagementexchangeaccesslevel-enum-type"></a><span data-ttu-id="5523c-103">deviceManagementExchangeAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="5523c-103">deviceManagementExchangeAccessLevel enum type</span></span>

> <span data-ttu-id="5523c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5523c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5523c-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5523c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5523c-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5523c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5523c-107">Exchange 中的访问级别。</span><span class="sxs-lookup"><span data-stu-id="5523c-107">Access Level in Exchange.</span></span>
## <a name="members"></a><span data-ttu-id="5523c-108">成员</span><span class="sxs-lookup"><span data-stu-id="5523c-108">Members</span></span>
|<span data-ttu-id="5523c-109">成员</span><span class="sxs-lookup"><span data-stu-id="5523c-109">Member</span></span>|<span data-ttu-id="5523c-110">值</span><span class="sxs-lookup"><span data-stu-id="5523c-110">Value</span></span>|<span data-ttu-id="5523c-111">说明</span><span class="sxs-lookup"><span data-stu-id="5523c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5523c-112">无</span><span class="sxs-lookup"><span data-stu-id="5523c-112">none</span></span>|<span data-ttu-id="5523c-113">0</span><span class="sxs-lookup"><span data-stu-id="5523c-113">0</span></span>|<span data-ttu-id="5523c-114">已在 Exchange 中不配置任何设备访问规则。</span><span class="sxs-lookup"><span data-stu-id="5523c-114">No device access rule has been configured in Exchange.</span></span>|
|<span data-ttu-id="5523c-115">允许</span><span class="sxs-lookup"><span data-stu-id="5523c-115">allow</span></span>|<span data-ttu-id="5523c-116">1</span><span class="sxs-lookup"><span data-stu-id="5523c-116">1</span></span>|<span data-ttu-id="5523c-117">允许 Exchange 设备访问。</span><span class="sxs-lookup"><span data-stu-id="5523c-117">Allow the device access to Exchange.</span></span>|
|<span data-ttu-id="5523c-118">阻止</span><span class="sxs-lookup"><span data-stu-id="5523c-118">block</span></span>|<span data-ttu-id="5523c-119">2</span><span class="sxs-lookup"><span data-stu-id="5523c-119">2</span></span>|<span data-ttu-id="5523c-120">阻止访问 Exchange 的设备。</span><span class="sxs-lookup"><span data-stu-id="5523c-120">Block the device from accessing Exchange.</span></span>|
|<span data-ttu-id="5523c-121">隔离</span><span class="sxs-lookup"><span data-stu-id="5523c-121">quarantine</span></span>|<span data-ttu-id="5523c-122">3</span><span class="sxs-lookup"><span data-stu-id="5523c-122">3</span></span>|<span data-ttu-id="5523c-123">在 Exchange 隔离设备。</span><span class="sxs-lookup"><span data-stu-id="5523c-123">Quarantine the device in Exchange.</span></span>|





