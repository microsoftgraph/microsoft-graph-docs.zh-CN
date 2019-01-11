---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 283bb12c775b1215a1bcfecf4f248882a56573aa
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839499"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="c41eb-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="c41eb-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="c41eb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c41eb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c41eb-105">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="c41eb-105">Possible values of Cloud Block Level</span></span>
## <a name="members"></a><span data-ttu-id="c41eb-106">成员</span><span class="sxs-lookup"><span data-stu-id="c41eb-106">Members</span></span>
|<span data-ttu-id="c41eb-107">成员</span><span class="sxs-lookup"><span data-stu-id="c41eb-107">Member</span></span>|<span data-ttu-id="c41eb-108">值</span><span class="sxs-lookup"><span data-stu-id="c41eb-108">Value</span></span>|<span data-ttu-id="c41eb-109">Description</span><span class="sxs-lookup"><span data-stu-id="c41eb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c41eb-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="c41eb-110">notConfigured</span></span>|<span data-ttu-id="c41eb-111">0</span><span class="sxs-lookup"><span data-stu-id="c41eb-111">0</span></span>|<span data-ttu-id="c41eb-112">默认值，使用默认 Windows Defender 防病毒软件阻止级别，并提供强检测而不会提高检测的风险合法文件</span><span class="sxs-lookup"><span data-stu-id="c41eb-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="c41eb-113">高</span><span class="sxs-lookup"><span data-stu-id="c41eb-113">high</span></span>|<span data-ttu-id="c41eb-114">1</span><span class="sxs-lookup"><span data-stu-id="c41eb-114">1</span></span>|<span data-ttu-id="c41eb-115">高适用检测强的级别。</span><span class="sxs-lookup"><span data-stu-id="c41eb-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="c41eb-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="c41eb-116">highPlus</span></span>|<span data-ttu-id="c41eb-117">2</span><span class="sxs-lookup"><span data-stu-id="c41eb-117">2</span></span>|<span data-ttu-id="c41eb-118">高 + 使用的高级别和应用添加保护措施</span><span class="sxs-lookup"><span data-stu-id="c41eb-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="c41eb-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="c41eb-119">zeroTolerance</span></span>|<span data-ttu-id="c41eb-120">3</span><span class="sxs-lookup"><span data-stu-id="c41eb-120">3</span></span>|<span data-ttu-id="c41eb-121">零公差阻止所有未知的可执行文件</span><span class="sxs-lookup"><span data-stu-id="c41eb-121">Zero tolerance blocks all unknown executables</span></span>|



