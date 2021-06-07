---
title: resourceAction 资源类型
description: 资源允许和不允许的操作集。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 3517a4608691b65ce33ac40b4a9d9929bd277f31
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52752432"
---
# <a name="resourceaction-resource-type"></a><span data-ttu-id="5eaef-103">resourceAction 资源类型</span><span class="sxs-lookup"><span data-stu-id="5eaef-103">resourceAction resource type</span></span>

<span data-ttu-id="5eaef-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5eaef-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5eaef-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5eaef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5eaef-106">资源允许和不允许的操作集。</span><span class="sxs-lookup"><span data-stu-id="5eaef-106">Set of allowed and not allowed actions for a resource.</span></span>

## <a name="properties"></a><span data-ttu-id="5eaef-107">属性</span><span class="sxs-lookup"><span data-stu-id="5eaef-107">Properties</span></span>
|<span data-ttu-id="5eaef-108">属性</span><span class="sxs-lookup"><span data-stu-id="5eaef-108">Property</span></span>|<span data-ttu-id="5eaef-109">类型</span><span class="sxs-lookup"><span data-stu-id="5eaef-109">Type</span></span>|<span data-ttu-id="5eaef-110">Description</span><span class="sxs-lookup"><span data-stu-id="5eaef-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5eaef-111">allowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="5eaef-111">allowedResourceActions</span></span>|<span data-ttu-id="5eaef-112">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5eaef-112">String collection</span></span>|<span data-ttu-id="5eaef-113">允许的操作</span><span class="sxs-lookup"><span data-stu-id="5eaef-113">Allowed Actions</span></span>|
|<span data-ttu-id="5eaef-114">notAllowedResourceActions</span><span class="sxs-lookup"><span data-stu-id="5eaef-114">notAllowedResourceActions</span></span>|<span data-ttu-id="5eaef-115">字符串集合</span><span class="sxs-lookup"><span data-stu-id="5eaef-115">String collection</span></span>|<span data-ttu-id="5eaef-116">不允许的操作。</span><span class="sxs-lookup"><span data-stu-id="5eaef-116">Not Allowed Actions.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5eaef-117">关系</span><span class="sxs-lookup"><span data-stu-id="5eaef-117">Relationships</span></span>
<span data-ttu-id="5eaef-118">无</span><span class="sxs-lookup"><span data-stu-id="5eaef-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5eaef-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5eaef-119">JSON Representation</span></span>
<span data-ttu-id="5eaef-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5eaef-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.resourceAction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.resourceAction",
  "allowedResourceActions": [
    "String"
  ],
  "notAllowedResourceActions": [
    "String"
  ]
}
```




