---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
ms.openlocfilehash: 70e43e9659e7dd7be1d3c0a190e21d80d7b8dc41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046983"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="63993-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="63993-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="63993-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="63993-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="63993-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="63993-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="63993-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="63993-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="63993-107">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="63993-107">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="63993-108">成员</span><span class="sxs-lookup"><span data-stu-id="63993-108">Members</span></span>
|<span data-ttu-id="63993-109">成员</span><span class="sxs-lookup"><span data-stu-id="63993-109">Member</span></span>|<span data-ttu-id="63993-110">值</span><span class="sxs-lookup"><span data-stu-id="63993-110">Value</span></span>|<span data-ttu-id="63993-111">说明</span><span class="sxs-lookup"><span data-stu-id="63993-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63993-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="63993-112">notConfigured</span></span>|<span data-ttu-id="63993-113">0</span><span class="sxs-lookup"><span data-stu-id="63993-113">0</span></span>|<span data-ttu-id="63993-114">默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强检测而不会提高检测的风险合法文件</span><span class="sxs-lookup"><span data-stu-id="63993-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="63993-115">高</span><span class="sxs-lookup"><span data-stu-id="63993-115">high</span></span>|<span data-ttu-id="63993-116">1</span><span class="sxs-lookup"><span data-stu-id="63993-116">1</span></span>|<span data-ttu-id="63993-117">高适用检测强的级别。</span><span class="sxs-lookup"><span data-stu-id="63993-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="63993-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="63993-118">highPlus</span></span>|<span data-ttu-id="63993-119">2</span><span class="sxs-lookup"><span data-stu-id="63993-119">2</span></span>|<span data-ttu-id="63993-120">高 + 使用的高级别和应用添加保护措施</span><span class="sxs-lookup"><span data-stu-id="63993-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="63993-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="63993-121">zeroTolerance</span></span>|<span data-ttu-id="63993-122">3</span><span class="sxs-lookup"><span data-stu-id="63993-122">3</span></span>|<span data-ttu-id="63993-123">零公差阻止所有未知的可执行文件</span><span class="sxs-lookup"><span data-stu-id="63993-123">Zero tolerance blocks all unknown executables</span></span>|





