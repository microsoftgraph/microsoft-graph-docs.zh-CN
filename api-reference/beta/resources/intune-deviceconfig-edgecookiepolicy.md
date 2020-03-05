---
title: edgeCookiePolicy 枚举类型
description: 指定允许在 Microsoft Edge 中使用哪些 cookie 的可能值。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: 1379c7d484c68d0f691fc57bd72923b3928becdb
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42530066"
---
# <a name="edgecookiepolicy-enum-type"></a><span data-ttu-id="1b779-103">edgeCookiePolicy 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1b779-103">edgeCookiePolicy enum type</span></span>

<span data-ttu-id="1b779-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="1b779-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1b779-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1b779-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1b779-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1b779-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1b779-107">指定允许在 Microsoft Edge 中使用哪些 cookie 的可能值。</span><span class="sxs-lookup"><span data-stu-id="1b779-107">Possible values to specify which cookies are allowed in Microsoft Edge.</span></span>

## <a name="members"></a><span data-ttu-id="1b779-108">成员</span><span class="sxs-lookup"><span data-stu-id="1b779-108">Members</span></span>
|<span data-ttu-id="1b779-109">成员</span><span class="sxs-lookup"><span data-stu-id="1b779-109">Member</span></span>|<span data-ttu-id="1b779-110">值</span><span class="sxs-lookup"><span data-stu-id="1b779-110">Value</span></span>|<span data-ttu-id="1b779-111">说明</span><span class="sxs-lookup"><span data-stu-id="1b779-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1b779-112">定制</span><span class="sxs-lookup"><span data-stu-id="1b779-112">userDefined</span></span>|<span data-ttu-id="1b779-113">0</span><span class="sxs-lookup"><span data-stu-id="1b779-113">0</span></span>|<span data-ttu-id="1b779-114">允许用户进行设置。</span><span class="sxs-lookup"><span data-stu-id="1b779-114">Allow the user to set.</span></span>|
|<span data-ttu-id="1b779-115">允许</span><span class="sxs-lookup"><span data-stu-id="1b779-115">allow</span></span>|<span data-ttu-id="1b779-116">1 </span><span class="sxs-lookup"><span data-stu-id="1b779-116">1</span></span>|<span data-ttu-id="1b779-117">允许.</span><span class="sxs-lookup"><span data-stu-id="1b779-117">Allow.</span></span>|
|<span data-ttu-id="1b779-118">blockThirdParty</span><span class="sxs-lookup"><span data-stu-id="1b779-118">blockThirdParty</span></span>|<span data-ttu-id="1b779-119">2 </span><span class="sxs-lookup"><span data-stu-id="1b779-119">2</span></span>|<span data-ttu-id="1b779-120">仅阻止第三方 cookie。</span><span class="sxs-lookup"><span data-stu-id="1b779-120">Block only third party cookies.</span></span>|
|<span data-ttu-id="1b779-121">blockAll</span><span class="sxs-lookup"><span data-stu-id="1b779-121">blockAll</span></span>|<span data-ttu-id="1b779-122">3 </span><span class="sxs-lookup"><span data-stu-id="1b779-122">3</span></span>|<span data-ttu-id="1b779-123">阻止所有 cookie。</span><span class="sxs-lookup"><span data-stu-id="1b779-123">Block all cookies.</span></span>|



