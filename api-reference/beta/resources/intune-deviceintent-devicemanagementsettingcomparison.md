---
title: deviceManagementSettingComparison 资源类型
description: 表示设置比较结果的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b10acc16cfb877a616dee9744daa5f0cc54b45b6
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275494"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="def13-103">deviceManagementSettingComparison 资源类型</span><span class="sxs-lookup"><span data-stu-id="def13-103">deviceManagementSettingComparison resource type</span></span>

<span data-ttu-id="def13-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="def13-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="def13-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="def13-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="def13-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="def13-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="def13-107">表示设置比较结果的实体</span><span class="sxs-lookup"><span data-stu-id="def13-107">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="def13-108">属性</span><span class="sxs-lookup"><span data-stu-id="def13-108">Properties</span></span>
|<span data-ttu-id="def13-109">属性</span><span class="sxs-lookup"><span data-stu-id="def13-109">Property</span></span>|<span data-ttu-id="def13-110">类型</span><span class="sxs-lookup"><span data-stu-id="def13-110">Type</span></span>|<span data-ttu-id="def13-111">说明</span><span class="sxs-lookup"><span data-stu-id="def13-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="def13-112">id</span><span class="sxs-lookup"><span data-stu-id="def13-112">id</span></span>|<span data-ttu-id="def13-113">字符串</span><span class="sxs-lookup"><span data-stu-id="def13-113">String</span></span>|<span data-ttu-id="def13-114">设置 ID</span><span class="sxs-lookup"><span data-stu-id="def13-114">The setting ID</span></span>|
|<span data-ttu-id="def13-115">displayName</span><span class="sxs-lookup"><span data-stu-id="def13-115">displayName</span></span>|<span data-ttu-id="def13-116">字符串</span><span class="sxs-lookup"><span data-stu-id="def13-116">String</span></span>|<span data-ttu-id="def13-117">设置的显示名称</span><span class="sxs-lookup"><span data-stu-id="def13-117">The setting's display name</span></span>|
|<span data-ttu-id="def13-118">definitionId</span><span class="sxs-lookup"><span data-stu-id="def13-118">definitionId</span></span>|<span data-ttu-id="def13-119">字符串</span><span class="sxs-lookup"><span data-stu-id="def13-119">String</span></span>|<span data-ttu-id="def13-120">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="def13-120">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="def13-121">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="def13-121">currentValueJson</span></span>|<span data-ttu-id="def13-122">字符串</span><span class="sxs-lookup"><span data-stu-id="def13-122">String</span></span>|<span data-ttu-id="def13-123">当前意向的 JSON 表示形式 (或) 模板设置的值</span><span class="sxs-lookup"><span data-stu-id="def13-123">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="def13-124">newValueJson</span><span class="sxs-lookup"><span data-stu-id="def13-124">newValueJson</span></span>|<span data-ttu-id="def13-125">字符串</span><span class="sxs-lookup"><span data-stu-id="def13-125">String</span></span>|<span data-ttu-id="def13-126">新模板设置值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="def13-126">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="def13-127">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="def13-127">comparisonResult</span></span>|[<span data-ttu-id="def13-128">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="def13-128">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="def13-129">设置比较结果。</span><span class="sxs-lookup"><span data-stu-id="def13-129">Setting comparison result.</span></span> <span data-ttu-id="def13-130">可取值为：`unknown`、`equal`、`notEqual`、`added`、`removed`。</span><span class="sxs-lookup"><span data-stu-id="def13-130">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="def13-131">关系</span><span class="sxs-lookup"><span data-stu-id="def13-131">Relationships</span></span>
<span data-ttu-id="def13-132">无</span><span class="sxs-lookup"><span data-stu-id="def13-132">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="def13-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="def13-133">JSON Representation</span></span>
<span data-ttu-id="def13-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="def13-134">Here is a JSON representation of the resource.</span></span>
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




