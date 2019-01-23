---
title: windowsPrivacyDataAccessLevel 枚举类型
description: 确定到特定 Windows 隐私数据类别的访问级别。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b5d6fed0897b22a6a6b478dc5d2b7954faca42b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410621"
---
# <a name="windowsprivacydataaccesslevel-enum-type"></a><span data-ttu-id="ccd91-103">windowsPrivacyDataAccessLevel 枚举类型</span><span class="sxs-lookup"><span data-stu-id="ccd91-103">windowsPrivacyDataAccessLevel enum type</span></span>

> <span data-ttu-id="ccd91-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="ccd91-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ccd91-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ccd91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ccd91-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ccd91-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ccd91-107">确定到特定 Windows 隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="ccd91-107">Determine the access level to specific Windows privacy data category.</span></span>

## <a name="members"></a><span data-ttu-id="ccd91-108">成员</span><span class="sxs-lookup"><span data-stu-id="ccd91-108">Members</span></span>
|<span data-ttu-id="ccd91-109">成员</span><span class="sxs-lookup"><span data-stu-id="ccd91-109">Member</span></span>|<span data-ttu-id="ccd91-110">值</span><span class="sxs-lookup"><span data-stu-id="ccd91-110">Value</span></span>|<span data-ttu-id="ccd91-111">说明</span><span class="sxs-lookup"><span data-stu-id="ccd91-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ccd91-112">notConfigured</span><span class="sxs-lookup"><span data-stu-id="ccd91-112">notConfigured</span></span>|<span data-ttu-id="ccd91-113">0</span><span class="sxs-lookup"><span data-stu-id="ccd91-113">0</span></span>|<span data-ttu-id="ccd91-114">指定无访问级别，没有方法。</span><span class="sxs-lookup"><span data-stu-id="ccd91-114">No access level specified, no intents.</span></span> <span data-ttu-id="ccd91-115">设备可能表现，可以如 UserInControl 或 ForceAllow 中所示。</span><span class="sxs-lookup"><span data-stu-id="ccd91-115">Device may behave either as in UserInControl or ForceAllow.</span></span> <span data-ttu-id="ccd91-116">它可能依赖的隐私数据已访问它们，Windows 版本和其他因素。</span><span class="sxs-lookup"><span data-stu-id="ccd91-116">It may depend on the privacy data been accessed, Windows versions and other factors.</span></span>|
|<span data-ttu-id="ccd91-117">forceAllow</span><span class="sxs-lookup"><span data-stu-id="ccd91-117">forceAllow</span></span>|<span data-ttu-id="ccd91-118">1</span><span class="sxs-lookup"><span data-stu-id="ccd91-118">1</span></span>|<span data-ttu-id="ccd91-119">应用程序将可以访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="ccd91-119">Apps will be allowed to access the specified privacy data.</span></span>|
|<span data-ttu-id="ccd91-120">forceDeny</span><span class="sxs-lookup"><span data-stu-id="ccd91-120">forceDeny</span></span>|<span data-ttu-id="ccd91-121">2</span><span class="sxs-lookup"><span data-stu-id="ccd91-121">2</span></span>|<span data-ttu-id="ccd91-122">应用程序将被拒绝访问指定的隐私数据。</span><span class="sxs-lookup"><span data-stu-id="ccd91-122">Apps will be denied to access specified privacy data.</span></span>|
|<span data-ttu-id="ccd91-123">userInControl</span><span class="sxs-lookup"><span data-stu-id="ccd91-123">userInControl</span></span>|<span data-ttu-id="ccd91-124">3</span><span class="sxs-lookup"><span data-stu-id="ccd91-124">3</span></span>|<span data-ttu-id="ccd91-125">应用程序尝试访问指定的隐私数据时，将会提示用户。</span><span class="sxs-lookup"><span data-stu-id="ccd91-125">Users will be prompted when apps try to access specified privacy data.</span></span>|




