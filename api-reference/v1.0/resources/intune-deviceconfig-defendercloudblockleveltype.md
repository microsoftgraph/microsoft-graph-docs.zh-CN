---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 908ebaef963b4c7d8baaf8f1cb0ecfb316d33ad2
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031876"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="08482-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="08482-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="08482-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08482-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08482-105">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="08482-105">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="08482-106">成员</span><span class="sxs-lookup"><span data-stu-id="08482-106">Members</span></span>
|<span data-ttu-id="08482-107">成员</span><span class="sxs-lookup"><span data-stu-id="08482-107">Member</span></span>|<span data-ttu-id="08482-108">值</span><span class="sxs-lookup"><span data-stu-id="08482-108">Value</span></span>|<span data-ttu-id="08482-109">说明</span><span class="sxs-lookup"><span data-stu-id="08482-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08482-110">notConfigured</span><span class="sxs-lookup"><span data-stu-id="08482-110">notConfigured</span></span>|<span data-ttu-id="08482-111">0</span><span class="sxs-lookup"><span data-stu-id="08482-111">0</span></span>|<span data-ttu-id="08482-112">默认值是, 使用默认的 Windows Defender 防病毒阻止级别, 并提供强大的检测功能, 而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="08482-112">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="08482-113">高效</span><span class="sxs-lookup"><span data-stu-id="08482-113">high</span></span>|<span data-ttu-id="08482-114">1</span><span class="sxs-lookup"><span data-stu-id="08482-114">1</span></span>|<span data-ttu-id="08482-115">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="08482-115">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="08482-116">highPlus</span><span class="sxs-lookup"><span data-stu-id="08482-116">highPlus</span></span>|<span data-ttu-id="08482-117">双面</span><span class="sxs-lookup"><span data-stu-id="08482-117">2</span></span>|<span data-ttu-id="08482-118">高级别 + 使用高级别, 并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="08482-118">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="08482-119">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="08482-119">zeroTolerance</span></span>|<span data-ttu-id="08482-120">第三章</span><span class="sxs-lookup"><span data-stu-id="08482-120">3</span></span>|<span data-ttu-id="08482-121">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="08482-121">Zero tolerance blocks all unknown executables</span></span>|



