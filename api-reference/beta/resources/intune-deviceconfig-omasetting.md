---
title: omaSetting 资源类型
description: OMA 设置定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bdc653c07ad7553e9358703037c15179d9366dad
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722990"
---
# <a name="omasetting-resource-type"></a><span data-ttu-id="a2ca3-103">omaSetting 资源类型</span><span class="sxs-lookup"><span data-stu-id="a2ca3-103">omaSetting resource type</span></span>

<span data-ttu-id="a2ca3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a2ca3-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a2ca3-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a2ca3-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ca3-107">OMA 设置定义。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-107">OMA Settings definition.</span></span>

## <a name="properties"></a><span data-ttu-id="a2ca3-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2ca3-108">Properties</span></span>
|<span data-ttu-id="a2ca3-109">属性</span><span class="sxs-lookup"><span data-stu-id="a2ca3-109">Property</span></span>|<span data-ttu-id="a2ca3-110">类型</span><span class="sxs-lookup"><span data-stu-id="a2ca3-110">Type</span></span>|<span data-ttu-id="a2ca3-111">说明</span><span class="sxs-lookup"><span data-stu-id="a2ca3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ca3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="a2ca3-112">displayName</span></span>|<span data-ttu-id="a2ca3-113">String</span><span class="sxs-lookup"><span data-stu-id="a2ca3-113">String</span></span>|<span data-ttu-id="a2ca3-114">显示名称。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-114">Display Name.</span></span>|
|<span data-ttu-id="a2ca3-115">说明</span><span class="sxs-lookup"><span data-stu-id="a2ca3-115">description</span></span>|<span data-ttu-id="a2ca3-116">String</span><span class="sxs-lookup"><span data-stu-id="a2ca3-116">String</span></span>|<span data-ttu-id="a2ca3-117">说明。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-117">Description.</span></span>|
|<span data-ttu-id="a2ca3-118">omaUri</span><span class="sxs-lookup"><span data-stu-id="a2ca3-118">omaUri</span></span>|<span data-ttu-id="a2ca3-119">String</span><span class="sxs-lookup"><span data-stu-id="a2ca3-119">String</span></span>|<span data-ttu-id="a2ca3-120">OMA。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-120">OMA.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a2ca3-121">关系</span><span class="sxs-lookup"><span data-stu-id="a2ca3-121">Relationships</span></span>
<span data-ttu-id="a2ca3-122">无</span><span class="sxs-lookup"><span data-stu-id="a2ca3-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a2ca3-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a2ca3-123">JSON Representation</span></span>
<span data-ttu-id="a2ca3-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2ca3-124">Here is a JSON representation of the resource.</span></span>
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





