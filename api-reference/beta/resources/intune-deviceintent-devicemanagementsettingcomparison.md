---
title: deviceManagementSettingComparison 资源类型
description: 表示设置比较结果的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 5e51d413dfa0e1e60fcf07e37c2806c39f62cc76
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48061243"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="2f937-103">deviceManagementSettingComparison 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f937-103">deviceManagementSettingComparison resource type</span></span>

<span data-ttu-id="2f937-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2f937-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2f937-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2f937-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2f937-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2f937-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f937-107">表示设置比较结果的实体</span><span class="sxs-lookup"><span data-stu-id="2f937-107">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="2f937-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f937-108">Properties</span></span>
|<span data-ttu-id="2f937-109">属性</span><span class="sxs-lookup"><span data-stu-id="2f937-109">Property</span></span>|<span data-ttu-id="2f937-110">类型</span><span class="sxs-lookup"><span data-stu-id="2f937-110">Type</span></span>|<span data-ttu-id="2f937-111">说明</span><span class="sxs-lookup"><span data-stu-id="2f937-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f937-112">id</span><span class="sxs-lookup"><span data-stu-id="2f937-112">id</span></span>|<span data-ttu-id="2f937-113">String</span><span class="sxs-lookup"><span data-stu-id="2f937-113">String</span></span>|<span data-ttu-id="2f937-114">设置 ID</span><span class="sxs-lookup"><span data-stu-id="2f937-114">The setting ID</span></span>|
|<span data-ttu-id="2f937-115">displayName</span><span class="sxs-lookup"><span data-stu-id="2f937-115">displayName</span></span>|<span data-ttu-id="2f937-116">String</span><span class="sxs-lookup"><span data-stu-id="2f937-116">String</span></span>|<span data-ttu-id="2f937-117">设置的显示名称</span><span class="sxs-lookup"><span data-stu-id="2f937-117">The setting's display name</span></span>|
|<span data-ttu-id="2f937-118">definitionId</span><span class="sxs-lookup"><span data-stu-id="2f937-118">definitionId</span></span>|<span data-ttu-id="2f937-119">String</span><span class="sxs-lookup"><span data-stu-id="2f937-119">String</span></span>|<span data-ttu-id="2f937-120">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="2f937-120">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="2f937-121">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="2f937-121">currentValueJson</span></span>|<span data-ttu-id="2f937-122">String</span><span class="sxs-lookup"><span data-stu-id="2f937-122">String</span></span>|<span data-ttu-id="2f937-123">当前意向的 JSON 表示形式 (或) 模板设置的值</span><span class="sxs-lookup"><span data-stu-id="2f937-123">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="2f937-124">newValueJson</span><span class="sxs-lookup"><span data-stu-id="2f937-124">newValueJson</span></span>|<span data-ttu-id="2f937-125">String</span><span class="sxs-lookup"><span data-stu-id="2f937-125">String</span></span>|<span data-ttu-id="2f937-126">新模板设置值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f937-126">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="2f937-127">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="2f937-127">comparisonResult</span></span>|[<span data-ttu-id="2f937-128">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="2f937-128">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="2f937-129">设置比较结果。</span><span class="sxs-lookup"><span data-stu-id="2f937-129">Setting comparison result.</span></span> <span data-ttu-id="2f937-130">可取值为：`unknown`、`equal`、`notEqual`、`added`、`removed`。</span><span class="sxs-lookup"><span data-stu-id="2f937-130">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f937-131">关系</span><span class="sxs-lookup"><span data-stu-id="2f937-131">Relationships</span></span>
<span data-ttu-id="2f937-132">无</span><span class="sxs-lookup"><span data-stu-id="2f937-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f937-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f937-133">JSON Representation</span></span>
<span data-ttu-id="2f937-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f937-134">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementSettingComparison"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettingComparison",
  "id": "String (identifier)",
  "displayName": "String",
  "definitionId": "String",
  "currentValueJson": "String",
  "newValueJson": "String",
  "comparisonResult": "String"
}
```






