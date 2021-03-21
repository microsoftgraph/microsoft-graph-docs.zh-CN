---
title: identityUserFlowAttribute 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的用户流属性。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: 8262d8c77d31abbd25aaaae26018c651f0dcfbe5
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50957007"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="aa6f1-103">identityUserFlowAttribute 资源类型</span><span class="sxs-lookup"><span data-stu-id="aa6f1-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="aa6f1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aa6f1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aa6f1-105">代表 Azure Active Directory（Azure AD）租户和 Azure AD B2C 租户中的用户流属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant and an Azure AD B2C tenant.</span></span>

<span data-ttu-id="aa6f1-106">在 Azure AD 或 Azure AD B2C 租户中配置用户流属性，可在注册期间收集用户的相关信息。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-106">Configuring user flow attributes in your Azure AD or Azure AD B2C tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="aa6f1-107">可选择收集内置属性集；例如，指定名字、姓氏、市/县和邮政编码。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-107">You can choose to collect a built-in set of attribute; for example, Given Name, Surname, City, and Postal Code.</span></span> <span data-ttu-id="aa6f1-108">还可以配置自定义用户流属性，以便收集未内置到目录中的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-108">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="aa6f1-109">自定义用户流属性是对[Azure Active Directory 架构扩展](/azure/active-directory/develop/active-directory-schema-extensions)的抽象。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-109">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="aa6f1-110">Methods</span><span class="sxs-lookup"><span data-stu-id="aa6f1-110">Methods</span></span>

| <span data-ttu-id="aa6f1-111">方法</span><span class="sxs-lookup"><span data-stu-id="aa6f1-111">Method</span></span>       | <span data-ttu-id="aa6f1-112">返回类型</span><span class="sxs-lookup"><span data-stu-id="aa6f1-112">Return Type</span></span>  |<span data-ttu-id="aa6f1-113">Description</span><span class="sxs-lookup"><span data-stu-id="aa6f1-113">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="aa6f1-114">List</span><span class="sxs-lookup"><span data-stu-id="aa6f1-114">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="aa6f1-115">identityUserFlowAttributes collection</span><span class="sxs-lookup"><span data-stu-id="aa6f1-115">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="aa6f1-116">检索所有内置和自定义的用户流属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-116">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="aa6f1-117">创建</span><span class="sxs-lookup"><span data-stu-id="aa6f1-117">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="aa6f1-118">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="aa6f1-118">identityUserFlowAttribute</span></span>|<span data-ttu-id="aa6f1-119">创建新的自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-119">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="aa6f1-120">获取</span><span class="sxs-lookup"><span data-stu-id="aa6f1-120">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="aa6f1-121">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="aa6f1-121">identityUserFlowAttribute</span></span>|<span data-ttu-id="aa6f1-122">检索用户流属性的属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-122">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="aa6f1-123">更新</span><span class="sxs-lookup"><span data-stu-id="aa6f1-123">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="aa6f1-124">无</span><span class="sxs-lookup"><span data-stu-id="aa6f1-124">None</span></span>|<span data-ttu-id="aa6f1-125">更新自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-125">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="aa6f1-126">删除</span><span class="sxs-lookup"><span data-stu-id="aa6f1-126">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="aa6f1-127">无</span><span class="sxs-lookup"><span data-stu-id="aa6f1-127">None</span></span>|<span data-ttu-id="aa6f1-128">删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-128">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="aa6f1-129">属性</span><span class="sxs-lookup"><span data-stu-id="aa6f1-129">Properties</span></span>

|<span data-ttu-id="aa6f1-130">属性</span><span class="sxs-lookup"><span data-stu-id="aa6f1-130">Property</span></span>|<span data-ttu-id="aa6f1-131">类型</span><span class="sxs-lookup"><span data-stu-id="aa6f1-131">Type</span></span>|<span data-ttu-id="aa6f1-132">说明</span><span class="sxs-lookup"><span data-stu-id="aa6f1-132">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aa6f1-133">id</span><span class="sxs-lookup"><span data-stu-id="aa6f1-133">id</span></span>|<span data-ttu-id="aa6f1-134">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-134">String</span></span>|<span data-ttu-id="aa6f1-135">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-135">The identifier of the user flow attribute.</span></span> <span data-ttu-id="aa6f1-136">这是一个自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-136">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="aa6f1-137">displayName</span><span class="sxs-lookup"><span data-stu-id="aa6f1-137">displayName</span></span>|<span data-ttu-id="aa6f1-138">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-138">String</span></span>|<span data-ttu-id="aa6f1-139">用户流属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-139">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="aa6f1-140">说明</span><span class="sxs-lookup"><span data-stu-id="aa6f1-140">description</span></span>|<span data-ttu-id="aa6f1-141">String</span><span class="sxs-lookup"><span data-stu-id="aa6f1-141">String</span></span>|<span data-ttu-id="aa6f1-142">注册时显示给用户的用户流量属性的描述。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-142">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="aa6f1-143">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="aa6f1-143">userFlowAttributeType</span></span>|<span data-ttu-id="aa6f1-144">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="aa6f1-144">identityUserFlowAttributeType</span></span>|<span data-ttu-id="aa6f1-145">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-145">The type of the user flow attribute.</span></span> <span data-ttu-id="aa6f1-146">这是一个自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-146">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="aa6f1-147">根据属性的类型，此属性的值将为 `builtIn`、 `custom`或 `required`。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-147">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="aa6f1-148">DataType</span><span class="sxs-lookup"><span data-stu-id="aa6f1-148">dataType</span></span>|<span data-ttu-id="aa6f1-149">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="aa6f1-149">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="aa6f1-150">用户流属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-150">The data type of the user flow attribute.</span></span> <span data-ttu-id="aa6f1-151">在创建自定义用户流属性后，不能对此进行修改。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-151">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="aa6f1-152">数据类型 **支持** 为： `string` 、 `boolean` 、 `int64` 、 `stringCollection` 、 `dateTime`。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-152">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aa6f1-153">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aa6f1-153">JSON representation</span></span>

<span data-ttu-id="aa6f1-154">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aa6f1-154">The following is a JSON representation of the resource.</span></span>

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
