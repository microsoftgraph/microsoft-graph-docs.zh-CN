---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e49aa085eb0cf23384bbed739235df46e5da1f72
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47978172"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="13a2c-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="13a2c-103">omaSetting resource type</span></span>

<span data-ttu-id="13a2c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="13a2c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="13a2c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="13a2c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="13a2c-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="13a2c-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="13a2c-107">属性</span><span class="sxs-lookup"><span data-stu-id="13a2c-107">Properties</span></span>
|<span data-ttu-id="13a2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="13a2c-108">Property</span></span>|<span data-ttu-id="13a2c-109">类型</span><span class="sxs-lookup"><span data-stu-id="13a2c-109">Type</span></span>|<span data-ttu-id="13a2c-110">说明</span><span class="sxs-lookup"><span data-stu-id="13a2c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="13a2c-111">displayName</span><span class="sxs-lookup"><span data-stu-id="13a2c-111">displayName</span></span>|<span data-ttu-id="13a2c-112">String</span><span class="sxs-lookup"><span data-stu-id="13a2c-112">String</span></span>|<span data-ttu-id="13a2c-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="13a2c-113">Display Name.</span></span>|
|<span data-ttu-id="13a2c-114">description</span><span class="sxs-lookup"><span data-stu-id="13a2c-114">description</span></span>|<span data-ttu-id="13a2c-115">String</span><span class="sxs-lookup"><span data-stu-id="13a2c-115">String</span></span>|<span data-ttu-id="13a2c-116">说明。</span><span class="sxs-lookup"><span data-stu-id="13a2c-116">Description.</span></span>|
|<span data-ttu-id="13a2c-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="13a2c-117">omaUri</span></span>|<span data-ttu-id="13a2c-118">String</span><span class="sxs-lookup"><span data-stu-id="13a2c-118">String</span></span>|<span data-ttu-id="13a2c-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="13a2c-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="13a2c-120">关系</span><span class="sxs-lookup"><span data-stu-id="13a2c-120">Relationships</span></span>
<span data-ttu-id="13a2c-121">无</span><span class="sxs-lookup"><span data-stu-id="13a2c-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="13a2c-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="13a2c-122">JSON Representation</span></span>
<span data-ttu-id="13a2c-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="13a2c-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.omaSetting"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.omaSetting",
  "displayName": "String",
  "description": "String",
  "omaUri": "String"
}
```









