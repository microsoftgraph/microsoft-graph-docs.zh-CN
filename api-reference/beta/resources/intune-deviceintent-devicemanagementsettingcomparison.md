---
title: deviceManagementSettingComparison 资源类型
description: 表示设置比较结果的实体
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5a91dc3ce4cb7e8730f346800d53740db78e5526
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785349"
---
# <a name="devicemanagementsettingcomparison-resource-type"></a><span data-ttu-id="be730-103">deviceManagementSettingComparison 资源类型</span><span class="sxs-lookup"><span data-stu-id="be730-103">deviceManagementSettingComparison resource type</span></span>

> <span data-ttu-id="be730-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="be730-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="be730-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="be730-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="be730-106">表示设置比较结果的实体</span><span class="sxs-lookup"><span data-stu-id="be730-106">Entity representing setting comparison result</span></span>

## <a name="properties"></a><span data-ttu-id="be730-107">属性</span><span class="sxs-lookup"><span data-stu-id="be730-107">Properties</span></span>
|<span data-ttu-id="be730-108">属性</span><span class="sxs-lookup"><span data-stu-id="be730-108">Property</span></span>|<span data-ttu-id="be730-109">类型</span><span class="sxs-lookup"><span data-stu-id="be730-109">Type</span></span>|<span data-ttu-id="be730-110">说明</span><span class="sxs-lookup"><span data-stu-id="be730-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="be730-111">id</span><span class="sxs-lookup"><span data-stu-id="be730-111">id</span></span>|<span data-ttu-id="be730-112">String</span><span class="sxs-lookup"><span data-stu-id="be730-112">String</span></span>|<span data-ttu-id="be730-113">设置 ID</span><span class="sxs-lookup"><span data-stu-id="be730-113">The setting ID</span></span>|
|<span data-ttu-id="be730-114">displayName</span><span class="sxs-lookup"><span data-stu-id="be730-114">displayName</span></span>|<span data-ttu-id="be730-115">String</span><span class="sxs-lookup"><span data-stu-id="be730-115">String</span></span>|<span data-ttu-id="be730-116">设置的显示名称</span><span class="sxs-lookup"><span data-stu-id="be730-116">The setting's display name</span></span>|
|<span data-ttu-id="be730-117">definitionId</span><span class="sxs-lookup"><span data-stu-id="be730-117">definitionId</span></span>|<span data-ttu-id="be730-118">String</span><span class="sxs-lookup"><span data-stu-id="be730-118">String</span></span>|<span data-ttu-id="be730-119">此实例的设置定义的 ID</span><span class="sxs-lookup"><span data-stu-id="be730-119">The ID of the setting definition for this instance</span></span>|
|<span data-ttu-id="be730-120">currentValueJson</span><span class="sxs-lookup"><span data-stu-id="be730-120">currentValueJson</span></span>|<span data-ttu-id="be730-121">String</span><span class="sxs-lookup"><span data-stu-id="be730-121">String</span></span>|<span data-ttu-id="be730-122">当前意图（或）模板设置值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be730-122">JSON representation of current intent (or) template setting's value</span></span>|
|<span data-ttu-id="be730-123">newValueJson</span><span class="sxs-lookup"><span data-stu-id="be730-123">newValueJson</span></span>|<span data-ttu-id="be730-124">String</span><span class="sxs-lookup"><span data-stu-id="be730-124">String</span></span>|<span data-ttu-id="be730-125">新模板设置值的 JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be730-125">JSON representation of new template setting's value</span></span>|
|<span data-ttu-id="be730-126">comparisonResult</span><span class="sxs-lookup"><span data-stu-id="be730-126">comparisonResult</span></span>|[<span data-ttu-id="be730-127">deviceManagementComparisonResult</span><span class="sxs-lookup"><span data-stu-id="be730-127">deviceManagementComparisonResult</span></span>](../resources/intune-deviceintent-devicemanagementcomparisonresult.md)|<span data-ttu-id="be730-128">设置比较结果。</span><span class="sxs-lookup"><span data-stu-id="be730-128">Setting comparison result.</span></span> <span data-ttu-id="be730-129">可取值为：`unknown`、`equal`、`notEqual`、`added`、`removed`。</span><span class="sxs-lookup"><span data-stu-id="be730-129">Possible values are: `unknown`, `equal`, `notEqual`, `added`, `removed`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="be730-130">关系</span><span class="sxs-lookup"><span data-stu-id="be730-130">Relationships</span></span>
<span data-ttu-id="be730-131">无</span><span class="sxs-lookup"><span data-stu-id="be730-131">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="be730-132">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="be730-132">JSON Representation</span></span>
<span data-ttu-id="be730-133">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="be730-133">Here is a JSON representation of the resource.</span></span>
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



