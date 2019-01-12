---
title: runState 枚举类型
description: 指示设备管理脚本执行状态的类型。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c2178d492b7c341ffc8f5b7af85c78f46bd3f733
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956029"
---
# <a name="runstate-enum-type"></a><span data-ttu-id="8d55a-103">runState 枚举类型</span><span class="sxs-lookup"><span data-stu-id="8d55a-103">runState enum type</span></span>

> <span data-ttu-id="8d55a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="8d55a-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8d55a-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="8d55a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8d55a-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="8d55a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8d55a-107">指示设备管理脚本执行状态的类型。</span><span class="sxs-lookup"><span data-stu-id="8d55a-107">Indicates the type of execution status of the device management script.</span></span>
## <a name="members"></a><span data-ttu-id="8d55a-108">成员</span><span class="sxs-lookup"><span data-stu-id="8d55a-108">Members</span></span>
|<span data-ttu-id="8d55a-109">成员</span><span class="sxs-lookup"><span data-stu-id="8d55a-109">Member</span></span>|<span data-ttu-id="8d55a-110">值</span><span class="sxs-lookup"><span data-stu-id="8d55a-110">Value</span></span>|<span data-ttu-id="8d55a-111">说明</span><span class="sxs-lookup"><span data-stu-id="8d55a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8d55a-112">unknown</span><span class="sxs-lookup"><span data-stu-id="8d55a-112">unknown</span></span>|<span data-ttu-id="8d55a-113">0</span><span class="sxs-lookup"><span data-stu-id="8d55a-113">0</span></span>|<span data-ttu-id="8d55a-114">未知的结果。</span><span class="sxs-lookup"><span data-stu-id="8d55a-114">Unknown result.</span></span>|
|<span data-ttu-id="8d55a-115">success</span><span class="sxs-lookup"><span data-stu-id="8d55a-115">success</span></span>|<span data-ttu-id="8d55a-116">1</span><span class="sxs-lookup"><span data-stu-id="8d55a-116">1</span></span>|<span data-ttu-id="8d55a-117">成功运行脚本。</span><span class="sxs-lookup"><span data-stu-id="8d55a-117">Script is run successfully.</span></span>|
|<span data-ttu-id="8d55a-118">失败</span><span class="sxs-lookup"><span data-stu-id="8d55a-118">fail</span></span>|<span data-ttu-id="8d55a-119">2</span><span class="sxs-lookup"><span data-stu-id="8d55a-119">2</span></span>|<span data-ttu-id="8d55a-120">运行脚本失败。</span><span class="sxs-lookup"><span data-stu-id="8d55a-120">Script failed to run.</span></span>|





