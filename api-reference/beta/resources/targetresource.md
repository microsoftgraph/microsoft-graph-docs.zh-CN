---
title: targetResource 资源复杂类型 - Microsoft Graph API
description: 定义 Microsoft Graph API 的 targetResource 实体资源复杂类型，该类型审核日志报告 (租户) 活动。
author: cloudhandler
localization_priority: Normal
doc_type: resourcePageType
ms.prod: identity-and-access-reports
ms.openlocfilehash: 2dc8adea2edf11674d844cee4e5548da96882f7d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50137583"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="95beb-103">targetResource 资源类型</span><span class="sxs-lookup"><span data-stu-id="95beb-103">targetResource resource type</span></span>

<span data-ttu-id="95beb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="95beb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="95beb-105">表示与审核活动关联的目标资源类型。</span><span class="sxs-lookup"><span data-stu-id="95beb-105">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="95beb-106">属性</span><span class="sxs-lookup"><span data-stu-id="95beb-106">Properties</span></span>

| <span data-ttu-id="95beb-107">属性</span><span class="sxs-lookup"><span data-stu-id="95beb-107">Property</span></span>     | <span data-ttu-id="95beb-108">类型</span><span class="sxs-lookup"><span data-stu-id="95beb-108">Type</span></span>   |<span data-ttu-id="95beb-109">说明</span><span class="sxs-lookup"><span data-stu-id="95beb-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="95beb-110">id</span><span class="sxs-lookup"><span data-stu-id="95beb-110">id</span></span>|<span data-ttu-id="95beb-111">字符串</span><span class="sxs-lookup"><span data-stu-id="95beb-111">String</span></span>|<span data-ttu-id="95beb-112">指示资源的唯一 ID。</span><span class="sxs-lookup"><span data-stu-id="95beb-112">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="95beb-113">displayName</span><span class="sxs-lookup"><span data-stu-id="95beb-113">displayName</span></span>|<span data-ttu-id="95beb-114">字符串</span><span class="sxs-lookup"><span data-stu-id="95beb-114">String</span></span>|<span data-ttu-id="95beb-115">指示为资源定义的可见名称。</span><span class="sxs-lookup"><span data-stu-id="95beb-115">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="95beb-116">通常在创建资源时指定。</span><span class="sxs-lookup"><span data-stu-id="95beb-116">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="95beb-117">type</span><span class="sxs-lookup"><span data-stu-id="95beb-117">type</span></span>|<span data-ttu-id="95beb-118">字符串</span><span class="sxs-lookup"><span data-stu-id="95beb-118">String</span></span>|<span data-ttu-id="95beb-119">描述资源类型。</span><span class="sxs-lookup"><span data-stu-id="95beb-119">Describes the resource type.</span></span>  <span data-ttu-id="95beb-120">示例值包括 `Application` 、 `Group` 和 `ServicePrincipal` `User` 。</span><span class="sxs-lookup"><span data-stu-id="95beb-120">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="95beb-121">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="95beb-121">userPrincipalName</span></span>|<span data-ttu-id="95beb-122">字符串</span><span class="sxs-lookup"><span data-stu-id="95beb-122">String</span></span>|<span data-ttu-id="95beb-123">当 **类型** 设置为 `User` 时，这包括启动该操作的用户名; `null` 对于其他类型的用户。</span><span class="sxs-lookup"><span data-stu-id="95beb-123">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="95beb-124">groupType</span><span class="sxs-lookup"><span data-stu-id="95beb-124">groupType</span></span>|<span data-ttu-id="95beb-125">字符串</span><span class="sxs-lookup"><span data-stu-id="95beb-125">String</span></span>|<span data-ttu-id="95beb-126">当 **类型** 设置为 `Group` 时，这表示组类型。</span><span class="sxs-lookup"><span data-stu-id="95beb-126">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="95beb-127">ModifiedProperties</span><span class="sxs-lookup"><span data-stu-id="95beb-127">modifiedProperties</span></span>|<span data-ttu-id="95beb-128">[modifiedProperty](modifiedproperty.md) 集合</span><span class="sxs-lookup"><span data-stu-id="95beb-128">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="95beb-129">指示更改的每个属性的名称、旧值和新值。</span><span class="sxs-lookup"><span data-stu-id="95beb-129">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="95beb-130">属性值取决于操作 **类型**。</span><span class="sxs-lookup"><span data-stu-id="95beb-130">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="95beb-131">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="95beb-131">JSON representation</span></span>

<span data-ttu-id="95beb-132">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95beb-132">Here is a JSON representation of the resource.</span></span>

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


