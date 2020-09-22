---
title: profileCardProperty 资源类型
description: 用于将新的属性指定为在共享、人员体验或应用了自定义的显示名称或批注的情况下进行呈现。 管理员可以为其组织中支持的语言定义默认的显示名称字符串和一组替代转换。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 0dc09ae31f2b0189f0b3f3e0be83a72ea76e2448
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48029090"
---
# <a name="profilecardproperty-resource-type"></a><span data-ttu-id="f7aea-104">profileCardProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7aea-104">profileCardProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7aea-105">表示适用于组织的 Microsoft 365 配置文件卡片上的用户的属性，用于在共享、人员体验中进行呈现。</span><span class="sxs-lookup"><span data-stu-id="f7aea-105">Represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

<span data-ttu-id="f7aea-106">该属性可以是 azure AD) 的 Azure Active Directory (的内置属性（例如 `Alias` 或）， `UserPrincipalName` 也可以是自定义属性。</span><span class="sxs-lookup"><span data-stu-id="f7aea-106">The attribute can be an Azure Active Directory (Azure AD) built-in attribute, such as `Alias` or `UserPrincipalName`, or it can be a custom attribute.</span></span> <span data-ttu-id="f7aea-107">对于自定义属性，管理员可以为 `en-us` 其组织中支持的语言定义默认的显示名称字符串和一组替代转换。</span><span class="sxs-lookup"><span data-stu-id="f7aea-107">For a custom attribute, an administrator can define an `en-us` default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

<span data-ttu-id="f7aea-108">有关向组织的配置文件卡片添加属性的详细信息，请参阅 [自定义配置文件卡片](/graph/add-properties-profilecard)。</span><span class="sxs-lookup"><span data-stu-id="f7aea-108">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="methods"></a><span data-ttu-id="f7aea-109">方法</span><span class="sxs-lookup"><span data-stu-id="f7aea-109">Methods</span></span>

| <span data-ttu-id="f7aea-110">方法</span><span class="sxs-lookup"><span data-stu-id="f7aea-110">Method</span></span>       | <span data-ttu-id="f7aea-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="f7aea-111">Return Type</span></span> | <span data-ttu-id="f7aea-112">Description</span><span class="sxs-lookup"><span data-stu-id="f7aea-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="f7aea-113">List</span><span class="sxs-lookup"><span data-stu-id="f7aea-113">List</span></span>](../api/organizationsettings-list-profilecardproperties.md) | [<span data-ttu-id="f7aea-114">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f7aea-114">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="f7aea-115">获取组织的 **profileCardProperty** 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="f7aea-115">Get a collection of **profileCardProperty** resources of an organization.</span></span> |
| [<span data-ttu-id="f7aea-116">创建</span><span class="sxs-lookup"><span data-stu-id="f7aea-116">Create</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="f7aea-117">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f7aea-117">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="f7aea-118">为组织创建新的 **profileCardProperty** 资源。</span><span class="sxs-lookup"><span data-stu-id="f7aea-118">Create a new **profileCardProperty** resource for an organization.</span></span> |
| [<span data-ttu-id="f7aea-119">获取</span><span class="sxs-lookup"><span data-stu-id="f7aea-119">Get</span></span>](../api/profilecardproperty-get.md) | [<span data-ttu-id="f7aea-120">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f7aea-120">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="f7aea-121">阅读 **profileCardProperty** 资源的属性和关系，其中包含在给定字段的 Microsoft 365 组织中存在的配置文件卡片自定义项。</span><span class="sxs-lookup"><span data-stu-id="f7aea-121">Read the properties and relationships of a **profileCardProperty** resource, which contains the profile card customizations that exist in a Microsoft 365 organization for a given field.</span></span> |
| [<span data-ttu-id="f7aea-122">更新</span><span class="sxs-lookup"><span data-stu-id="f7aea-122">Update</span></span>](../api/profilecardproperty-update.md)               | [<span data-ttu-id="f7aea-123">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="f7aea-123">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="f7aea-124">更新 **profileCardProperty** 对象。</span><span class="sxs-lookup"><span data-stu-id="f7aea-124">Update a **profileCardProperty** object.</span></span>                               |
| [<span data-ttu-id="f7aea-125">删除</span><span class="sxs-lookup"><span data-stu-id="f7aea-125">Delete</span></span>](../api/profilecardproperty-delete.md)               | <span data-ttu-id="f7aea-126">无</span><span class="sxs-lookup"><span data-stu-id="f7aea-126">None</span></span>                                          | <span data-ttu-id="f7aea-127">删除 **profileCardProperty** 对象。</span><span class="sxs-lookup"><span data-stu-id="f7aea-127">Delete a **profileCardProperty** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="f7aea-128">属性</span><span class="sxs-lookup"><span data-stu-id="f7aea-128">Properties</span></span>

| <span data-ttu-id="f7aea-129">属性</span><span class="sxs-lookup"><span data-stu-id="f7aea-129">Property</span></span>             | <span data-ttu-id="f7aea-130">类型</span><span class="sxs-lookup"><span data-stu-id="f7aea-130">Type</span></span>                                                        | <span data-ttu-id="f7aea-131">说明</span><span class="sxs-lookup"><span data-stu-id="f7aea-131">Description</span></span> |
|:---------------------|:------------------------------------------------------------|:------------|
|<span data-ttu-id="f7aea-132">批注</span><span class="sxs-lookup"><span data-stu-id="f7aea-132">annotations</span></span>           |<span data-ttu-id="f7aea-133">[profileCardAnnotation](profilecardannotation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7aea-133">[profileCardAnnotation](profilecardannotation.md) collection</span></span> | <span data-ttu-id="f7aea-134">允许管理员为目录属性设置自定义显示标签，并针对其租户中的用户对其进行本地化。</span><span class="sxs-lookup"><span data-stu-id="f7aea-134">Allows an administrator to set a custom display label for the directory property and localize it for the users in their tenant.</span></span>|
|<span data-ttu-id="f7aea-135">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="f7aea-135">directoryPropertyName</span></span> |<span data-ttu-id="f7aea-136">String</span><span class="sxs-lookup"><span data-stu-id="f7aea-136">String</span></span>                                                       | <span data-ttu-id="f7aea-137">标识[获取](../api/profilecardproperty-get.md)、[更新](../api/profilecardproperty-update.md)或[删除](../api/profilecardproperty-delete.md)操作中的**profileCardProperty**资源。</span><span class="sxs-lookup"><span data-stu-id="f7aea-137">Identifies a **profileCardProperty** resource in [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md), or [Delete](../api/profilecardproperty-delete.md) operations.</span></span> <span data-ttu-id="f7aea-138">允许管理员在其租户内的 Microsoft 365 配置文件卡上 (Azure AD) 属性呈现隐藏的 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="f7aea-138">Allows an administrator to surface hidden Azure Active Directory (Azure AD) properties on the Microsoft 365 profile card within their tenant.</span></span> <span data-ttu-id="f7aea-139">如果存在，则此字段中引用的 Azure AD 字段将在配置文件卡片的联系人窗格中对租户中的所有用户可见。</span><span class="sxs-lookup"><span data-stu-id="f7aea-139">When present, the Azure AD field referenced in this field will be visible to all users in your tenant on the contact pane of the profile card.</span></span> <span data-ttu-id="f7aea-140">此字段允许的值为：、、、、、、、、、、、、、、、、、、、、 `UserPrincipalName` `Fax` `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1`  `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` `CustomAttribute8` `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` 。</span><span class="sxs-lookup"><span data-stu-id="f7aea-140">Allowed values for this field are: `UserPrincipalName`, `Fax`, `StreetAddress`, `PostalCode`, `StateOrProvince`, `Alias`, `CustomAttribute1`,  `CustomAttribute2`, `CustomAttribute3`, `CustomAttribute4`, `CustomAttribute5`, `CustomAttribute6`, `CustomAttribute7`, `CustomAttribute8`, `CustomAttribute9`, `CustomAttribute10`, `CustomAttribute11`, `CustomAttribute12`, `CustomAttribute13`, `CustomAttribute14`, `CustomAttribute15`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="f7aea-141">关系</span><span class="sxs-lookup"><span data-stu-id="f7aea-141">Relationships</span></span>

<span data-ttu-id="f7aea-142">无。</span><span class="sxs-lookup"><span data-stu-id="f7aea-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f7aea-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7aea-143">JSON representation</span></span>

<span data-ttu-id="f7aea-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7aea-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty",
  "baseType": ""
}-->

```json
{
  "annotations": [
    {
      "displayName": "String",
      "localizations": [
        {
          "languageTag": "String",
          "displayName": "String"
        }
      ]
    }
  ],
  "directoryPropertyName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "profileCardProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

