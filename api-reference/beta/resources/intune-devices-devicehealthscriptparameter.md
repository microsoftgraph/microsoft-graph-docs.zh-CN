---
title: deviceHealthScriptParameter 资源类型
description: Script 参数的 Base 属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a11915af80b10944fe6a3573d5293c19e3fc0357
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48729346"
---
# <a name="devicehealthscriptparameter-resource-type"></a><span data-ttu-id="1e056-103">deviceHealthScriptParameter 资源类型</span><span class="sxs-lookup"><span data-stu-id="1e056-103">deviceHealthScriptParameter resource type</span></span>

<span data-ttu-id="1e056-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e056-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1e056-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1e056-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e056-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1e056-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e056-107">Script 参数的 Base 属性。</span><span class="sxs-lookup"><span data-stu-id="1e056-107">Base properties of the script parameter.</span></span>

## <a name="properties"></a><span data-ttu-id="1e056-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e056-108">Properties</span></span>
|<span data-ttu-id="1e056-109">属性</span><span class="sxs-lookup"><span data-stu-id="1e056-109">Property</span></span>|<span data-ttu-id="1e056-110">类型</span><span class="sxs-lookup"><span data-stu-id="1e056-110">Type</span></span>|<span data-ttu-id="1e056-111">说明</span><span class="sxs-lookup"><span data-stu-id="1e056-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e056-112">name</span><span class="sxs-lookup"><span data-stu-id="1e056-112">name</span></span>|<span data-ttu-id="1e056-113">String</span><span class="sxs-lookup"><span data-stu-id="1e056-113">String</span></span>|<span data-ttu-id="1e056-114">参数的名称</span><span class="sxs-lookup"><span data-stu-id="1e056-114">The name of the param</span></span>|
|<span data-ttu-id="1e056-115">说明</span><span class="sxs-lookup"><span data-stu-id="1e056-115">description</span></span>|<span data-ttu-id="1e056-116">String</span><span class="sxs-lookup"><span data-stu-id="1e056-116">String</span></span>|<span data-ttu-id="1e056-117">参数的说明</span><span class="sxs-lookup"><span data-stu-id="1e056-117">The description of the param</span></span>|
|<span data-ttu-id="1e056-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="1e056-118">isRequired</span></span>|<span data-ttu-id="1e056-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e056-119">Boolean</span></span>|<span data-ttu-id="1e056-120">Param 是否是必需的</span><span class="sxs-lookup"><span data-stu-id="1e056-120">Whether the param is required</span></span>|
|<span data-ttu-id="1e056-121">applyDefaultValueWhenNotAssigned</span><span class="sxs-lookup"><span data-stu-id="1e056-121">applyDefaultValueWhenNotAssigned</span></span>|<span data-ttu-id="1e056-122">布尔</span><span class="sxs-lookup"><span data-stu-id="1e056-122">Boolean</span></span>|<span data-ttu-id="1e056-123">未赋值时是否应用 DefaultValue</span><span class="sxs-lookup"><span data-stu-id="1e056-123">Whether Apply DefaultValue When Not Assigned</span></span>|

## <a name="relationships"></a><span data-ttu-id="1e056-124">关系</span><span class="sxs-lookup"><span data-stu-id="1e056-124">Relationships</span></span>
<span data-ttu-id="1e056-125">无</span><span class="sxs-lookup"><span data-stu-id="1e056-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1e056-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="1e056-126">JSON Representation</span></span>
<span data-ttu-id="1e056-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e056-127">Here is a JSON representation of the resource.</span></span>
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





