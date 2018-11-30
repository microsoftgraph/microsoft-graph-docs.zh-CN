---
title: safeSearchFilterType 枚举类型
description: 指定需要何种级别的安全搜索 （筛选成人内容）
ms.openlocfilehash: cf4f61e1b9e4e9f4fcfd94e6372ce517f3b735e6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27009424"
---
# <a name="safesearchfiltertype-enum-type"></a><span data-ttu-id="1f6a8-103">safeSearchFilterType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="1f6a8-103">safeSearchFilterType enum type</span></span>

> <span data-ttu-id="1f6a8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f6a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f6a8-105">指定需要何种级别的安全搜索 （筛选成人内容）</span><span class="sxs-lookup"><span data-stu-id="1f6a8-105">Specifies what level of safe search (filtering adult content) is required</span></span>
## <a name="members"></a><span data-ttu-id="1f6a8-106">成员</span><span class="sxs-lookup"><span data-stu-id="1f6a8-106">Members</span></span>
|<span data-ttu-id="1f6a8-107">成员</span><span class="sxs-lookup"><span data-stu-id="1f6a8-107">Member</span></span>|<span data-ttu-id="1f6a8-108">值</span><span class="sxs-lookup"><span data-stu-id="1f6a8-108">Value</span></span>|<span data-ttu-id="1f6a8-109">说明</span><span class="sxs-lookup"><span data-stu-id="1f6a8-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f6a8-110">用户定制</span><span class="sxs-lookup"><span data-stu-id="1f6a8-110">userDefined</span></span>|<span data-ttu-id="1f6a8-111">0</span><span class="sxs-lookup"><span data-stu-id="1f6a8-111">0</span></span>|<span data-ttu-id="1f6a8-112">用户定义，默认值、 没有用途。</span><span class="sxs-lookup"><span data-stu-id="1f6a8-112">User Defined, default value, no intent.</span></span>|
|<span data-ttu-id="1f6a8-113">严格</span><span class="sxs-lookup"><span data-stu-id="1f6a8-113">strict</span></span>|<span data-ttu-id="1f6a8-114">1</span><span class="sxs-lookup"><span data-stu-id="1f6a8-114">1</span></span>|<span data-ttu-id="1f6a8-115">严格，最高针对成人内容筛选。</span><span class="sxs-lookup"><span data-stu-id="1f6a8-115">Strict, highest filtering against adult content.</span></span>|
|<span data-ttu-id="1f6a8-116">中等</span><span class="sxs-lookup"><span data-stu-id="1f6a8-116">moderate</span></span>|<span data-ttu-id="1f6a8-117">2</span><span class="sxs-lookup"><span data-stu-id="1f6a8-117">2</span></span>|<span data-ttu-id="1f6a8-118">中等筛选成人内容 （有效的搜索结果将不会筛选）。</span><span class="sxs-lookup"><span data-stu-id="1f6a8-118">Moderate filtering against adult content (valid search results will not be filtered).</span></span>|



