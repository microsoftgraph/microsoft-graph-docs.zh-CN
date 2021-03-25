---
title: assignmentFilterState 资源类型
description: 表示 GetState API 的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 969d902635962a9ff89bb197f32e7d995dd9b35f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51159376"
---
# <a name="assignmentfilterstate-resource-type"></a><span data-ttu-id="72a8c-103">assignmentFilterState 资源类型</span><span class="sxs-lookup"><span data-stu-id="72a8c-103">assignmentFilterState resource type</span></span>

<span data-ttu-id="72a8c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72a8c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72a8c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="72a8c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="72a8c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72a8c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72a8c-107">表示 GetState API 的结果。</span><span class="sxs-lookup"><span data-stu-id="72a8c-107">Represents result of GetState API.</span></span>

## <a name="properties"></a><span data-ttu-id="72a8c-108">属性</span><span class="sxs-lookup"><span data-stu-id="72a8c-108">Properties</span></span>
|<span data-ttu-id="72a8c-109">属性</span><span class="sxs-lookup"><span data-stu-id="72a8c-109">Property</span></span>|<span data-ttu-id="72a8c-110">类型</span><span class="sxs-lookup"><span data-stu-id="72a8c-110">Type</span></span>|<span data-ttu-id="72a8c-111">说明</span><span class="sxs-lookup"><span data-stu-id="72a8c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72a8c-112">已启用</span><span class="sxs-lookup"><span data-stu-id="72a8c-112">enabled</span></span>|<span data-ttu-id="72a8c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="72a8c-113">Boolean</span></span>|<span data-ttu-id="72a8c-114">指示 AssignmentFilter 是启用还是禁用的指示器。</span><span class="sxs-lookup"><span data-stu-id="72a8c-114">Indicator to if AssignmentFilter is enabled or disabled.</span></span>|

## <a name="relationships"></a><span data-ttu-id="72a8c-115">关系</span><span class="sxs-lookup"><span data-stu-id="72a8c-115">Relationships</span></span>
<span data-ttu-id="72a8c-116">无</span><span class="sxs-lookup"><span data-stu-id="72a8c-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="72a8c-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="72a8c-117">JSON Representation</span></span>
<span data-ttu-id="72a8c-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72a8c-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterState",
  "enabled": true
}
```




