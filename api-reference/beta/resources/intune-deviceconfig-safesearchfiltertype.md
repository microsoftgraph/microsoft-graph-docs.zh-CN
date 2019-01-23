---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4493c71b48a0f5ff4b0c48307504087c722393e1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403481"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="59171-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="59171-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="59171-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="59171-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="59171-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="59171-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="59171-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="59171-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="59171-107">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="59171-107">Specifies what level of safe search (filtering adult content) is required</span></span>

## <a name="members"></a><span data-ttu-id="59171-108">成员</span><span class="sxs-lookup"><span data-stu-id="59171-108">Members</span></span>
|<span data-ttu-id="59171-109">成员</span><span class="sxs-lookup"><span data-stu-id="59171-109">Member</span></span>|<span data-ttu-id="59171-110">值</span><span class="sxs-lookup"><span data-stu-id="59171-110">Value</span></span>|<span data-ttu-id="59171-111">说明</span><span class="sxs-lookup"><span data-stu-id="59171-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="59171-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="59171-112">userDefined</span></span>|<span data-ttu-id="59171-113">0</span><span class="sxs-lookup"><span data-stu-id="59171-113">0</span></span>|<span data-ttu-id="59171-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="59171-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="59171-115">严格</span><span class="sxs-lookup"><span data-stu-id="59171-115">strict</span></span>|<span data-ttu-id="59171-116">1</span><span class="sxs-lookup"><span data-stu-id="59171-116">1</span></span>|<span data-ttu-id="59171-117">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="59171-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="59171-118">中等</span><span class="sxs-lookup"><span data-stu-id="59171-118">moderate</span></span>|<span data-ttu-id="59171-119">2</span><span class="sxs-lookup"><span data-stu-id="59171-119">2</span></span>|<span data-ttu-id="59171-120">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="59171-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|




