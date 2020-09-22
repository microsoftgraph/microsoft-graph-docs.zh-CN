---
title: organizationSettings 资源类型
description: 包含适用于组织或其内的用户对象的设置。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: e95bae902b444735b87fa7b29e061bf9bf2629ba
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998472"
---
# <a name="organizationsettings-resource-type"></a><span data-ttu-id="361d2-103">organizationSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="361d2-103">organizationSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="361d2-104">包含适用于 [组织](organization.md) 或应应用于组织中的 [用户](user.md) 对象的设置。</span><span class="sxs-lookup"><span data-stu-id="361d2-104">Contains settings that are applicable to the [organization](organization.md) or that should be applied to [user](user.md) objects within an organization.</span></span>

## <a name="methods"></a><span data-ttu-id="361d2-105">方法</span><span class="sxs-lookup"><span data-stu-id="361d2-105">Methods</span></span>

| <span data-ttu-id="361d2-106">方法</span><span class="sxs-lookup"><span data-stu-id="361d2-106">Method</span></span>       | <span data-ttu-id="361d2-107">返回类型</span><span class="sxs-lookup"><span data-stu-id="361d2-107">Return Type</span></span> | <span data-ttu-id="361d2-108">说明</span><span class="sxs-lookup"><span data-stu-id="361d2-108">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="361d2-109">获取组织设置</span><span class="sxs-lookup"><span data-stu-id="361d2-109">Get organization settings</span></span>](../api/organizationsettings-get.md) | [<span data-ttu-id="361d2-110">organizationSettings</span><span class="sxs-lookup"><span data-stu-id="361d2-110">organizationSettings</span></span>](organizationsettings.md) | <span data-ttu-id="361d2-111">读取组织设置对象。</span><span class="sxs-lookup"><span data-stu-id="361d2-111">Read the organization settings object.</span></span> |
| [<span data-ttu-id="361d2-112">创建 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="361d2-112">Create profileCardProperty</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="361d2-113">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="361d2-113">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="361d2-114">通过发布到**profileCardProperty**对象集合创建新的**profileCardProperty** 。</span><span class="sxs-lookup"><span data-stu-id="361d2-114">Create a new **profileCardProperty** by posting to the **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="361d2-115">列出 profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="361d2-115">List profileCardProperties</span></span>](../api/organizationsettings-list-profilecardproperties.md) | <span data-ttu-id="361d2-116">[profileCardProperty](profilecardproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="361d2-116">[profileCardProperty](profilecardproperty.md) collection</span></span> | <span data-ttu-id="361d2-117">获取 **profileCardProperty** 对象集合。</span><span class="sxs-lookup"><span data-stu-id="361d2-117">Get a **profileCardProperty** object collection.</span></span> |
| [<span data-ttu-id="361d2-118">获取 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="361d2-118">Get itemInsightsSettings</span></span>](../api/iteminsightssettings-get.md) | [<span data-ttu-id="361d2-119">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="361d2-119">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="361d2-120">获取 **itemInsightsSettings** 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="361d2-120">Get the properties of an **itemInsightsSettings** object.</span></span> |
| [<span data-ttu-id="361d2-121">更新 itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="361d2-121">Update itemInsightsSettings</span></span>](../api/iteminsightssettings-update.md) | [<span data-ttu-id="361d2-122">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="361d2-122">itemInsightsSettings</span></span>](iteminsightssettings.md) | <span data-ttu-id="361d2-123">更新指定的 **itemInsightsSettings** 资源的属性。</span><span class="sxs-lookup"><span data-stu-id="361d2-123">Update the properties of the specified **itemInsightsSettings** resource.</span></span> |

## <a name="properties"></a><span data-ttu-id="361d2-124">属性</span><span class="sxs-lookup"><span data-stu-id="361d2-124">Properties</span></span>

<span data-ttu-id="361d2-125">无。</span><span class="sxs-lookup"><span data-stu-id="361d2-125">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="361d2-126">关系</span><span class="sxs-lookup"><span data-stu-id="361d2-126">Relationships</span></span>

| <span data-ttu-id="361d2-127">关系</span><span class="sxs-lookup"><span data-stu-id="361d2-127">Relationship</span></span> | <span data-ttu-id="361d2-128">类型</span><span class="sxs-lookup"><span data-stu-id="361d2-128">Type</span></span>        | <span data-ttu-id="361d2-129">说明</span><span class="sxs-lookup"><span data-stu-id="361d2-129">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="361d2-130">id</span><span class="sxs-lookup"><span data-stu-id="361d2-130">id</span></span> |<span data-ttu-id="361d2-131">String</span><span class="sxs-lookup"><span data-stu-id="361d2-131">String</span></span>| <span data-ttu-id="361d2-132">组织的设置对象的 Id。</span><span class="sxs-lookup"><span data-stu-id="361d2-132">Id of the settings object for the organization.</span></span> |
|<span data-ttu-id="361d2-133">profileCardProperties</span><span class="sxs-lookup"><span data-stu-id="361d2-133">profileCardProperties</span></span>|<span data-ttu-id="361d2-134">[profileCardProperty](profilecardproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="361d2-134">[profileCardProperty](profilecardproperty.md) collection</span></span>| <span data-ttu-id="361d2-135">包含管理员已定义为在 Microsoft 365 配置文件卡上可见的属性的集合。</span><span class="sxs-lookup"><span data-stu-id="361d2-135">Contains a collection of the properties an administrator has defined as visible on the Microsoft 365 profile card.</span></span> <span data-ttu-id="361d2-136">[Get organization settings](../api/organizationsettings-get.md) 返回为组织配置文件卡片配置的属性。</span><span class="sxs-lookup"><span data-stu-id="361d2-136">[Get organization settings](../api/organizationsettings-get.md) returns the properties configured for profile cards for the organization.</span></span>|
|<span data-ttu-id="361d2-137">itemInsights</span><span class="sxs-lookup"><span data-stu-id="361d2-137">itemInsights</span></span>|[<span data-ttu-id="361d2-138">itemInsightsSettings</span><span class="sxs-lookup"><span data-stu-id="361d2-138">itemInsightsSettings</span></span>](iteminsightssettings.md)| <span data-ttu-id="361d2-139">包含由管理员为 microsoft Graph 派生的见解的可见性配置的属性，这些属性与 Microsoft 365 中的用户和其他项目（如文档或网站）之间的可见性。</span><span class="sxs-lookup"><span data-stu-id="361d2-139">Contains the properties that are configured by an administrator for the visibility of Microsoft Graph-derived insights, between a user and other items in Microsoft 365, such as documents or sites.</span></span> <span data-ttu-id="361d2-140">通过此导航属性[获取 itemInsightsSettings](../api/iteminsightssettings-get.md) 。</span><span class="sxs-lookup"><span data-stu-id="361d2-140">[Get itemInsightsSettings](../api/iteminsightssettings-get.md) through this navigation property.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="361d2-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="361d2-141">JSON representation</span></span>

<span data-ttu-id="361d2-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="361d2-142">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.organizationSettings",
  "baseType": "",
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


