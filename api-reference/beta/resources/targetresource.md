---
title: targetResource 资源复杂类型-Microsoft Graph API
description: 定义支持审核日志报告组织 (租户) 活动的 Microsoft Graph API 的 targetResource 实体资源复杂类型。
author: davidmu1
localization_priority: Normal
doc_type: resourcePageType
ms.prod: azure-ad
ms.openlocfilehash: a67cfbccf9d05872ec0d9207ac54c51cda222053
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964576"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="b6258-103">targetResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="b6258-103">targetResource resource type</span></span>

<span data-ttu-id="b6258-104">表示与审核活动相关联的目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="b6258-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="b6258-105">属性</span><span class="sxs-lookup"><span data-stu-id="b6258-105">Properties</span></span>

| <span data-ttu-id="b6258-106">属性</span><span class="sxs-lookup"><span data-stu-id="b6258-106">Property</span></span>     | <span data-ttu-id="b6258-107">类型</span><span class="sxs-lookup"><span data-stu-id="b6258-107">Type</span></span>   |<span data-ttu-id="b6258-108">说明</span><span class="sxs-lookup"><span data-stu-id="b6258-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6258-109">id</span><span class="sxs-lookup"><span data-stu-id="b6258-109">id</span></span>|<span data-ttu-id="b6258-110">String</span><span class="sxs-lookup"><span data-stu-id="b6258-110">String</span></span>|<span data-ttu-id="b6258-111">指示资源的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="b6258-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="b6258-112">displayName</span><span class="sxs-lookup"><span data-stu-id="b6258-112">displayName</span></span>|<span data-ttu-id="b6258-113">String</span><span class="sxs-lookup"><span data-stu-id="b6258-113">String</span></span>|<span data-ttu-id="b6258-114">指示为资源定义的可见名称。</span><span class="sxs-lookup"><span data-stu-id="b6258-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="b6258-115">通常是在创建资源时指定的。</span><span class="sxs-lookup"><span data-stu-id="b6258-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="b6258-116">type</span><span class="sxs-lookup"><span data-stu-id="b6258-116">type</span></span>|<span data-ttu-id="b6258-117">String</span><span class="sxs-lookup"><span data-stu-id="b6258-117">String</span></span>|<span data-ttu-id="b6258-118">描述资源类型。</span><span class="sxs-lookup"><span data-stu-id="b6258-118">Describes the resource type.</span></span>  <span data-ttu-id="b6258-119">示例值包括`Application`、 `Group`、 `ServicePrincipal`和`User`。</span><span class="sxs-lookup"><span data-stu-id="b6258-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="b6258-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6258-120">userPrincipalName</span></span>|<span data-ttu-id="b6258-121">字符串</span><span class="sxs-lookup"><span data-stu-id="b6258-121">String</span></span>|<span data-ttu-id="b6258-122">当 "**类型**" 设置`User`为时, 这包括启动操作的用户名;`null`对于其他类型。</span><span class="sxs-lookup"><span data-stu-id="b6258-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="b6258-123">groupType</span><span class="sxs-lookup"><span data-stu-id="b6258-123">groupType</span></span>|<span data-ttu-id="b6258-124">String</span><span class="sxs-lookup"><span data-stu-id="b6258-124">String</span></span>|<span data-ttu-id="b6258-125">当 "**类型**" 设置`Group`为时, 这表示组类型。</span><span class="sxs-lookup"><span data-stu-id="b6258-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="b6258-126">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="b6258-126">modifiedProperties</span></span>|<span data-ttu-id="b6258-127">[modifiedProperty](modifiedproperty.md)集合</span><span class="sxs-lookup"><span data-stu-id="b6258-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="b6258-128">指示已更改的每个属性的名称、旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="b6258-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="b6258-129">属性值取决于操作**类型**。</span><span class="sxs-lookup"><span data-stu-id="b6258-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b6258-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b6258-130">JSON representation</span></span>

<span data-ttu-id="b6258-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6258-131">Here is a JSON representation of the resource.</span></span>

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
