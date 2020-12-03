---
title: itemInsightsSettings 资源类型
description: 表示 itemInsights 的隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: c84b2397c938997a3285d16612d090ae22444580
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49522725"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="e83e6-103">itemInsightsSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e83e6-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e83e6-104">表示用于会议时间见解的 [itemInsights](iteminsights.md) 和隐私设置的隐私设置。</span><span class="sxs-lookup"><span data-stu-id="e83e6-104">Represents privacy settings for [itemInsights](iteminsights.md) and privacy setting for meeting hours insights.</span></span> <span data-ttu-id="e83e6-105">使用此 API 可以禁用/启用项目见解和会议时间见解的计算和可见性。</span><span class="sxs-lookup"><span data-stu-id="e83e6-105">Use this API to disable/enable calculation and visibility of item insights and meeting hours insights.</span></span> 

- <span data-ttu-id="e83e6-106">Item insights：计算用户和项目（如 Microsoft 365 中的文档或网站）之间的关系。</span><span class="sxs-lookup"><span data-stu-id="e83e6-106">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="e83e6-107">会议时间见解：根据 Microsoft 365 中的 Word、Excel、PowerPoint、电子邮件和 Outlook 日历中的活动计算人员的日历会议时间。</span><span class="sxs-lookup"><span data-stu-id="e83e6-107">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

> [!NOTE]
> <span data-ttu-id="e83e6-108">向从11月2020开始的客户推出会议时间见解。</span><span class="sxs-lookup"><span data-stu-id="e83e6-108">Meeting hours insights are rolling out to customers starting November 2020.</span></span> 

## <a name="methods"></a><span data-ttu-id="e83e6-109">方法</span><span class="sxs-lookup"><span data-stu-id="e83e6-109">Methods</span></span>

| <span data-ttu-id="e83e6-110">方法</span><span class="sxs-lookup"><span data-stu-id="e83e6-110">Method</span></span>       | <span data-ttu-id="e83e6-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="e83e6-111">Return Type</span></span> | <span data-ttu-id="e83e6-112">说明</span><span class="sxs-lookup"><span data-stu-id="e83e6-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="e83e6-113">获取</span><span class="sxs-lookup"><span data-stu-id="e83e6-113">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="e83e6-114">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="e83e6-114">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="e83e6-115">读取 **itemInsightsSettings** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e83e6-115">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="e83e6-116">更新</span><span class="sxs-lookup"><span data-stu-id="e83e6-116">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="e83e6-117">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="e83e6-117">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="e83e6-118">更新 **itemInsightsSettings** 对象。</span><span class="sxs-lookup"><span data-stu-id="e83e6-118">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="e83e6-119">属性</span><span class="sxs-lookup"><span data-stu-id="e83e6-119">Properties</span></span>
| <span data-ttu-id="e83e6-120">属性</span><span class="sxs-lookup"><span data-stu-id="e83e6-120">Property</span></span>   | <span data-ttu-id="e83e6-121">类型</span><span class="sxs-lookup"><span data-stu-id="e83e6-121">Type</span></span>|<span data-ttu-id="e83e6-122">说明</span><span class="sxs-lookup"><span data-stu-id="e83e6-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="e83e6-123">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="e83e6-123">isEnabledInOrganization</span></span>|<span data-ttu-id="e83e6-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="e83e6-124">Boolean</span></span>| <span data-ttu-id="e83e6-125">`true` 如果启用了组织项目见解，则为 `false` 如果对不例外的所有用户禁用了组织项目见解。</span><span class="sxs-lookup"><span data-stu-id="e83e6-125">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="e83e6-126">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="e83e6-126">Default is `true`.</span></span> <span data-ttu-id="e83e6-127">可选。</span><span class="sxs-lookup"><span data-stu-id="e83e6-127">Optional.</span></span>|
|<span data-ttu-id="e83e6-128">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="e83e6-128">disabledForGroup</span></span>|<span data-ttu-id="e83e6-129">String</span><span class="sxs-lookup"><span data-stu-id="e83e6-129">String</span></span>| <span data-ttu-id="e83e6-130">Azure AD 组的 ID，其中成员的项目见解已禁用。</span><span class="sxs-lookup"><span data-stu-id="e83e6-130">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="e83e6-131">默认值为 `empty`。</span><span class="sxs-lookup"><span data-stu-id="e83e6-131">Default is `empty`.</span></span> <span data-ttu-id="e83e6-132">可选。</span><span class="sxs-lookup"><span data-stu-id="e83e6-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e83e6-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e83e6-133">JSON representation</span></span>

<span data-ttu-id="e83e6-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e83e6-134">Here is a JSON representation of the resource</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.itemInsightsSettings"
}-->

```json
{
  "isEnabledInOrganization": "Boolean",
  "disabledForGroup": "String"
}
```


