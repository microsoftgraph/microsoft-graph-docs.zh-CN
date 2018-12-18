---
title: runState 枚举类型
description: 指示设备管理脚本执行状态的类型。
author: tfitzmac
ms.openlocfilehash: 87c845c02bd5a1571ab2f6382acbcc92cf81170d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27349271"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="bc640-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="bc640-103">runState enum type</span></span>

> <span data-ttu-id="bc640-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bc640-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bc640-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bc640-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="bc640-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="bc640-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bc640-107">指示设备管理脚本执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="bc640-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="bc640-108">成员</span><span class="sxs-lookup"><span data-stu-id="bc640-108">Members</span></span>
|<span data-ttu-id="bc640-109">成员</span><span class="sxs-lookup"><span data-stu-id="bc640-109">Member</span></span>|<span data-ttu-id="bc640-110">值</span><span class="sxs-lookup"><span data-stu-id="bc640-110">Value</span></span>|<span data-ttu-id="bc640-111">说明</span><span class="sxs-lookup"><span data-stu-id="bc640-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bc640-112">unknown</span><span class="sxs-lookup"><span data-stu-id="bc640-112">unknown</span></span>|<span data-ttu-id="bc640-113">0</span><span class="sxs-lookup"><span data-stu-id="bc640-113">0</span></span>|<span data-ttu-id="bc640-114">未知的结果。</span><span class="sxs-lookup"><span data-stu-id="bc640-114">Unknown result.</span></span>|
|<span data-ttu-id="bc640-115">success</span><span class="sxs-lookup"><span data-stu-id="bc640-115">success</span></span>|<span data-ttu-id="bc640-116">1</span><span class="sxs-lookup"><span data-stu-id="bc640-116">1</span></span>|<span data-ttu-id="bc640-117">成功运行脚本。</span><span class="sxs-lookup"><span data-stu-id="bc640-117">Script is run successfully.</span></span>|
|<span data-ttu-id="bc640-118">失败</span><span class="sxs-lookup"><span data-stu-id="bc640-118">fail</span></span>|<span data-ttu-id="bc640-119">2</span><span class="sxs-lookup"><span data-stu-id="bc640-119">2</span></span>|<span data-ttu-id="bc640-120">运行脚本失败。</span><span class="sxs-lookup"><span data-stu-id="bc640-120">Script failed to run.</span></span>|





