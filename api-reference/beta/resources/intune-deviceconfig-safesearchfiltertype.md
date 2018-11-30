---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
ms.openlocfilehash: 71a59574fd98e2571a33e58415acb612f32326a2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042728"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="cfdfa-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="cfdfa-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="cfdfa-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cfdfa-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cfdfa-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cfdfa-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cfdfa-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cfdfa-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cfdfa-107">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="cfdfa-107">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="cfdfa-108">成员</span><span class="sxs-lookup"><span data-stu-id="cfdfa-108">Members</span></span>
|<span data-ttu-id="cfdfa-109">成员</span><span class="sxs-lookup"><span data-stu-id="cfdfa-109">Member</span></span>|<span data-ttu-id="cfdfa-110">值</span><span class="sxs-lookup"><span data-stu-id="cfdfa-110">Value</span></span>|<span data-ttu-id="cfdfa-111">说明</span><span class="sxs-lookup"><span data-stu-id="cfdfa-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cfdfa-112">用户定制</span><span class="sxs-lookup"><span data-stu-id="cfdfa-112">userDefined</span></span>|<span data-ttu-id="cfdfa-113">0</span><span class="sxs-lookup"><span data-stu-id="cfdfa-113">0</span></span>|<span data-ttu-id="cfdfa-114">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="cfdfa-114">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="cfdfa-115">严格</span><span class="sxs-lookup"><span data-stu-id="cfdfa-115">strict</span></span>|<span data-ttu-id="cfdfa-116">1</span><span class="sxs-lookup"><span data-stu-id="cfdfa-116">1</span></span>|<span data-ttu-id="cfdfa-117">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="cfdfa-117">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="cfdfa-118">中等</span><span class="sxs-lookup"><span data-stu-id="cfdfa-118">moderate</span></span>|<span data-ttu-id="cfdfa-119">2</span><span class="sxs-lookup"><span data-stu-id="cfdfa-119">2</span></span>|<span data-ttu-id="cfdfa-120">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="cfdfa-120">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|





