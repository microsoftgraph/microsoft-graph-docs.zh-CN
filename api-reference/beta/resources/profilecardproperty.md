---
title: profileCardProperty 资源类型
description: 用于指定要以共享、人员体验显示的新属性或将应用自定义显示名称或批注的属性。 管理员可以定义一个默认显示名称字符串和一组替代翻译，供他们在组织中支持的语言使用。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: resourcePageType
ms.openlocfilehash: 33d2b1111580ba2302848ab1dbce3f773055a0b4
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50153562"
---
# <a name="profilecardproperty-resource-type"></a><span data-ttu-id="82153-104">profileCardProperty 资源类型</span><span class="sxs-lookup"><span data-stu-id="82153-104">profileCardProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="82153-105">表示组织在 Microsoft 365 个人资料卡上显示共享人员体验的用户属性。</span><span class="sxs-lookup"><span data-stu-id="82153-105">Represents an attribute of a user on the Microsoft 365 profile card for an organization to surface in a shared, people experience.</span></span>

<span data-ttu-id="82153-106">该属性可以是 Azure Active Directory (Azure AD) 内置属性（如 `Alias` or）或自定义 `UserPrincipalName` 属性。</span><span class="sxs-lookup"><span data-stu-id="82153-106">The attribute can be an Azure Active Directory (Azure AD) built-in attribute, such as `Alias` or `UserPrincipalName`, or it can be a custom attribute.</span></span> <span data-ttu-id="82153-107">对于自定义属性，管理员可以定义一个默认显示名称字符串和一组替代翻译，用于他们在组织中支持 `en-us` 的语言。</span><span class="sxs-lookup"><span data-stu-id="82153-107">For a custom attribute, an administrator can define an `en-us` default display name string and a set of alternative translations for the languages that they support in their organization.</span></span>

<span data-ttu-id="82153-108">有关向组织的配置文件卡添加属性详细信息，请参阅 [自定义配置文件卡片](/graph/add-properties-profilecard)。</span><span class="sxs-lookup"><span data-stu-id="82153-108">For more information on adding properties to the profile card for an organization, see [customize the profile card](/graph/add-properties-profilecard).</span></span>

## <a name="methods"></a><span data-ttu-id="82153-109">方法</span><span class="sxs-lookup"><span data-stu-id="82153-109">Methods</span></span>

| <span data-ttu-id="82153-110">方法</span><span class="sxs-lookup"><span data-stu-id="82153-110">Method</span></span>       | <span data-ttu-id="82153-111">返回类型</span><span class="sxs-lookup"><span data-stu-id="82153-111">Return Type</span></span> | <span data-ttu-id="82153-112">Description</span><span class="sxs-lookup"><span data-stu-id="82153-112">Description</span></span> |
|:-------------------------------------------------------------|:----------------------------------------------|:-----------------------------------------------------------------|
| [<span data-ttu-id="82153-113">List</span><span class="sxs-lookup"><span data-stu-id="82153-113">List</span></span>](../api/organizationsettings-list-profilecardproperties.md) | [<span data-ttu-id="82153-114">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="82153-114">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="82153-115">获取组织的 **profileCardProperty** 资源的集合。</span><span class="sxs-lookup"><span data-stu-id="82153-115">Get a collection of **profileCardProperty** resources of an organization.</span></span> |
| [<span data-ttu-id="82153-116">创建</span><span class="sxs-lookup"><span data-stu-id="82153-116">Create</span></span>](../api/organizationsettings-post-profilecardproperties.md) | [<span data-ttu-id="82153-117">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="82153-117">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="82153-118">为组织 **创建新的 profileCardProperty** 资源。</span><span class="sxs-lookup"><span data-stu-id="82153-118">Create a new **profileCardProperty** resource for an organization.</span></span> |
| [<span data-ttu-id="82153-119">Get</span><span class="sxs-lookup"><span data-stu-id="82153-119">Get</span></span>](../api/profilecardproperty-get.md) | [<span data-ttu-id="82153-120">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="82153-120">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="82153-121">读取 **profileCardProperty** 资源的属性和关系，其中包含给定字段的 Microsoft 365 组织中存在的配置文件卡自定义项。</span><span class="sxs-lookup"><span data-stu-id="82153-121">Read the properties and relationships of a **profileCardProperty** resource, which contains the profile card customizations that exist in a Microsoft 365 organization for a given field.</span></span> |
| [<span data-ttu-id="82153-122">更新</span><span class="sxs-lookup"><span data-stu-id="82153-122">Update</span></span>](../api/profilecardproperty-update.md)               | [<span data-ttu-id="82153-123">profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="82153-123">profileCardProperty</span></span>](profilecardproperty.md) | <span data-ttu-id="82153-124">更新 **profileCardProperty** 对象。</span><span class="sxs-lookup"><span data-stu-id="82153-124">Update a **profileCardProperty** object.</span></span>                               |
| [<span data-ttu-id="82153-125">删除</span><span class="sxs-lookup"><span data-stu-id="82153-125">Delete</span></span>](../api/profilecardproperty-delete.md)               | <span data-ttu-id="82153-126">无</span><span class="sxs-lookup"><span data-stu-id="82153-126">None</span></span>                                          | <span data-ttu-id="82153-127">删除 **profileCardProperty** 对象。</span><span class="sxs-lookup"><span data-stu-id="82153-127">Delete a **profileCardProperty** object.</span></span>                               |

## <a name="properties"></a><span data-ttu-id="82153-128">属性</span><span class="sxs-lookup"><span data-stu-id="82153-128">Properties</span></span>

| <span data-ttu-id="82153-129">属性</span><span class="sxs-lookup"><span data-stu-id="82153-129">Property</span></span>             | <span data-ttu-id="82153-130">类型</span><span class="sxs-lookup"><span data-stu-id="82153-130">Type</span></span>                                                        | <span data-ttu-id="82153-131">说明</span><span class="sxs-lookup"><span data-stu-id="82153-131">Description</span></span> |
|:---------------------|:------------------------------------------------------------|:------------|
|<span data-ttu-id="82153-132">批注</span><span class="sxs-lookup"><span data-stu-id="82153-132">annotations</span></span>           |<span data-ttu-id="82153-133">[profileCardAnnotation](profilecardannotation.md) 集合</span><span class="sxs-lookup"><span data-stu-id="82153-133">[profileCardAnnotation](profilecardannotation.md) collection</span></span> | <span data-ttu-id="82153-134">允许管理员为目录属性设置自定义显示标签，并针对租户中的用户进行本地化。</span><span class="sxs-lookup"><span data-stu-id="82153-134">Allows an administrator to set a custom display label for the directory property and localize it for the users in their tenant.</span></span>|
|<span data-ttu-id="82153-135">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="82153-135">directoryPropertyName</span></span> |<span data-ttu-id="82153-136">String</span><span class="sxs-lookup"><span data-stu-id="82153-136">String</span></span>                                                       | <span data-ttu-id="82153-137">标识 **获取、更新或删除操作中的 profileCardProperty** [资源。](../api/profilecardproperty-delete.md) [](../api/profilecardproperty-get.md) [](../api/profilecardproperty-update.md)</span><span class="sxs-lookup"><span data-stu-id="82153-137">Identifies a **profileCardProperty** resource in [Get](../api/profilecardproperty-get.md), [Update](../api/profilecardproperty-update.md), or [Delete](../api/profilecardproperty-delete.md) operations.</span></span> <span data-ttu-id="82153-138">允许管理员在其租户内的 Microsoft 365 (Azure AD) 显示隐藏的 Azure Active Directory 属性。</span><span class="sxs-lookup"><span data-stu-id="82153-138">Allows an administrator to surface hidden Azure Active Directory (Azure AD) properties on the Microsoft 365 profile card within their tenant.</span></span> <span data-ttu-id="82153-139">存在此状态时，此字段中引用的 Azure AD 字段将在个人资料卡片的联系人窗格上对租户中的所有用户可见。</span><span class="sxs-lookup"><span data-stu-id="82153-139">When present, the Azure AD field referenced in this field will be visible to all users in your tenant on the contact pane of the profile card.</span></span> <span data-ttu-id="82153-140">此字段允许的值是： `UserPrincipalName` ， `Fax` ， ， ， `StreetAddress` `PostalCode` `StateOrProvince` `Alias` `CustomAttribute1`  `CustomAttribute2` `CustomAttribute3` `CustomAttribute4` `CustomAttribute5` `CustomAttribute6` `CustomAttribute7` `CustomAttribute8` `CustomAttribute9` `CustomAttribute10` `CustomAttribute11` `CustomAttribute12` `CustomAttribute13` `CustomAttribute14` `CustomAttribute15` 。</span><span class="sxs-lookup"><span data-stu-id="82153-140">Allowed values for this field are: `UserPrincipalName`, `Fax`, `StreetAddress`, `PostalCode`, `StateOrProvince`, `Alias`, `CustomAttribute1`,  `CustomAttribute2`, `CustomAttribute3`, `CustomAttribute4`, `CustomAttribute5`, `CustomAttribute6`, `CustomAttribute7`, `CustomAttribute8`, `CustomAttribute9`, `CustomAttribute10`, `CustomAttribute11`, `CustomAttribute12`, `CustomAttribute13`, `CustomAttribute14`, `CustomAttribute15`.</span></span> |

## <a name="relationships"></a><span data-ttu-id="82153-141">关系</span><span class="sxs-lookup"><span data-stu-id="82153-141">Relationships</span></span>

<span data-ttu-id="82153-142">无。</span><span class="sxs-lookup"><span data-stu-id="82153-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="82153-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="82153-143">JSON representation</span></span>

<span data-ttu-id="82153-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82153-144">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.profileCardProperty"
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

