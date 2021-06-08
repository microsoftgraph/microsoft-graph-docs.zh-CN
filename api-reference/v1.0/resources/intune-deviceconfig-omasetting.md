---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 34137caf93bcdd3a3621842b9976e964b8f44c78
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759992"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="77478-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="77478-103">omaSetting resource type</span></span>

<span data-ttu-id="77478-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="77478-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="77478-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77478-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77478-106">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="77478-106">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="77478-107">属性</span><span class="sxs-lookup"><span data-stu-id="77478-107">Properties</span></span>
|<span data-ttu-id="77478-108">属性</span><span class="sxs-lookup"><span data-stu-id="77478-108">Property</span></span>|<span data-ttu-id="77478-109">类型</span><span class="sxs-lookup"><span data-stu-id="77478-109">Type</span></span>|<span data-ttu-id="77478-110">说明</span><span class="sxs-lookup"><span data-stu-id="77478-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="77478-111">displayName</span><span class="sxs-lookup"><span data-stu-id="77478-111">displayName</span></span>|<span data-ttu-id="77478-112">String</span><span class="sxs-lookup"><span data-stu-id="77478-112">String</span></span>|<span data-ttu-id="77478-113">显示名称。</span><span class="sxs-lookup"><span data-stu-id="77478-113">Display Name.</span></span>|
|<span data-ttu-id="77478-114">description</span><span class="sxs-lookup"><span data-stu-id="77478-114">description</span></span>|<span data-ttu-id="77478-115">String</span><span class="sxs-lookup"><span data-stu-id="77478-115">String</span></span>|<span data-ttu-id="77478-116">说明。</span><span class="sxs-lookup"><span data-stu-id="77478-116">Description.</span></span>|
|<span data-ttu-id="77478-117">omaUri</span><span class="sxs-lookup"><span data-stu-id="77478-117">omaUri</span></span>|<span data-ttu-id="77478-118">String</span><span class="sxs-lookup"><span data-stu-id="77478-118">String</span></span>|<span data-ttu-id="77478-119">OMA。</span><span class="sxs-lookup"><span data-stu-id="77478-119">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="77478-120">关系</span><span class="sxs-lookup"><span data-stu-id="77478-120">Relationships</span></span>
<span data-ttu-id="77478-121">无</span><span class="sxs-lookup"><span data-stu-id="77478-121">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="77478-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="77478-122">JSON Representation</span></span>
<span data-ttu-id="77478-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="77478-123">Here is a JSON representation of the resource.</span></span>
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




