---
title: organizationSettings 资源类型
description: 包含适用于组织或其中用户对象的设置。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 105a57c7cb5827e9017df7494d32802ef7ac6fa5
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50158322"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="89794-103">organizationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="89794-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89794-104">包含适用于组织 [或](organization.md) 应用于组织中 [用户对象的](user.md) 设置。</span><span class="sxs-lookup"><span data-stu-id="89794-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="89794-105">方法</span><span class="sxs-lookup"><span data-stu-id="89794-105">Methods</span></span>

| <span data-ttu-id="89794-106">方法</span><span class="sxs-lookup"><span data-stu-id="89794-106">Method</span></span>       | <span data-ttu-id="89794-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="89794-107">Return Type</span></span> | <span data-ttu-id="89794-108">说明</span><span class="sxs-lookup"><span data-stu-id="89794-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="89794-109">获取组织设置</span><span class="sxs-lookup"><span data-stu-id="89794-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="89794-110">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="89794-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="89794-111">读取组织设置对象。</span><span class="sxs-lookup"><span data-stu-id="89794-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="89794-112">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="89794-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="89794-113">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="89794-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="89794-114">通过发布到 **profileCardProperty** 对象集合创建新的 **profileCardProperty。**</span><span class="sxs-lookup"><span data-stu-id="89794-114">Create a new **profileCardProperty** by posting to the **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="89794-115">列出 profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="89794-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="89794-116">[profileCardProperty](profilecardproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89794-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="89794-117">获取 **profileCardProperty** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="89794-117">Get a **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="89794-118">获取 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="89794-118">Get itemInsightsSettings</span></span>](../api/iteminsightssettings-get.md) | [<span data-ttu-id="89794-119">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="89794-119">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="89794-120">获取 **itemInsightsSettings 对象** 的属性。</span><span class="sxs-lookup"><span data-stu-id="89794-120">Get the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="89794-121">更新 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="89794-121">Update itemInsightsSettings</span></span>](../api/iteminsightssettings-update.md) | [<span data-ttu-id="89794-122">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="89794-122">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="89794-123">更新指定 **itemInsightsSettings 资源** 的属性。</span><span class="sxs-lookup"><span data-stu-id="89794-123">Update the properties of the specified **itemInsightsSettings** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="89794-124">属性</span><span class="sxs-lookup"><span data-stu-id="89794-124">Properties</span></span>

<span data-ttu-id="89794-125">无。</span><span class="sxs-lookup"><span data-stu-id="89794-125">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="89794-126">关系</span><span class="sxs-lookup"><span data-stu-id="89794-126">Relationships</span></span>

| <span data-ttu-id="89794-127">关系</span><span class="sxs-lookup"><span data-stu-id="89794-127">Relationship</span></span> | <span data-ttu-id="89794-128">类型</span><span class="sxs-lookup"><span data-stu-id="89794-128">Type</span></span>        | <span data-ttu-id="89794-129">说明</span><span class="sxs-lookup"><span data-stu-id="89794-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="89794-130">id</span><span class="sxs-lookup"><span data-stu-id="89794-130">id</span></span> |<span data-ttu-id="89794-131">String</span><span class="sxs-lookup"><span data-stu-id="89794-131">String</span></span>| <span data-ttu-id="89794-132">组织的设置对象的 ID。</span><span class="sxs-lookup"><span data-stu-id="89794-132">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="89794-133">profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="89794-133">profileCardProperties</span></span>|<span data-ttu-id="89794-134">[profileCardProperty](profilecardproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89794-134">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="89794-135">包含管理员已定义为在 Microsoft 365 配置文件卡上可见的属性的集合。</span><span class="sxs-lookup"><span data-stu-id="89794-135">Contains a collection of the properties an administrator has defined as visible on the Microsoft 365 profile card.</span></span> <span data-ttu-id="89794-136">[获取组织设置](../api/organizationsettings-get.md) 将返回为组织的配置文件卡配置的属性。</span><span class="sxs-lookup"><span data-stu-id="89794-136">[Get organization settings](../api/organizationsettings-get.md) returns the properties configured for profile cards for the organization.</span></span>|
|<span data-ttu-id="89794-137">itemInsights</span><span class="sxs-lookup"><span data-stu-id="89794-137">itemInsights</span></span>|[<span data-ttu-id="89794-138">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="89794-138">itemInsightsSettings</span></span>](iteminsightssettings.md)| <span data-ttu-id="89794-139">包含管理员为在用户与 Microsoft 365 中其他项目（如文档或网站）之间可见性 Microsoft Graph 派生的见解而配置的属性。</span><span class="sxs-lookup"><span data-stu-id="89794-139">Contains the properties that are configured by an administrator for the visibility of Microsoft Graph-derived insights, between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="89794-140">[通过此导航属性获取 itemInsightsSettings。](../api/iteminsightssettings-get.md)</span><span class="sxs-lookup"><span data-stu-id="89794-140">[Get itemInsightsSettings](../api/iteminsightssettings-get.md) through this navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="89794-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89794-141">JSON representation</span></span>

<span data-ttu-id="89794-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89794-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "keyProperty": "id"
}-->

```json
{
  "id": "String (identifier)",
  "profileCardProperties": [{"@odata.type": "microsoft.graph.profileCardProperty"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "organizationSettings resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


