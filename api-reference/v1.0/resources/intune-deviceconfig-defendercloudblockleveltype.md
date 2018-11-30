---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
ms.openlocfilehash: 6ea336418a90a3d4caeab074cb71fce997ea1275
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009636"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="9978e-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="9978e-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="9978e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9978e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9978e-105">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="9978e-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="9978e-106">成员</span><span class="sxs-lookup"><span data-stu-id="9978e-106">Members</span></span>
|<span data-ttu-id="9978e-107">成员</span><span class="sxs-lookup"><span data-stu-id="9978e-107">Member</span></span>|<span data-ttu-id="9978e-108">值</span><span class="sxs-lookup"><span data-stu-id="9978e-108">Value</span></span>|<span data-ttu-id="9978e-109">说明</span><span class="sxs-lookup"><span data-stu-id="9978e-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9978e-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="9978e-110">notConfigured</span></span>|<span data-ttu-id="9978e-111">0</span><span class="sxs-lookup"><span data-stu-id="9978e-111">0</span></span>|<span data-ttu-id="9978e-112">默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强检测而不会提高检测的风险合法文件</span><span class="sxs-lookup"><span data-stu-id="9978e-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="9978e-113">高</span><span class="sxs-lookup"><span data-stu-id="9978e-113">high</span></span>|<span data-ttu-id="9978e-114">1</span><span class="sxs-lookup"><span data-stu-id="9978e-114">1</span></span>|<span data-ttu-id="9978e-115">高适用检测强的级别。</span><span class="sxs-lookup"><span data-stu-id="9978e-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="9978e-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="9978e-116">highPlus</span></span>|<span data-ttu-id="9978e-117">2</span><span class="sxs-lookup"><span data-stu-id="9978e-117">2</span></span>|<span data-ttu-id="9978e-118">高 + 使用的高级别和应用添加保护措施</span><span class="sxs-lookup"><span data-stu-id="9978e-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="9978e-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="9978e-119">zeroTolerance</span></span>|<span data-ttu-id="9978e-120">3</span><span class="sxs-lookup"><span data-stu-id="9978e-120">3</span></span>|<span data-ttu-id="9978e-121">零公差阻止所有未知的可执行文件</span><span class="sxs-lookup"><span data-stu-id="9978e-121">Zero tolerance blocks all unknown executables</span></span>|



