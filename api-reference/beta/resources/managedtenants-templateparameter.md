---
title: templateParameter 资源类型
description: 表示在管理模板中利用的参数。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: resourcePageType
ms.openlocfilehash: 4f533bc375e2d7e4a1e4ef2f7f801f248c1801c4
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402395"
---
# <a name="templateparameter-resource-type"></a><span data-ttu-id="2ddad-103">templateParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ddad-103">templateParameter resource type</span></span>

<span data-ttu-id="2ddad-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="2ddad-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ddad-105">表示在管理模板中利用的参数。</span><span class="sxs-lookup"><span data-stu-id="2ddad-105">Represents a parameter utilized in a management template.</span></span>

## <a name="properties"></a><span data-ttu-id="2ddad-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ddad-106">Properties</span></span>
|<span data-ttu-id="2ddad-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ddad-107">Property</span></span>|<span data-ttu-id="2ddad-108">类型</span><span class="sxs-lookup"><span data-stu-id="2ddad-108">Type</span></span>|<span data-ttu-id="2ddad-109">说明</span><span class="sxs-lookup"><span data-stu-id="2ddad-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ddad-110">说明</span><span class="sxs-lookup"><span data-stu-id="2ddad-110">description</span></span>|<span data-ttu-id="2ddad-111">String</span><span class="sxs-lookup"><span data-stu-id="2ddad-111">String</span></span>|<span data-ttu-id="2ddad-112">模板参数的说明。</span><span class="sxs-lookup"><span data-stu-id="2ddad-112">The description for the template parameter.</span></span> <span data-ttu-id="2ddad-113">可选。</span><span class="sxs-lookup"><span data-stu-id="2ddad-113">Optional.</span></span> <span data-ttu-id="2ddad-114">只读。</span><span class="sxs-lookup"><span data-stu-id="2ddad-114">Read-only.</span></span>|
|<span data-ttu-id="2ddad-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2ddad-115">displayName</span></span>|<span data-ttu-id="2ddad-116">String</span><span class="sxs-lookup"><span data-stu-id="2ddad-116">String</span></span>|<span data-ttu-id="2ddad-117">template 显示名称参数的值。</span><span class="sxs-lookup"><span data-stu-id="2ddad-117">The display name for the template parameter.</span></span> <span data-ttu-id="2ddad-118">必填。</span><span class="sxs-lookup"><span data-stu-id="2ddad-118">Required.</span></span> <span data-ttu-id="2ddad-119">只读。</span><span class="sxs-lookup"><span data-stu-id="2ddad-119">Read-only.</span></span>|
|<span data-ttu-id="2ddad-120">jsonAllowedValues</span><span class="sxs-lookup"><span data-stu-id="2ddad-120">jsonAllowedValues</span></span>|<span data-ttu-id="2ddad-121">String</span><span class="sxs-lookup"><span data-stu-id="2ddad-121">String</span></span>|<span data-ttu-id="2ddad-122">模板参数的允许值，由 JSON 的序列化字符串表示。</span><span class="sxs-lookup"><span data-stu-id="2ddad-122">The allowed values for the template parameter represented by a serialized string of JSON.</span></span> <span data-ttu-id="2ddad-123">可选。</span><span class="sxs-lookup"><span data-stu-id="2ddad-123">Optional.</span></span> <span data-ttu-id="2ddad-124">只读。</span><span class="sxs-lookup"><span data-stu-id="2ddad-124">Read-only.</span></span>|
|<span data-ttu-id="2ddad-125">jsonDefaultValue</span><span class="sxs-lookup"><span data-stu-id="2ddad-125">jsonDefaultValue</span></span>|<span data-ttu-id="2ddad-126">String</span><span class="sxs-lookup"><span data-stu-id="2ddad-126">String</span></span>|<span data-ttu-id="2ddad-127">模板参数的默认值，由 JSON 的序列化字符串表示。</span><span class="sxs-lookup"><span data-stu-id="2ddad-127">The default value for the template parameter represented by a serialized string of JSON.</span></span> <span data-ttu-id="2ddad-128">必填。</span><span class="sxs-lookup"><span data-stu-id="2ddad-128">Required.</span></span> <span data-ttu-id="2ddad-129">只读。</span><span class="sxs-lookup"><span data-stu-id="2ddad-129">Read-only.</span></span>|
|<span data-ttu-id="2ddad-130">valueType</span><span class="sxs-lookup"><span data-stu-id="2ddad-130">valueType</span></span>|<span data-ttu-id="2ddad-131">managementParameterValueType</span><span class="sxs-lookup"><span data-stu-id="2ddad-131">managementParameterValueType</span></span>|<span data-ttu-id="2ddad-132">模板数据类型参数的值。</span><span class="sxs-lookup"><span data-stu-id="2ddad-132">The data type for the template parameter..</span></span> <span data-ttu-id="2ddad-133">可取值为：`string`、`integer`、`boolean`、`guid`、`stringCollection`、`integerCollection`、`booleanCollection`、`guidCollection`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2ddad-133">Possible values are: `string`, `integer`, `boolean`, `guid`, `stringCollection`, `integerCollection`, `booleanCollection`, `guidCollection`, `unknownFutureValue`.</span></span> <span data-ttu-id="2ddad-134">必填。</span><span class="sxs-lookup"><span data-stu-id="2ddad-134">Required.</span></span> <span data-ttu-id="2ddad-135">只读。</span><span class="sxs-lookup"><span data-stu-id="2ddad-135">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2ddad-136">关系</span><span class="sxs-lookup"><span data-stu-id="2ddad-136">Relationships</span></span>
<span data-ttu-id="2ddad-137">无。</span><span class="sxs-lookup"><span data-stu-id="2ddad-137">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ddad-138">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ddad-138">JSON representation</span></span>
<span data-ttu-id="2ddad-139">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ddad-139">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managedTenants.templateParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedTenants.templateParameter",
  "displayName": "String",
  "description": "String",
  "valueType": "String",
  "jsonDefaultValue": "String",
  "jsonAllowedValues": "String"
}
```
