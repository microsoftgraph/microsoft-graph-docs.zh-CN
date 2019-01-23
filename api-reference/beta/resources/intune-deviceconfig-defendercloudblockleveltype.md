---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b309184623cff19e44ee5afea311d46fa89210fb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425909"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="b7b6c-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="b7b6c-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="b7b6c-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b7b6c-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b7b6c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b7b6c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b7b6c-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b7b6c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7b6c-107">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="b7b6c-107">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="b7b6c-108">成员</span><span class="sxs-lookup"><span data-stu-id="b7b6c-108">Members</span></span>
|<span data-ttu-id="b7b6c-109">成员</span><span class="sxs-lookup"><span data-stu-id="b7b6c-109">Member</span></span>|<span data-ttu-id="b7b6c-110">值</span><span class="sxs-lookup"><span data-stu-id="b7b6c-110">Value</span></span>|<span data-ttu-id="b7b6c-111">说明</span><span class="sxs-lookup"><span data-stu-id="b7b6c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b7b6c-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="b7b6c-112">notConfigured</span></span>|<span data-ttu-id="b7b6c-113">0</span><span class="sxs-lookup"><span data-stu-id="b7b6c-113">0</span></span>|<span data-ttu-id="b7b6c-114">默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强检测而不会提高检测的风险合法文件</span><span class="sxs-lookup"><span data-stu-id="b7b6c-114">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="b7b6c-115">高</span><span class="sxs-lookup"><span data-stu-id="b7b6c-115">high</span></span>|<span data-ttu-id="b7b6c-116">1</span><span class="sxs-lookup"><span data-stu-id="b7b6c-116">1</span></span>|<span data-ttu-id="b7b6c-117">高适用检测强的级别。</span><span class="sxs-lookup"><span data-stu-id="b7b6c-117">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="b7b6c-118">highPlus</span><span class="sxs-lookup"><span data-stu-id="b7b6c-118">highPlus</span></span>|<span data-ttu-id="b7b6c-119">2</span><span class="sxs-lookup"><span data-stu-id="b7b6c-119">2</span></span>|<span data-ttu-id="b7b6c-120">高 + 使用的高级别和应用添加保护措施</span><span class="sxs-lookup"><span data-stu-id="b7b6c-120">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="b7b6c-121">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="b7b6c-121">zeroTolerance</span></span>|<span data-ttu-id="b7b6c-122">3</span><span class="sxs-lookup"><span data-stu-id="b7b6c-122">3</span></span>|<span data-ttu-id="b7b6c-123">零公差阻止所有未知的可执行文件</span><span class="sxs-lookup"><span data-stu-id="b7b6c-123">Zero tolerance blocks all unknown executables</span></span>|




