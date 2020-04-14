---
title: edgeCookiePolicy 枚举类型
description: 指定允许在 Microsoft Edge 中使用哪些 cookie 的可能值。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 0066e7a64cd63425352787b5bcc33bfc32fe8342
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43386460"
---
# <a name="edgecookiepolicy-enum-type"></a><span data-ttu-id="fc3bc-103">edgeCookiePolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fc3bc-103">edgeCookiePolicy enum type</span></span>

<span data-ttu-id="fc3bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc3bc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fc3bc-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fc3bc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fc3bc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc3bc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc3bc-107">指定允许在 Microsoft Edge 中使用哪些 cookie 的可能值。</span><span class="sxs-lookup"><span data-stu-id="fc3bc-107">Possible values to specify which cookies are allowed in Microsoft Edge.</span></span>

## <a name="members"></a><span data-ttu-id="fc3bc-108">成员</span><span class="sxs-lookup"><span data-stu-id="fc3bc-108">Members</span></span>
|<span data-ttu-id="fc3bc-109">成员</span><span class="sxs-lookup"><span data-stu-id="fc3bc-109">Member</span></span>|<span data-ttu-id="fc3bc-110">值</span><span class="sxs-lookup"><span data-stu-id="fc3bc-110">Value</span></span>|<span data-ttu-id="fc3bc-111">说明</span><span class="sxs-lookup"><span data-stu-id="fc3bc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc3bc-112">定制</span><span class="sxs-lookup"><span data-stu-id="fc3bc-112">userDefined</span></span>|<span data-ttu-id="fc3bc-113">0</span><span class="sxs-lookup"><span data-stu-id="fc3bc-113">0</span></span>|<span data-ttu-id="fc3bc-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="fc3bc-114">Allow the user to set.</span></span>|
|<span data-ttu-id="fc3bc-115">允许</span><span class="sxs-lookup"><span data-stu-id="fc3bc-115">allow</span></span>|<span data-ttu-id="fc3bc-116">1</span><span class="sxs-lookup"><span data-stu-id="fc3bc-116">1</span></span>|<span data-ttu-id="fc3bc-117">允许.</span><span class="sxs-lookup"><span data-stu-id="fc3bc-117">Allow.</span></span>|
|<span data-ttu-id="fc3bc-118">blockThirdParty</span><span class="sxs-lookup"><span data-stu-id="fc3bc-118">blockThirdParty</span></span>|<span data-ttu-id="fc3bc-119">双面</span><span class="sxs-lookup"><span data-stu-id="fc3bc-119">2</span></span>|<span data-ttu-id="fc3bc-120">仅阻止第三方 cookie。</span><span class="sxs-lookup"><span data-stu-id="fc3bc-120">Block only third party cookies.</span></span>|
|<span data-ttu-id="fc3bc-121">blockAll</span><span class="sxs-lookup"><span data-stu-id="fc3bc-121">blockAll</span></span>|<span data-ttu-id="fc3bc-122">第三章</span><span class="sxs-lookup"><span data-stu-id="fc3bc-122">3</span></span>|<span data-ttu-id="fc3bc-123">阻止所有 cookie。</span><span class="sxs-lookup"><span data-stu-id="fc3bc-123">Block all cookies.</span></span>|



