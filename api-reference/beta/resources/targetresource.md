---
title: targetResource 资源复杂类型-Microsoft Graph API
description: 定义支持 (租户) 活动的审核日志报告组织的 Microsoft Graph API 的 targetResource 实体资源复杂类型。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: bec25af7e0f39a4adf15577c21d4141e1a3c431a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47985648"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="1e27b-103">targetResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e27b-103">targetResource resource type</span></span>

<span data-ttu-id="1e27b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e27b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="1e27b-105">表示与审核活动相关联的目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="1e27b-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="1e27b-106">属性</span><span class="sxs-lookup"><span data-stu-id="1e27b-106">Properties</span></span>

| <span data-ttu-id="1e27b-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e27b-107">Property</span></span>     | <span data-ttu-id="1e27b-108">类型</span><span class="sxs-lookup"><span data-stu-id="1e27b-108">Type</span></span>   |<span data-ttu-id="1e27b-109">说明</span><span class="sxs-lookup"><span data-stu-id="1e27b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1e27b-110">id</span><span class="sxs-lookup"><span data-stu-id="1e27b-110">id</span></span>|<span data-ttu-id="1e27b-111">String</span><span class="sxs-lookup"><span data-stu-id="1e27b-111">String</span></span>|<span data-ttu-id="1e27b-112">指示资源的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="1e27b-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="1e27b-113">displayName</span><span class="sxs-lookup"><span data-stu-id="1e27b-113">displayName</span></span>|<span data-ttu-id="1e27b-114">String</span><span class="sxs-lookup"><span data-stu-id="1e27b-114">String</span></span>|<span data-ttu-id="1e27b-115">指示为资源定义的可见名称。</span><span class="sxs-lookup"><span data-stu-id="1e27b-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="1e27b-116">通常是在创建资源时指定的。</span><span class="sxs-lookup"><span data-stu-id="1e27b-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="1e27b-117">type</span><span class="sxs-lookup"><span data-stu-id="1e27b-117">type</span></span>|<span data-ttu-id="1e27b-118">String</span><span class="sxs-lookup"><span data-stu-id="1e27b-118">String</span></span>|<span data-ttu-id="1e27b-119">描述资源类型。</span><span class="sxs-lookup"><span data-stu-id="1e27b-119">Describes the resource type.</span></span>  <span data-ttu-id="1e27b-120">示例值包括 `Application` 、 `Group` 、 `ServicePrincipal` 和 `User` 。</span><span class="sxs-lookup"><span data-stu-id="1e27b-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="1e27b-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="1e27b-121">userPrincipalName</span></span>|<span data-ttu-id="1e27b-122">String</span><span class="sxs-lookup"><span data-stu-id="1e27b-122">String</span></span>|<span data-ttu-id="1e27b-123">当 " **类型** " 设置为时 `User` ，其中包括启动操作的用户名; `null` 针对其他类型。</span><span class="sxs-lookup"><span data-stu-id="1e27b-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="1e27b-124">groupType</span><span class="sxs-lookup"><span data-stu-id="1e27b-124">groupType</span></span>|<span data-ttu-id="1e27b-125">String</span><span class="sxs-lookup"><span data-stu-id="1e27b-125">String</span></span>|<span data-ttu-id="1e27b-126">当 " **类型** " 设置为时 `Group` ，这表示组类型。</span><span class="sxs-lookup"><span data-stu-id="1e27b-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="1e27b-127">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="1e27b-127">modifiedProperties</span></span>|<span data-ttu-id="1e27b-128">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="1e27b-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="1e27b-129">指示已更改的每个属性的名称、旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="1e27b-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="1e27b-130">属性值取决于操作 **类型**。</span><span class="sxs-lookup"><span data-stu-id="1e27b-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1e27b-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e27b-131">JSON representation</span></span>

<span data-ttu-id="1e27b-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e27b-132">Here is a JSON representation of the resource.</span></span>

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


