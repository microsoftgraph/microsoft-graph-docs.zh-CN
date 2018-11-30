---
title: runState 枚举类型
description: 指示设备管理脚本执行状态的类型。
ms.openlocfilehash: 74802b347d83db0785c5c132315071024d944ddc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041256"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="8f1f2-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8f1f2-103">runState enum type</span></span>

> <span data-ttu-id="8f1f2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f1f2-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f1f2-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f1f2-107">指示设备管理脚本执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="8f1f2-108">成员</span><span class="sxs-lookup"><span data-stu-id="8f1f2-108">Members</span></span>
|<span data-ttu-id="8f1f2-109">成员</span><span class="sxs-lookup"><span data-stu-id="8f1f2-109">Member</span></span>|<span data-ttu-id="8f1f2-110">值</span><span class="sxs-lookup"><span data-stu-id="8f1f2-110">Value</span></span>|<span data-ttu-id="8f1f2-111">说明</span><span class="sxs-lookup"><span data-stu-id="8f1f2-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f1f2-112">unknown</span><span class="sxs-lookup"><span data-stu-id="8f1f2-112">unknown</span></span>|<span data-ttu-id="8f1f2-113">0</span><span class="sxs-lookup"><span data-stu-id="8f1f2-113">0</span></span>|<span data-ttu-id="8f1f2-114">未知的结果。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-114">Unknown result.</span></span>|
|<span data-ttu-id="8f1f2-115">success</span><span class="sxs-lookup"><span data-stu-id="8f1f2-115">success</span></span>|<span data-ttu-id="8f1f2-116">1</span><span class="sxs-lookup"><span data-stu-id="8f1f2-116">1</span></span>|<span data-ttu-id="8f1f2-117">成功运行脚本。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-117">Script is run successfully.</span></span>|
|<span data-ttu-id="8f1f2-118">失败</span><span class="sxs-lookup"><span data-stu-id="8f1f2-118">fail</span></span>|<span data-ttu-id="8f1f2-119">2</span><span class="sxs-lookup"><span data-stu-id="8f1f2-119">2</span></span>|<span data-ttu-id="8f1f2-120">运行脚本失败。</span><span class="sxs-lookup"><span data-stu-id="8f1f2-120">Script failed to run.</span></span>|





