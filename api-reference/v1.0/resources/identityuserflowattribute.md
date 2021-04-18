---
title: identityUserFlowAttribute 资源类型
description: 代表 Azure Active Directory 租户和 Azure AD B2C 租户中的用户流属性。
localization_priority: Priority
doc_type: resourcePageType
ms.prod: identity-and-sign-in
author: jkdouglas
ms.openlocfilehash: af3ec2a762fc0252da929d863917ba6cd274ba95
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882914"
---
# <a name="identityuserflowattribute-resource-type"></a><span data-ttu-id="39d55-103">identityUserFlowAttribute 资源类型</span><span class="sxs-lookup"><span data-stu-id="39d55-103">identityUserFlowAttribute resource type</span></span>

<span data-ttu-id="39d55-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="39d55-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="39d55-105">表示 Azure Active Directory （Azure AD） 租户中的用户流属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-105">Represents user flow attributes in an Azure Active Directory (Azure AD) tenant.</span></span>

<span data-ttu-id="39d55-106">在 Azure AD 租户中配置用户流属性可让你在注册期间收集用户相关信息。</span><span class="sxs-lookup"><span data-stu-id="39d55-106">Configuring user flow attributes in your Azure AD tenant allows you to collect information about a user during sign-up.</span></span> <span data-ttu-id="39d55-107">可以选择收集一组内置属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-107">You can choose to collect a built-in set of attributes.</span></span> <span data-ttu-id="39d55-108">例如，给定姓名、省/市/县和邮政编码。</span><span class="sxs-lookup"><span data-stu-id="39d55-108">For example, given name, surname, city, and postal code.</span></span> <span data-ttu-id="39d55-109">还可以配置自定义用户流属性，以便收集未内置到目录中的用户的信息。</span><span class="sxs-lookup"><span data-stu-id="39d55-109">You can also configure custom user flow attributes to collect information from a user that is not built in to the directory.</span></span> <span data-ttu-id="39d55-110">自定义用户流属性是对[Azure Active Directory 架构扩展](/azure/active-directory/develop/active-directory-schema-extensions)的抽象。</span><span class="sxs-lookup"><span data-stu-id="39d55-110">Custom user flow attributes are an abstraction over [Azure Active Directory schema extensions](/azure/active-directory/develop/active-directory-schema-extensions).</span></span>

## <a name="methods"></a><span data-ttu-id="39d55-111">Methods</span><span class="sxs-lookup"><span data-stu-id="39d55-111">Methods</span></span>

| <span data-ttu-id="39d55-112">方法</span><span class="sxs-lookup"><span data-stu-id="39d55-112">Method</span></span>       | <span data-ttu-id="39d55-113">返回类型</span><span class="sxs-lookup"><span data-stu-id="39d55-113">Return Type</span></span>  |<span data-ttu-id="39d55-114">Description</span><span class="sxs-lookup"><span data-stu-id="39d55-114">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="39d55-115">List</span><span class="sxs-lookup"><span data-stu-id="39d55-115">List</span></span>](../api/identityuserflowattribute-list.md)|<span data-ttu-id="39d55-116">identityUserFlowAttributes collection</span><span class="sxs-lookup"><span data-stu-id="39d55-116">identityUserFlowAttributes collection</span></span>|<span data-ttu-id="39d55-117">检索所有内置和自定义的用户流属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-117">Retrieve all built-in and custom user flow attributes.</span></span>|
|[<span data-ttu-id="39d55-118">创建</span><span class="sxs-lookup"><span data-stu-id="39d55-118">Create</span></span>](../api/identityuserflowattribute-post.md)|<span data-ttu-id="39d55-119">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="39d55-119">identityUserFlowAttribute</span></span>|<span data-ttu-id="39d55-120">创建新的自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-120">Create a new custom user flow attribute.</span></span>|
|[<span data-ttu-id="39d55-121">获取</span><span class="sxs-lookup"><span data-stu-id="39d55-121">Get</span></span>](../api/identityuserflowattribute-get.md) |<span data-ttu-id="39d55-122">identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="39d55-122">identityUserFlowAttribute</span></span>|<span data-ttu-id="39d55-123">检索用户流属性的属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-123">Retrieve properties of a user flow attribute.</span></span>|
|[<span data-ttu-id="39d55-124">更新</span><span class="sxs-lookup"><span data-stu-id="39d55-124">Update</span></span>](../api/identityuserflowattribute-update.md)|<span data-ttu-id="39d55-125">无</span><span class="sxs-lookup"><span data-stu-id="39d55-125">None</span></span>|<span data-ttu-id="39d55-126">更新自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-126">Update a custom user flow attribute.</span></span>|
|[<span data-ttu-id="39d55-127">删除</span><span class="sxs-lookup"><span data-stu-id="39d55-127">Delete</span></span>](../api/identityuserflowattribute-delete.md)|<span data-ttu-id="39d55-128">无</span><span class="sxs-lookup"><span data-stu-id="39d55-128">None</span></span>|<span data-ttu-id="39d55-129">删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-129">Delete a custom user flow attribute.</span></span>|

## <a name="properties"></a><span data-ttu-id="39d55-130">属性</span><span class="sxs-lookup"><span data-stu-id="39d55-130">Properties</span></span>

|<span data-ttu-id="39d55-131">属性</span><span class="sxs-lookup"><span data-stu-id="39d55-131">Property</span></span>|<span data-ttu-id="39d55-132">类型</span><span class="sxs-lookup"><span data-stu-id="39d55-132">Type</span></span>|<span data-ttu-id="39d55-133">说明</span><span class="sxs-lookup"><span data-stu-id="39d55-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="39d55-134">id</span><span class="sxs-lookup"><span data-stu-id="39d55-134">id</span></span>|<span data-ttu-id="39d55-135">String</span><span class="sxs-lookup"><span data-stu-id="39d55-135">String</span></span>|<span data-ttu-id="39d55-136">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="39d55-136">The identifier of the user flow attribute.</span></span> <span data-ttu-id="39d55-137">这是一个自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-137">This is a read-only attribute that is automatically created.</span></span>|
|<span data-ttu-id="39d55-138">displayName</span><span class="sxs-lookup"><span data-stu-id="39d55-138">displayName</span></span>|<span data-ttu-id="39d55-139">String</span><span class="sxs-lookup"><span data-stu-id="39d55-139">String</span></span>|<span data-ttu-id="39d55-140">用户流属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="39d55-140">The display name of the user flow attribute.</span></span>|
|<span data-ttu-id="39d55-141">说明</span><span class="sxs-lookup"><span data-stu-id="39d55-141">description</span></span>|<span data-ttu-id="39d55-142">String</span><span class="sxs-lookup"><span data-stu-id="39d55-142">String</span></span>|<span data-ttu-id="39d55-143">注册时显示给用户的用户流量属性的描述。</span><span class="sxs-lookup"><span data-stu-id="39d55-143">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span>|
|<span data-ttu-id="39d55-144">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="39d55-144">userFlowAttributeType</span></span>|<span data-ttu-id="39d55-145">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="39d55-145">identityUserFlowAttributeType</span></span>|<span data-ttu-id="39d55-146">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="39d55-146">The type of the user flow attribute.</span></span> <span data-ttu-id="39d55-147">这是一个自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="39d55-147">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="39d55-148">根据属性的类型，此属性的值将为 `builtIn`、 `custom`或 `required`。</span><span class="sxs-lookup"><span data-stu-id="39d55-148">Depending on the type of attribute, the values for this property will be `builtIn`, `custom`, or `required`.</span></span>|
|<span data-ttu-id="39d55-149">DataType</span><span class="sxs-lookup"><span data-stu-id="39d55-149">dataType</span></span>|<span data-ttu-id="39d55-150">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="39d55-150">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="39d55-151">用户流属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="39d55-151">The data type of the user flow attribute.</span></span> <span data-ttu-id="39d55-152">在创建自定义用户流属性后，不能对此进行修改。</span><span class="sxs-lookup"><span data-stu-id="39d55-152">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="39d55-153">数据类型 **支持** 为： `string` 、 `boolean` 、 `int64` 、 `stringCollection` 、 `dateTime`。</span><span class="sxs-lookup"><span data-stu-id="39d55-153">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="39d55-154">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39d55-154">JSON representation</span></span>

<span data-ttu-id="39d55-155">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39d55-155">The following is a JSON representation of the resource.</span></span>

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
