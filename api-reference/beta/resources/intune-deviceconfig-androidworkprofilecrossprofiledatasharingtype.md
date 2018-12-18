---
title: androidWorkProfileCrossProfileDataSharingType 枚举类型
description: Android 工作模板跨共享类型的配置文件数据。
author: tfitzmac
ms.openlocfilehash: 278d9af142128003cf05b69f1cce340eb155f973
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27308148"
---
# <a name="androidworkprofilecrossprofiledatasharingtype-enum-type"></a><span data-ttu-id="fc173-103">androidWorkProfileCrossProfileDataSharingType 枚举类型</span><span class="sxs-lookup"><span data-stu-id="fc173-103">androidWorkProfileCrossProfileDataSharingType enum type</span></span>

> <span data-ttu-id="fc173-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fc173-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fc173-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fc173-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc173-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fc173-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc173-107">Android 工作模板跨共享类型的配置文件数据。</span><span class="sxs-lookup"><span data-stu-id="fc173-107">Android Work Profile cross profile data sharing type.</span></span>
## <a name="members"></a><span data-ttu-id="fc173-108">成员</span><span class="sxs-lookup"><span data-stu-id="fc173-108">Members</span></span>
|<span data-ttu-id="fc173-109">成员</span><span class="sxs-lookup"><span data-stu-id="fc173-109">Member</span></span>|<span data-ttu-id="fc173-110">值</span><span class="sxs-lookup"><span data-stu-id="fc173-110">Value</span></span>|<span data-ttu-id="fc173-111">说明</span><span class="sxs-lookup"><span data-stu-id="fc173-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc173-112">deviceDefault</span><span class="sxs-lookup"><span data-stu-id="fc173-112">deviceDefault</span></span>|<span data-ttu-id="fc173-113">0</span><span class="sxs-lookup"><span data-stu-id="fc173-113">0</span></span>|<span data-ttu-id="fc173-114">设备默认值，没有用途。</span><span class="sxs-lookup"><span data-stu-id="fc173-114">Device default value, no intent.</span></span>|
|<span data-ttu-id="fc173-115">preventAny</span><span class="sxs-lookup"><span data-stu-id="fc173-115">preventAny</span></span>|<span data-ttu-id="fc173-116">1</span><span class="sxs-lookup"><span data-stu-id="fc173-116">1</span></span>|<span data-ttu-id="fc173-117">防止任何共享。</span><span class="sxs-lookup"><span data-stu-id="fc173-117">Prevent any sharing.</span></span>|
|<span data-ttu-id="fc173-118">allowPersonalToWork</span><span class="sxs-lookup"><span data-stu-id="fc173-118">allowPersonalToWork</span></span>|<span data-ttu-id="fc173-119">2</span><span class="sxs-lookup"><span data-stu-id="fc173-119">2</span></span>|<span data-ttu-id="fc173-120">允许共享个人配置文件中的请求，以配置文件的数据。</span><span class="sxs-lookup"><span data-stu-id="fc173-120">Allow data sharing request from personal profile to work profile.</span></span>|
|<span data-ttu-id="fc173-121">noRestrictions</span><span class="sxs-lookup"><span data-stu-id="fc173-121">noRestrictions</span></span>|<span data-ttu-id="fc173-122">3</span><span class="sxs-lookup"><span data-stu-id="fc173-122">3</span></span>|<span data-ttu-id="fc173-123">共享没有限制。</span><span class="sxs-lookup"><span data-stu-id="fc173-123">No restrictions on sharing.</span></span>|





