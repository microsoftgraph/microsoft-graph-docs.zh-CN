---
title: 键值资源类型
description: 项值定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e0d112c76e03f45ba7bf28fea3b6d219745c4332
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49283216"
---
# <a name="keyvalue-resource-type"></a><span data-ttu-id="2bf3d-103">键值资源类型</span><span class="sxs-lookup"><span data-stu-id="2bf3d-103">keyValue resource type</span></span>

<span data-ttu-id="2bf3d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2bf3d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2bf3d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2bf3d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bf3d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2bf3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bf3d-107">项值定义。</span><span class="sxs-lookup"><span data-stu-id="2bf3d-107">Key Value definition.</span></span>

## <a name="properties"></a><span data-ttu-id="2bf3d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2bf3d-108">Properties</span></span>
|<span data-ttu-id="2bf3d-109">属性</span><span class="sxs-lookup"><span data-stu-id="2bf3d-109">Property</span></span>|<span data-ttu-id="2bf3d-110">类型</span><span class="sxs-lookup"><span data-stu-id="2bf3d-110">Type</span></span>|<span data-ttu-id="2bf3d-111">Description</span><span class="sxs-lookup"><span data-stu-id="2bf3d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2bf3d-112">Key</span><span class="sxs-lookup"><span data-stu-id="2bf3d-112">key</span></span>|<span data-ttu-id="2bf3d-113">String</span><span class="sxs-lookup"><span data-stu-id="2bf3d-113">String</span></span>|<span data-ttu-id="2bf3d-114">键。</span><span class="sxs-lookup"><span data-stu-id="2bf3d-114">Key.</span></span>|
|<span data-ttu-id="2bf3d-115">value</span><span class="sxs-lookup"><span data-stu-id="2bf3d-115">value</span></span>|<span data-ttu-id="2bf3d-116">String</span><span class="sxs-lookup"><span data-stu-id="2bf3d-116">String</span></span>|<span data-ttu-id="2bf3d-117">值。</span><span class="sxs-lookup"><span data-stu-id="2bf3d-117">Value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2bf3d-118">关系</span><span class="sxs-lookup"><span data-stu-id="2bf3d-118">Relationships</span></span>
<span data-ttu-id="2bf3d-119">无</span><span class="sxs-lookup"><span data-stu-id="2bf3d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2bf3d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bf3d-120">JSON Representation</span></span>
<span data-ttu-id="2bf3d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bf3d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.keyValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.keyValue",
  "key": "String",
  "value": "String"
}
```




