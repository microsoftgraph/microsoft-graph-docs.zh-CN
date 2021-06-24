---
title: itemInsightsSettings 资源类型
description: 表示 itemInsights 的隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 80ca42440bcf365e051d9fb25fbc088af8a7f4bb
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53108822"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="9acc9-103">itemInsightsSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="9acc9-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9acc9-104">表示用于会议时间 [见解的 itemInsights](iteminsights.md) 的隐私 [设置和隐私设置](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 。</span><span class="sxs-lookup"><span data-stu-id="9acc9-104">Represents privacy settings for [itemInsights](iteminsights.md) and privacy setting for [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) .</span></span> <span data-ttu-id="9acc9-105">使用此 API 禁用/启用项目见解和会议时间见解的计算和可见性。</span><span class="sxs-lookup"><span data-stu-id="9acc9-105">Use this API to disable/enable calculation and visibility of item insights and meeting hours insights.</span></span> 

- <span data-ttu-id="9acc9-106">项目见解：计算用户与项目（如文档中的文档或网站）Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="9acc9-106">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="9acc9-107">会议时间见解：根据 Word、Excel、PowerPoint、电子邮件和 Microsoft 365 日历中的活动计算Outlook会议Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="9acc9-107">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

<span data-ttu-id="9acc9-108">使用 [userInsightsSettings](userinsightssettings.md) 资源可禁用/启用计算和查看用户的项目见解和会议时间见解。</span><span class="sxs-lookup"><span data-stu-id="9acc9-108">Use the [userInsightsSettings](userinsightssettings.md) resource to disable/enable calculation and visibility of item insights and meeting hours insights of a user.</span></span>

## <a name="methods"></a><span data-ttu-id="9acc9-109">方法</span><span class="sxs-lookup"><span data-stu-id="9acc9-109">Methods</span></span>

| <span data-ttu-id="9acc9-110">方法</span><span class="sxs-lookup"><span data-stu-id="9acc9-110">Method</span></span>       | <span data-ttu-id="9acc9-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="9acc9-111">Return Type</span></span> | <span data-ttu-id="9acc9-112">说明</span><span class="sxs-lookup"><span data-stu-id="9acc9-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="9acc9-113">获取</span><span class="sxs-lookup"><span data-stu-id="9acc9-113">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="9acc9-114">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="9acc9-114">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="9acc9-115">读取 **itemInsightsSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="9acc9-115">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="9acc9-116">更新</span><span class="sxs-lookup"><span data-stu-id="9acc9-116">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="9acc9-117">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="9acc9-117">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="9acc9-118">更新 **itemInsightsSettings** 对象。</span><span class="sxs-lookup"><span data-stu-id="9acc9-118">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="9acc9-119">属性</span><span class="sxs-lookup"><span data-stu-id="9acc9-119">Properties</span></span>
| <span data-ttu-id="9acc9-120">属性</span><span class="sxs-lookup"><span data-stu-id="9acc9-120">Property</span></span>   | <span data-ttu-id="9acc9-121">类型</span><span class="sxs-lookup"><span data-stu-id="9acc9-121">Type</span></span>|<span data-ttu-id="9acc9-122">说明</span><span class="sxs-lookup"><span data-stu-id="9acc9-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9acc9-123">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="9acc9-123">isEnabledInOrganization</span></span>|<span data-ttu-id="9acc9-124">布尔值</span><span class="sxs-lookup"><span data-stu-id="9acc9-124">Boolean</span></span>| <span data-ttu-id="9acc9-125">`true` 如果已启用组织项目见解; `false` 如果为所有用户禁用组织项目见解，则无例外。</span><span class="sxs-lookup"><span data-stu-id="9acc9-125">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="9acc9-126">默认值为“`true`”。</span><span class="sxs-lookup"><span data-stu-id="9acc9-126">Default is `true`.</span></span> <span data-ttu-id="9acc9-127">可选。</span><span class="sxs-lookup"><span data-stu-id="9acc9-127">Optional.</span></span>|
|<span data-ttu-id="9acc9-128">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="9acc9-128">disabledForGroup</span></span>|<span data-ttu-id="9acc9-129">字符串</span><span class="sxs-lookup"><span data-stu-id="9acc9-129">String</span></span>| <span data-ttu-id="9acc9-130">已禁用成员的项见解的 Azure AD 组的 ID。</span><span class="sxs-lookup"><span data-stu-id="9acc9-130">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="9acc9-131">默认值为“`empty`”。</span><span class="sxs-lookup"><span data-stu-id="9acc9-131">Default is `empty`.</span></span> <span data-ttu-id="9acc9-132">可选。</span><span class="sxs-lookup"><span data-stu-id="9acc9-132">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9acc9-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9acc9-133">JSON representation</span></span>

<span data-ttu-id="9acc9-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9acc9-134">Here is a JSON representation of the resource</span></span>
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


