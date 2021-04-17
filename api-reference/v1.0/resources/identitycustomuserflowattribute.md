---
title: identityCustomUserFlowAttribute 资源类型
description: 表示 Azure Active Directory 租户中可用于自助服务注册用户流的自定义用户流属性。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: resourcePageType
ms.openlocfilehash: 2bb354ab8028a6d3ca96418c4b0566ea6fe195ef
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882989"
---
# <a name="identitycustomuserflowattribute-resource-type"></a><span data-ttu-id="91750-103">identityCustomUserFlowAttribute 资源类型</span><span class="sxs-lookup"><span data-stu-id="91750-103">identityCustomUserFlowAttribute resource type</span></span>

<span data-ttu-id="91750-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91750-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="91750-105">表示 Azure Active Directory 租户中可用于自助服务注册用户流的自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="91750-105">Represents a custom user flow attribute in Azure Active Directory tenants that can be used in a self-service sign-up user flow.</span></span> <span data-ttu-id="91750-106">这些属性无法修改且为只读。</span><span class="sxs-lookup"><span data-stu-id="91750-106">These attributes cannot be modified and are read-only.</span></span>

<span data-ttu-id="91750-107">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="91750-107">Inherits from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>

## <a name="properties"></a><span data-ttu-id="91750-108">属性</span><span class="sxs-lookup"><span data-stu-id="91750-108">Properties</span></span>

|<span data-ttu-id="91750-109">属性</span><span class="sxs-lookup"><span data-stu-id="91750-109">Property</span></span>|<span data-ttu-id="91750-110">类型</span><span class="sxs-lookup"><span data-stu-id="91750-110">Type</span></span>|<span data-ttu-id="91750-111">说明</span><span class="sxs-lookup"><span data-stu-id="91750-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91750-112">id</span><span class="sxs-lookup"><span data-stu-id="91750-112">id</span></span>|<span data-ttu-id="91750-113">String</span><span class="sxs-lookup"><span data-stu-id="91750-113">String</span></span>|<span data-ttu-id="91750-114">用户流属性的标识符。</span><span class="sxs-lookup"><span data-stu-id="91750-114">The identifier of the user flow attribute.</span></span> <span data-ttu-id="91750-115">这是一个自动创建的只读属性。</span><span class="sxs-lookup"><span data-stu-id="91750-115">This is a read-only attribute that is automatically created.</span></span> <span data-ttu-id="91750-116">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="91750-116">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="91750-117">displayName</span><span class="sxs-lookup"><span data-stu-id="91750-117">displayName</span></span>|<span data-ttu-id="91750-118">String</span><span class="sxs-lookup"><span data-stu-id="91750-118">String</span></span>|<span data-ttu-id="91750-119">用户流属性的显示名称。</span><span class="sxs-lookup"><span data-stu-id="91750-119">The display name of the user flow attribute.</span></span> <span data-ttu-id="91750-120">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="91750-120">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="91750-121">说明</span><span class="sxs-lookup"><span data-stu-id="91750-121">description</span></span>|<span data-ttu-id="91750-122">String</span><span class="sxs-lookup"><span data-stu-id="91750-122">String</span></span>|<span data-ttu-id="91750-123">注册时显示给用户的用户流量属性的描述。</span><span class="sxs-lookup"><span data-stu-id="91750-123">The description of the user flow attribute that's shown to the user at the time of sign-up.</span></span> <span data-ttu-id="91750-124">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span><span class="sxs-lookup"><span data-stu-id="91750-124">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md)</span></span>|
|<span data-ttu-id="91750-125">userFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="91750-125">userFlowAttributeType</span></span>|<span data-ttu-id="91750-126">identityUserFlowAttributeType</span><span class="sxs-lookup"><span data-stu-id="91750-126">identityUserFlowAttributeType</span></span>|<span data-ttu-id="91750-127">用户流属性的类型。</span><span class="sxs-lookup"><span data-stu-id="91750-127">The type of the user flow attribute.</span></span> <span data-ttu-id="91750-128">这是一个自动设置的只读属性。</span><span class="sxs-lookup"><span data-stu-id="91750-128">This is a read-only attribute that is automatically set.</span></span> <span data-ttu-id="91750-129">此属性的值将为 `custom` 。</span><span class="sxs-lookup"><span data-stu-id="91750-129">The value for this property will be `custom`.</span></span> <span data-ttu-id="91750-130">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="91750-130">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>|
|<span data-ttu-id="91750-131">DataType</span><span class="sxs-lookup"><span data-stu-id="91750-131">dataType</span></span>|<span data-ttu-id="91750-132">identityUserFlowAttributeDataType</span><span class="sxs-lookup"><span data-stu-id="91750-132">identityUserFlowAttributeDataType</span></span>|<span data-ttu-id="91750-133">用户流属性的数据类型。</span><span class="sxs-lookup"><span data-stu-id="91750-133">The data type of the user flow attribute.</span></span> <span data-ttu-id="91750-134">在创建自定义用户流属性后，不能对此进行修改。</span><span class="sxs-lookup"><span data-stu-id="91750-134">This cannot be modified after the custom user flow attribute is created.</span></span> <span data-ttu-id="91750-135">数据类型 **支持** 为： `string` 、 `boolean` 、 `int64` 、 `stringCollection` 、 `dateTime`。</span><span class="sxs-lookup"><span data-stu-id="91750-135">The supported values for **dataType** are: `string` , `boolean` , `int64` , `stringCollection` , `dateTime`.</span></span> <span data-ttu-id="91750-136">继承自 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="91750-136">Inherited from [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span>|

## <a name="relationships"></a><span data-ttu-id="91750-137">关系</span><span class="sxs-lookup"><span data-stu-id="91750-137">Relationships</span></span>

<span data-ttu-id="91750-138">无。</span><span class="sxs-lookup"><span data-stu-id="91750-138">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="91750-139">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="91750-139">JSON representation</span></span>

<span data-ttu-id="91750-140">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91750-140">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.identityCustomUserFlowAttribute",
  "baseType": "microsoft.graph.identityUserFlowAttribute",
  "openType": false
}
-->

``` json
{
  "@odata.type": "#microsoft.graph.identityCustomUserFlowAttribute",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "userFlowAttributeType": "String",
  "dataType": "String"
}
```
