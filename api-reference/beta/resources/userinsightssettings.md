---
title: userInsightsSettings 资源类型
description: 表示项目见解和会议时间见解的用户隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5ecc9277d0bd98df99387a5dd222998074c6eb1b
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109090"
---
# <a name="userinsightssettings-resource-type"></a><span data-ttu-id="cf96d-103">userInsightsSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf96d-103">userInsightsSettings resource type</span></span>

<span data-ttu-id="cf96d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cf96d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cf96d-105">表示 [itemInsights](iteminsights.md) 和会议时间见解 [的用户隐私设置](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) 。</span><span class="sxs-lookup"><span data-stu-id="cf96d-105">Represents user privacy settings for [itemInsights](iteminsights.md) and [meeting hours insights](https://support.microsoft.com/en-us/office/update-your-meeting-hours-using-the-profile-card-0613d113-d7c1-4faa-bb11-c8ba30a78ef1) .</span></span> <span data-ttu-id="cf96d-106">使用此资源可禁用/启用计算和查看用户的项目见解和会议时间见解。</span><span class="sxs-lookup"><span data-stu-id="cf96d-106">Use this resource to disable/enable calculation and visibility of item insights and meeting hours insights of a user.</span></span> 

- <span data-ttu-id="cf96d-107">项目见解：计算用户与项目（如文档中的文档或网站）Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="cf96d-107">Item insights: Calculates relationship between users and items such as documents or sites in Microsoft 365.</span></span>  
- <span data-ttu-id="cf96d-108">会议时间见解：根据 Word、Excel、PowerPoint、电子邮件和 Microsoft 365 日历中的活动计算Outlook会议Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="cf96d-108">Meeting hours insights: Calculates a person's calendar meeting hours based on activities in Word, Excel, PowerPoint, email, and Outlook calendar in Microsoft 365.</span></span>

<span data-ttu-id="cf96d-109">使用 [itemInsightsSettings](iteminsightssettings.md) 资源在组织级别禁用/启用项目见解和会议小时数见解的计算和可见性。</span><span class="sxs-lookup"><span data-stu-id="cf96d-109">Use the [itemInsightsSettings](iteminsightssettings.md) resource to disable/enable calculation and visibility of item insights and meeting hours insights at an organization level.</span></span>

## <a name="methods"></a><span data-ttu-id="cf96d-110">方法</span><span class="sxs-lookup"><span data-stu-id="cf96d-110">Methods</span></span>

| <span data-ttu-id="cf96d-111">方法</span><span class="sxs-lookup"><span data-stu-id="cf96d-111">Method</span></span>                                                 | <span data-ttu-id="cf96d-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="cf96d-112">Return Type</span></span>                                                   | <span data-ttu-id="cf96d-113">说明</span><span class="sxs-lookup"><span data-stu-id="cf96d-113">Description</span></span>                                                                                        |
|:-------------------------------------------------------|:--------------------------------------------------------------|:---------------------------------------------------------------------------------------------------|
| [<span data-ttu-id="cf96d-114">获取</span><span class="sxs-lookup"><span data-stu-id="cf96d-114">Get</span></span>](../api/userinsightssettings-get.md)       | [<span data-ttu-id="cf96d-115">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="cf96d-115">userInsightsSettings</span></span>](userinsightssettings.md) | <span data-ttu-id="cf96d-116">读取 **userinsightssettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="cf96d-116">Read the properties of a **userinsightssettings** object.</span></span>  |
| [<span data-ttu-id="cf96d-117">更新</span><span class="sxs-lookup"><span data-stu-id="cf96d-117">Update</span></span>](../api/userinsightssettings-update.md) | [<span data-ttu-id="cf96d-118">userInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="cf96d-118">userInsightsSettings</span></span>](userinsightssettings.md) | <span data-ttu-id="cf96d-119">更新 **userinsightssettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="cf96d-119">Update the properties of a **userinsightssettings** object.</span></span> |

## <a name="properties"></a><span data-ttu-id="cf96d-120">属性</span><span class="sxs-lookup"><span data-stu-id="cf96d-120">Properties</span></span>
| <span data-ttu-id="cf96d-121">属性</span><span class="sxs-lookup"><span data-stu-id="cf96d-121">Property</span></span>                   | <span data-ttu-id="cf96d-122">类型</span><span class="sxs-lookup"><span data-stu-id="cf96d-122">Type</span></span>                                                  | <span data-ttu-id="cf96d-123">说明</span><span class="sxs-lookup"><span data-stu-id="cf96d-123">Description</span></span>                                                                                                                                                         |
|----------------------------|-------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="cf96d-124">isEnabled</span><span class="sxs-lookup"><span data-stu-id="cf96d-124">isEnabled</span></span>     | <span data-ttu-id="cf96d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf96d-125">Boolean</span></span>  |  <span data-ttu-id="cf96d-126">`true` 如果用户的 **itemInsights** 和会议时间见解已启用; `false` 如果禁用了 **用户的 itemInsights** 和会议小时数见解。</span><span class="sxs-lookup"><span data-stu-id="cf96d-126">`true` if user's **itemInsights** and meeting hours insights are enabled; `false` if user's **itemInsights** and meeting hours insights are disabled.</span></span> <span data-ttu-id="cf96d-127">默认值为“`true`”。</span><span class="sxs-lookup"><span data-stu-id="cf96d-127">Default is `true`.</span></span> <span data-ttu-id="cf96d-128">可选。</span><span class="sxs-lookup"><span data-stu-id="cf96d-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cf96d-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf96d-129">JSON representation</span></span>

<span data-ttu-id="cf96d-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf96d-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.userInsightsSettings"
}-->

```json
{
  "isEnabled": "Boolean"
}
```


