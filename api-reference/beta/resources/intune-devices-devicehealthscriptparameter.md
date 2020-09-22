---
title: deviceHealthScriptParameter 资源类型
description: Script 参数的 Base 属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ad82da1915702448a62c0c99f6933ddf1a51c5b1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48060298"
---
# <a name="devicehealthscriptparameter-resource-type"></a><span data-ttu-id="68a9e-103">deviceHealthScriptParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="68a9e-103">deviceHealthScriptParameter resource type</span></span>

<span data-ttu-id="68a9e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="68a9e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="68a9e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="68a9e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68a9e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="68a9e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68a9e-107">Script 参数的 Base 属性。</span><span class="sxs-lookup"><span data-stu-id="68a9e-107">Base properties of the script parameter.</span></span>

## <a name="properties"></a><span data-ttu-id="68a9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="68a9e-108">Properties</span></span>
|<span data-ttu-id="68a9e-109">属性</span><span class="sxs-lookup"><span data-stu-id="68a9e-109">Property</span></span>|<span data-ttu-id="68a9e-110">类型</span><span class="sxs-lookup"><span data-stu-id="68a9e-110">Type</span></span>|<span data-ttu-id="68a9e-111">说明</span><span class="sxs-lookup"><span data-stu-id="68a9e-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68a9e-112">名称</span><span class="sxs-lookup"><span data-stu-id="68a9e-112">name</span></span>|<span data-ttu-id="68a9e-113">String</span><span class="sxs-lookup"><span data-stu-id="68a9e-113">String</span></span>|<span data-ttu-id="68a9e-114">参数的名称</span><span class="sxs-lookup"><span data-stu-id="68a9e-114">The name of the param</span></span>|
|<span data-ttu-id="68a9e-115">说明</span><span class="sxs-lookup"><span data-stu-id="68a9e-115">description</span></span>|<span data-ttu-id="68a9e-116">String</span><span class="sxs-lookup"><span data-stu-id="68a9e-116">String</span></span>|<span data-ttu-id="68a9e-117">参数的说明</span><span class="sxs-lookup"><span data-stu-id="68a9e-117">The description of the param</span></span>|
|<span data-ttu-id="68a9e-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="68a9e-118">isRequired</span></span>|<span data-ttu-id="68a9e-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="68a9e-119">Boolean</span></span>|<span data-ttu-id="68a9e-120">Param 是否是必需的</span><span class="sxs-lookup"><span data-stu-id="68a9e-120">Whether the param is required</span></span>|
|<span data-ttu-id="68a9e-121">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="68a9e-121">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="68a9e-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="68a9e-122">Boolean</span></span>|<span data-ttu-id="68a9e-123">未赋值时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="68a9e-123">Whether Apply DefaultValue When Not Assigned</span></span>|

## <a name="relationships"></a><span data-ttu-id="68a9e-124">关系</span><span class="sxs-lookup"><span data-stu-id="68a9e-124">Relationships</span></span>
<span data-ttu-id="68a9e-125">无</span><span class="sxs-lookup"><span data-stu-id="68a9e-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68a9e-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="68a9e-126">JSON Representation</span></span>
<span data-ttu-id="68a9e-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="68a9e-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceHealthScriptParameter"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceHealthScriptParameter",
  "name": "String",
  "description": "String",
  "isRequired": true,
  "applyDefaultValueWhenNotAssigned": true
}
```






