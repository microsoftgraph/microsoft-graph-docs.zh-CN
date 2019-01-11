---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定到特定 Windows 隐私数据类别的访问级别。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 74ab32a703422203fec7a6c9ed1bc035e01949a9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27888772"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="74c35-103">windowsPrivacyDataAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="74c35-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="74c35-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="74c35-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="74c35-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="74c35-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="74c35-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="74c35-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="74c35-107">确定到特定 Windows 隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="74c35-107">Determine the access level to specific Windows privacy data category.</span></span>
## <a name="members"></a><span data-ttu-id="74c35-108">成员</span><span class="sxs-lookup"><span data-stu-id="74c35-108">Members</span></span>
|<span data-ttu-id="74c35-109">成员</span><span class="sxs-lookup"><span data-stu-id="74c35-109">Member</span></span>|<span data-ttu-id="74c35-110">值</span><span class="sxs-lookup"><span data-stu-id="74c35-110">Value</span></span>|<span data-ttu-id="74c35-111">Description</span><span class="sxs-lookup"><span data-stu-id="74c35-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74c35-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="74c35-112">notConfigured</span></span>|<span data-ttu-id="74c35-113">0</span><span class="sxs-lookup"><span data-stu-id="74c35-113">0</span></span>|<span data-ttu-id="74c35-114">指定无访问级别，没有方法。</span><span class="sxs-lookup"><span data-stu-id="74c35-114">No access level specified, no intents.</span></span> <span data-ttu-id="74c35-115">设备可能表现，可以如 UserInControl 或 ForceAllow 中所示。</span><span class="sxs-lookup"><span data-stu-id="74c35-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="74c35-116">它可能依赖的隐私数据已访问它们，Windows 版本和其他因素。</span><span class="sxs-lookup"><span data-stu-id="74c35-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="74c35-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="74c35-117">forceAllow</span></span>|<span data-ttu-id="74c35-118">1</span><span class="sxs-lookup"><span data-stu-id="74c35-118">1</span></span>|<span data-ttu-id="74c35-119">应用程序将可以访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="74c35-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="74c35-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="74c35-120">forceDeny</span></span>|<span data-ttu-id="74c35-121">2</span><span class="sxs-lookup"><span data-stu-id="74c35-121">2</span></span>|<span data-ttu-id="74c35-122">应用程序将被拒绝访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="74c35-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="74c35-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="74c35-123">userInControl</span></span>|<span data-ttu-id="74c35-124">3</span><span class="sxs-lookup"><span data-stu-id="74c35-124">3</span></span>|<span data-ttu-id="74c35-125">应用程序尝试访问指定的隐私数据时，将会提示用户。</span><span class="sxs-lookup"><span data-stu-id="74c35-125">Users will be prompted when apps try to access specified privacy data.</span></span>|





