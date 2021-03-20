---
title: targetResource 资源类型
description: 表示与审核活动关联的目标资源类型。
localization_priority: Normal
author: dhanyahk
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 148591f603a45d0e8752e4af87beaabd39152fae
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961886"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="a48b6-103">targetResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="a48b6-103">targetResource resource type</span></span>

<span data-ttu-id="a48b6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a48b6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a48b6-105">表示与审核活动关联的目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="a48b6-105">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="a48b6-106">属性</span><span class="sxs-lookup"><span data-stu-id="a48b6-106">Properties</span></span>

| <span data-ttu-id="a48b6-107">属性</span><span class="sxs-lookup"><span data-stu-id="a48b6-107">Property</span></span>     | <span data-ttu-id="a48b6-108">类型</span><span class="sxs-lookup"><span data-stu-id="a48b6-108">Type</span></span>   |<span data-ttu-id="a48b6-109">说明</span><span class="sxs-lookup"><span data-stu-id="a48b6-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a48b6-110">id</span><span class="sxs-lookup"><span data-stu-id="a48b6-110">id</span></span>|<span data-ttu-id="a48b6-111">String</span><span class="sxs-lookup"><span data-stu-id="a48b6-111">String</span></span>|<span data-ttu-id="a48b6-112">指示资源的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="a48b6-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="a48b6-113">displayName</span><span class="sxs-lookup"><span data-stu-id="a48b6-113">displayName</span></span>|<span data-ttu-id="a48b6-114">String</span><span class="sxs-lookup"><span data-stu-id="a48b6-114">String</span></span>|<span data-ttu-id="a48b6-115">指示为资源定义的可见名称。</span><span class="sxs-lookup"><span data-stu-id="a48b6-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="a48b6-116">通常在创建资源时指定。</span><span class="sxs-lookup"><span data-stu-id="a48b6-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="a48b6-117">type</span><span class="sxs-lookup"><span data-stu-id="a48b6-117">type</span></span>|<span data-ttu-id="a48b6-118">String</span><span class="sxs-lookup"><span data-stu-id="a48b6-118">String</span></span>|<span data-ttu-id="a48b6-119">描述资源类型。</span><span class="sxs-lookup"><span data-stu-id="a48b6-119">Describes the resource type.</span></span>  <span data-ttu-id="a48b6-120">示例值包括 `Application` 、 、 和 `Group` `ServicePrincipal` `User` 。</span><span class="sxs-lookup"><span data-stu-id="a48b6-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="a48b6-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a48b6-121">userPrincipalName</span></span>|<span data-ttu-id="a48b6-122">String</span><span class="sxs-lookup"><span data-stu-id="a48b6-122">String</span></span>|<span data-ttu-id="a48b6-123">当 **type** 设置为 `User` 时，这包括启动该操作的用户名; `null` 对于其他类型。</span><span class="sxs-lookup"><span data-stu-id="a48b6-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="a48b6-124">groupType</span><span class="sxs-lookup"><span data-stu-id="a48b6-124">groupType</span></span>|<span data-ttu-id="a48b6-125">groupType</span><span class="sxs-lookup"><span data-stu-id="a48b6-125">groupType</span></span>|<span data-ttu-id="a48b6-126">当 **type** 设置为 `Group` 时，这表示组类型。</span><span class="sxs-lookup"><span data-stu-id="a48b6-126">When **type** is set to `Group`, this indicates the group type.</span></span> <span data-ttu-id="a48b6-127">可能的值包括 `unifiedGroups` ：、 `azureAD` 和 `unknownFutureValue`</span><span class="sxs-lookup"><span data-stu-id="a48b6-127">Possible values are: `unifiedGroups`, `azureAD`, and `unknownFutureValue`</span></span>|
|<span data-ttu-id="a48b6-128">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="a48b6-128">modifiedProperties</span></span>|<span data-ttu-id="a48b6-129">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a48b6-129">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="a48b6-130">指示更改的每个属性的名称、旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="a48b6-130">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="a48b6-131">属性值取决于操作 **类型**。</span><span class="sxs-lookup"><span data-stu-id="a48b6-131">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a48b6-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a48b6-132">JSON representation</span></span>

<span data-ttu-id="a48b6-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a48b6-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

