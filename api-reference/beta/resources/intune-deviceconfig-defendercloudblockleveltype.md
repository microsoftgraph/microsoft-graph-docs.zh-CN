---
title: defenderCloudBlockLevelType 枚举类型
description: 云块级别的可能值
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: dc0e99f9d964e80410b10bc48e20ea0a5fd1d608
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36333588"
---
# <a name="defendercloudblockleveltype-enum-type"></a><span data-ttu-id="0adac-103">defenderCloudBlockLevelType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="0adac-103">defenderCloudBlockLevelType enum type</span></span>

> <span data-ttu-id="0adac-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0adac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0adac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0adac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0adac-106">云块级别的可能值</span><span class="sxs-lookup"><span data-stu-id="0adac-106">Possible values of Cloud Block Level</span></span>

## <a name="members"></a><span data-ttu-id="0adac-107">成员</span><span class="sxs-lookup"><span data-stu-id="0adac-107">Members</span></span>
|<span data-ttu-id="0adac-108">成员</span><span class="sxs-lookup"><span data-stu-id="0adac-108">Member</span></span>|<span data-ttu-id="0adac-109">值</span><span class="sxs-lookup"><span data-stu-id="0adac-109">Value</span></span>|<span data-ttu-id="0adac-110">说明</span><span class="sxs-lookup"><span data-stu-id="0adac-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0adac-111">notConfigured</span><span class="sxs-lookup"><span data-stu-id="0adac-111">notConfigured</span></span>|<span data-ttu-id="0adac-112">0</span><span class="sxs-lookup"><span data-stu-id="0adac-112">0</span></span>|<span data-ttu-id="0adac-113">默认值是, 使用默认的 Windows Defender 防病毒阻止级别, 并提供强大的检测功能, 而不会增加检测合法文件的风险</span><span class="sxs-lookup"><span data-stu-id="0adac-113">Default value, uses the default Windows Defender Antivirus blocking level and provides strong detection without increasing the risk of detecting legitimate files</span></span>|
|<span data-ttu-id="0adac-114">高效</span><span class="sxs-lookup"><span data-stu-id="0adac-114">high</span></span>|<span data-ttu-id="0adac-115">1</span><span class="sxs-lookup"><span data-stu-id="0adac-115">1</span></span>|<span data-ttu-id="0adac-116">High 适用于强级别的检测。</span><span class="sxs-lookup"><span data-stu-id="0adac-116">High applies a strong level of detection.</span></span>|
|<span data-ttu-id="0adac-117">highPlus</span><span class="sxs-lookup"><span data-stu-id="0adac-117">highPlus</span></span>|<span data-ttu-id="0adac-118">双面</span><span class="sxs-lookup"><span data-stu-id="0adac-118">2</span></span>|<span data-ttu-id="0adac-119">高级别 + 使用高级别, 并应用附加保护措施</span><span class="sxs-lookup"><span data-stu-id="0adac-119">High + uses the High level and applies addition protection measures</span></span>|
|<span data-ttu-id="0adac-120">zeroTolerance</span><span class="sxs-lookup"><span data-stu-id="0adac-120">zeroTolerance</span></span>|<span data-ttu-id="0adac-121">第三章</span><span class="sxs-lookup"><span data-stu-id="0adac-121">3</span></span>|<span data-ttu-id="0adac-122">零耐受性阻止所有未知可执行文件</span><span class="sxs-lookup"><span data-stu-id="0adac-122">Zero tolerance blocks all unknown executables</span></span>|



