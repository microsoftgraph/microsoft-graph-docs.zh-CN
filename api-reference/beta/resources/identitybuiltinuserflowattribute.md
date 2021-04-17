---
title: identityBuiltInUserFlowAttribute 资源类型
description: 表示 Azure Active Directory 租户中的内置用户流属性，可用于自助服务注册用户流。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: e3d6c9eef25f428734214854d28a342f9c4f59dd
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882659"
---
# <a name="identitybuiltinuserflowattribute-resource-type"></a><span data-ttu-id="be120-103">identityBuiltInUserFlowAttribute 资源类型</span><span class="sxs-lookup"><span data-stu-id="be120-103">identityBuiltInUserFlowAttribute resource type</span></span>

<span data-ttu-id="be120-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="be120-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="be120-105">表示 Azure Active Directory 租户中的内置用户流属性，可用于自助服务注册用户流。</span><span class="sxs-lookup"><span data-stu-id="be120-105">Represents a built-in user flow attribute in Azure Active Directory tenants that can be used in your self-service sign-up user flows.</span></span> <span data-ttu-id="be120-106">这些属性无法修改且为只读。</span><span class="sxs-lookup"><span data-stu-id="be120-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="be120-107">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="be120-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="be120-108">属性</span><span class="sxs-lookup"><span data-stu-id="be120-108">Properties</span></span>

|<span data-ttu-id="be120-109">属性</span><span class="sxs-lookup"><span data-stu-id="be120-109">Property</span></span>|<span data-ttu-id="be120-110">类型</span><span class="sxs-lookup"><span data-stu-id="be120-110">Type</span></span>|<span data-ttu-id="be120-111">说明</span><span class="sxs-lookup"><span data-stu-id="be120-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be120-112">id</span><span class="sxs-lookup"><span data-stu-id="be120-112">id</span></span>|<span data-ttu-id="be120-113">String</span><span class="sxs-lookup"><span data-stu-id="be120-113">String</span></span>|<span data-ttu-id="be120-114">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="be120-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="be120-115">这是一个自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="be120-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="be120-116">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="be120-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="be120-117">displayName</span><span class="sxs-lookup"><span data-stu-id="be120-117">displayName</span></span>|<span data-ttu-id="be120-118">String</span><span class="sxs-lookup"><span data-stu-id="be120-118">String</span></span>|<span data-ttu-id="be120-119">用户流属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="be120-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="be120-120">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="be120-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="be120-121">只读。</span><span class="sxs-lookup"><span data-stu-id="be120-121">Read-only.</span></span>|
|<span data-ttu-id="be120-122">说明</span><span class="sxs-lookup"><span data-stu-id="be120-122">description</span></span>|<span data-ttu-id="be120-123">String</span><span class="sxs-lookup"><span data-stu-id="be120-123">String</span></span>|<span data-ttu-id="be120-124">注册时显示给用户的用户流量属性的描述。</span><span class="sxs-lookup"><span data-stu-id="be120-124">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="be120-125">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="be120-125">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="be120-126">只读。</span><span class="sxs-lookup"><span data-stu-id="be120-126">Read-only.</span></span>|
|<span data-ttu-id="be120-127">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="be120-127">userFlowAttributeType</span></span>|<span data-ttu-id="be120-128">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="be120-128">identityUserFlowAttributeType</span></span>|<span data-ttu-id="be120-129">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="be120-129">The type of the user flow attribute.</span></span> <span data-ttu-id="be120-130">这是一个自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="be120-130">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="be120-131">此属性的值将为 `builtIn` 。</span><span class="sxs-lookup"><span data-stu-id="be120-131">The value for this property will be `builtIn`.</span></span> <span data-ttu-id="be120-132">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="be120-132">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="be120-133">只读。</span><span class="sxs-lookup"><span data-stu-id="be120-133">Read-only.</span></span>|
|<span data-ttu-id="be120-134">DataType</span><span class="sxs-lookup"><span data-stu-id="be120-134">dataType</span></span>|<span data-ttu-id="be120-135">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="be120-135">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="be120-136">用户流属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="be120-136">The data type of the user flow attribute.</span></span> <span data-ttu-id="be120-137">在创建自定义用户流属性后，不能对此进行修改。</span><span class="sxs-lookup"><span data-stu-id="be120-137">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="be120-138">数据类型 **支持** 为： `string` 、 `boolean` 、 `int64` 、 `stringCollection` 、 `dateTime`。</span><span class="sxs-lookup"><span data-stu-id="be120-138">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="be120-139">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="be120-139">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="be120-140">只读。</span><span class="sxs-lookup"><span data-stu-id="be120-140">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be120-141">关系</span><span class="sxs-lookup"><span data-stu-id="be120-141">Relationships</span></span>

<span data-ttu-id="be120-142">无。</span><span class="sxs-lookup"><span data-stu-id="be120-142">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="be120-143">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be120-143">JSON representation</span></span>

<span data-ttu-id="be120-144">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be120-144">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityBuiltInUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityBuiltInUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
