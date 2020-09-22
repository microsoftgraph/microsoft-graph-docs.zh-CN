---
title: itemInsightsSettings 资源类型
description: 表示 itemInsights 的隐私设置。
localization_priority: Normal
author: simonhult
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 5d05a9fdf3a901fcddd55207bec373a3a0736afa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48089327"
---
# <a name="iteminsightssettings-resource-type"></a><span data-ttu-id="a3cc8-103">itemInsightsSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="a3cc8-103">itemInsightsSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a3cc8-104">表示 [itemInsights](iteminsights.md)的隐私设置，该设置配置从 microsoft Graph 派生的见解的可见性，在 microsoft 365 中的文档或网站) 的用户和其他项目 (。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-104">Represents privacy settings for [itemInsights](iteminsights.md), which configure the visibility of insights derived from Microsoft Graph, between users and other items (such as documents or sites) in Microsoft 365.</span></span>

## <a name="methods"></a><span data-ttu-id="a3cc8-105">方法</span><span class="sxs-lookup"><span data-stu-id="a3cc8-105">Methods</span></span>

| <span data-ttu-id="a3cc8-106">方法</span><span class="sxs-lookup"><span data-stu-id="a3cc8-106">Method</span></span>       | <span data-ttu-id="a3cc8-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="a3cc8-107">Return Type</span></span> | <span data-ttu-id="a3cc8-108">说明</span><span class="sxs-lookup"><span data-stu-id="a3cc8-108">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="a3cc8-109">Get</span><span class="sxs-lookup"><span data-stu-id="a3cc8-109">Get</span></span>](../api/iteminsightssettings-get.md)| [<span data-ttu-id="a3cc8-110">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="a3cc8-110">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="a3cc8-111">读取 **itemInsightsSettings** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-111">Read the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="a3cc8-112">更新</span><span class="sxs-lookup"><span data-stu-id="a3cc8-112">Update</span></span>](../api/iteminsightssettings-update.md)| [<span data-ttu-id="a3cc8-113">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="a3cc8-113">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="a3cc8-114">更新 **itemInsightsSettings** 对象。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-114">Update an **itemInsightsSettings** object.</span></span>|


## <a name="properties"></a><span data-ttu-id="a3cc8-115">属性</span><span class="sxs-lookup"><span data-stu-id="a3cc8-115">Properties</span></span>
| <span data-ttu-id="a3cc8-116">属性</span><span class="sxs-lookup"><span data-stu-id="a3cc8-116">Property</span></span>   | <span data-ttu-id="a3cc8-117">类型</span><span class="sxs-lookup"><span data-stu-id="a3cc8-117">Type</span></span>|<span data-ttu-id="a3cc8-118">说明</span><span class="sxs-lookup"><span data-stu-id="a3cc8-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a3cc8-119">isEnabledInOrganization</span><span class="sxs-lookup"><span data-stu-id="a3cc8-119">isEnabledInOrganization</span></span>|<span data-ttu-id="a3cc8-120">布尔</span><span class="sxs-lookup"><span data-stu-id="a3cc8-120">Boolean</span></span>| <span data-ttu-id="a3cc8-121">`true` 如果启用了组织项目见解，则为 `false` 如果对不例外的所有用户禁用了组织项目见解。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-121">`true` if organization item insights are enabled; `false` if organization item insights are disabled for all users without exceptions.</span></span> <span data-ttu-id="a3cc8-122">默认值为 `true`。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-122">Default is `true`.</span></span> <span data-ttu-id="a3cc8-123">可选。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-123">Optional.</span></span>|
|<span data-ttu-id="a3cc8-124">disabledForGroup</span><span class="sxs-lookup"><span data-stu-id="a3cc8-124">disabledForGroup</span></span>|<span data-ttu-id="a3cc8-125">字符串</span><span class="sxs-lookup"><span data-stu-id="a3cc8-125">String</span></span>| <span data-ttu-id="a3cc8-126">Azure AD 组的 ID，其中成员的项目见解已禁用。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-126">The ID of an Azure AD group, of which the members' item insights are disabled.</span></span> <span data-ttu-id="a3cc8-127">默认值为 `empty`。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-127">Default is `empty`.</span></span> <span data-ttu-id="a3cc8-128">可选。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-128">Optional.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a3cc8-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a3cc8-129">JSON representation</span></span>

<span data-ttu-id="a3cc8-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3cc8-130">Here is a JSON representation of the resource</span></span>
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


