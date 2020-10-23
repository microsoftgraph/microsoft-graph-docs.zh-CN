---
title: identityUserFlowAttribute 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的用户流属性。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: jkdouglas
ms.openlocfilehash: f5166cafff64a7050b89bbd7f70cba66f429646d
ms.sourcegitcommit: 17cd789abbab2bf674ce4e39b3fcdc1bbebc83ce
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/23/2020
ms.locfileid: "48742369"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="49f5f-103">identityUserFlowAttribute 资源类型</span><span class="sxs-lookup"><span data-stu-id="49f5f-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="49f5f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="49f5f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49f5f-105">代表 Azure Active Directory（Azure AD）租户和 Azure AD B2C 租户中的用户流属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="49f5f-106">在 Azure AD 或 Azure AD B2C 租户中配置用户流属性，可在注册期间收集用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="49f5f-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="49f5f-107">可选择收集内置属性集；例如，指定名字、姓氏、市/县和邮政编码。</span><span class="sxs-lookup"><span data-stu-id="49f5f-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="49f5f-108">还可以配置自定义用户流属性，以便收集未内置到目录中的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="49f5f-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="49f5f-109">自定义用户流属性是对[Azure Active Directory 架构扩展](/azure/active-directory/develop/active-directory-schema-extensions)的抽象。</span><span class="sxs-lookup"><span data-stu-id="49f5f-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="49f5f-110">方法</span><span class="sxs-lookup"><span data-stu-id="49f5f-110">Methods</span></span>

| <span data-ttu-id="49f5f-111">方法</span><span class="sxs-lookup"><span data-stu-id="49f5f-111">Method</span></span>       | <span data-ttu-id="49f5f-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="49f5f-112">Return Type</span></span>  |<span data-ttu-id="49f5f-113">Description</span><span class="sxs-lookup"><span data-stu-id="49f5f-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="49f5f-114">列表</span><span class="sxs-lookup"><span data-stu-id="49f5f-114">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="49f5f-115">identityUserFlowAttributes collection</span><span class="sxs-lookup"><span data-stu-id="49f5f-115">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="49f5f-116">检索所有内置和自定义的用户流属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-116">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="49f5f-117">创建</span><span class="sxs-lookup"><span data-stu-id="49f5f-117">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="49f5f-118">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="49f5f-118">identityUserFlowAttribute</span></span>|<span data-ttu-id="49f5f-119">创建新的自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-119">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="49f5f-120">获取</span><span class="sxs-lookup"><span data-stu-id="49f5f-120">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="49f5f-121">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="49f5f-121">identityUserFlowAttribute</span></span>|<span data-ttu-id="49f5f-122">检索用户流属性的属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-122">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="49f5f-123">更新</span><span class="sxs-lookup"><span data-stu-id="49f5f-123">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="49f5f-124">无</span><span class="sxs-lookup"><span data-stu-id="49f5f-124">None</span></span>|<span data-ttu-id="49f5f-125">更新自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-125">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="49f5f-126">删除</span><span class="sxs-lookup"><span data-stu-id="49f5f-126">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="49f5f-127">无</span><span class="sxs-lookup"><span data-stu-id="49f5f-127">None</span></span>|<span data-ttu-id="49f5f-128">删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-128">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="49f5f-129">属性</span><span class="sxs-lookup"><span data-stu-id="49f5f-129">Properties</span></span>

|<span data-ttu-id="49f5f-130">属性</span><span class="sxs-lookup"><span data-stu-id="49f5f-130">Property</span></span>|<span data-ttu-id="49f5f-131">类型</span><span class="sxs-lookup"><span data-stu-id="49f5f-131">Type</span></span>|<span data-ttu-id="49f5f-132">说明</span><span class="sxs-lookup"><span data-stu-id="49f5f-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49f5f-133">id</span><span class="sxs-lookup"><span data-stu-id="49f5f-133">id</span></span>|<span data-ttu-id="49f5f-134">String</span><span class="sxs-lookup"><span data-stu-id="49f5f-134">String</span></span>|<span data-ttu-id="49f5f-135">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="49f5f-135">The identifier of the user flow attribute.</span></span> <span data-ttu-id="49f5f-136">这是一个自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-136">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="49f5f-137">displayName</span><span class="sxs-lookup"><span data-stu-id="49f5f-137">displayName</span></span>|<span data-ttu-id="49f5f-138">String</span><span class="sxs-lookup"><span data-stu-id="49f5f-138">String</span></span>|<span data-ttu-id="49f5f-139">用户流属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="49f5f-139">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="49f5f-140">description</span><span class="sxs-lookup"><span data-stu-id="49f5f-140">description</span></span>|<span data-ttu-id="49f5f-141">String</span><span class="sxs-lookup"><span data-stu-id="49f5f-141">String</span></span>|<span data-ttu-id="49f5f-142">注册时显示给用户的用户流量属性的描述。</span><span class="sxs-lookup"><span data-stu-id="49f5f-142">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="49f5f-143">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="49f5f-143">userFlowAttributeType</span></span>|<span data-ttu-id="49f5f-144">String</span><span class="sxs-lookup"><span data-stu-id="49f5f-144">String</span></span>|<span data-ttu-id="49f5f-145">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="49f5f-145">The type of the user flow attribute.</span></span> <span data-ttu-id="49f5f-146">这是一个自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="49f5f-146">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="49f5f-147">此属性的值将是 `builtIn` 或 `custom`，具体取决于属性的类型。</span><span class="sxs-lookup"><span data-stu-id="49f5f-147">Depending on the type of attribute, the values for this property will be `builtIn` or `custom`.</span></span>|
|<span data-ttu-id="49f5f-148">DataType</span><span class="sxs-lookup"><span data-stu-id="49f5f-148">dataType</span></span>|<span data-ttu-id="49f5f-149">String</span><span class="sxs-lookup"><span data-stu-id="49f5f-149">String</span></span>|<span data-ttu-id="49f5f-150">用户流属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="49f5f-150">The data type of the user flow attribute.</span></span> <span data-ttu-id="49f5f-151">在创建自定义用户流属性后，不能对此进行修改。</span><span class="sxs-lookup"><span data-stu-id="49f5f-151">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="49f5f-152">**dataType** 支持的值有：</span><span class="sxs-lookup"><span data-stu-id="49f5f-152">The supported values for **dataType** are:</span></span><br/><ul><li><span data-ttu-id="49f5f-153">`string` - 表示 identityUserFlowAttribute 的数据类型为字符串。</span><span class="sxs-lookup"><span data-stu-id="49f5f-153">`string` - denotes that the dataType for the identityUserFlowAttribute is a string.</span></span> </li><li><span data-ttu-id="49f5f-154">`boolean` - 表示 identityUserFlowAttribute 的数据类型为Boolean。</span><span class="sxs-lookup"><span data-stu-id="49f5f-154">`boolean` - denotes that the dataType for the identityUserFlowAttribute is a Boolean.</span></span></li><li><span data-ttu-id="49f5f-155">`int64` - 表示 identityUserFlowAttribute 的数据类型为整数。</span><span class="sxs-lookup"><span data-stu-id="49f5f-155">`int64` - denotes that the dataType for the identityUserFlowAttribute is an integer.</span></span></li></ul>|

## <a name="json-representation"></a><span data-ttu-id="49f5f-156">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49f5f-156">JSON representation</span></span>

<span data-ttu-id="49f5f-157">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49f5f-157">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```json
{
    "@odata.type": "#microsoft.graph.identityUserFlowAttribute",
    "id": "String (identifier)",
    "displayName": "String",
    "description": "String",
    "userFlowAttributeType": "String",
    "dataType": "String"
}
```
