---
title: updateManagementEnrollment 资源类型
description: 表示通过特定更新类别的服务注册到管理中。
author: Alice-at-Microsoft
localization_priority: Normal
ms.prod: w10
doc_type: resourcePageType
ms.openlocfilehash: 1d00bc152d5fc3b7b4be267cd3ea56fab52b8b38
ms.sourcegitcommit: 1b09298649d5606b471b4cbe1055419bbe2fc7e5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2021
ms.locfileid: "52067298"
---
# <a name="updatemanagementenrollment-resource-type"></a><span data-ttu-id="04fb3-103">updateManagementEnrollment 资源类型</span><span class="sxs-lookup"><span data-stu-id="04fb3-103">updateManagementEnrollment resource type</span></span>

<span data-ttu-id="04fb3-104">命名空间：microsoft.graph.windowsUpdates</span><span class="sxs-lookup"><span data-stu-id="04fb3-104">Namespace: microsoft.graph.windowsUpdates</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="04fb3-105">表示通过特定更新类别的服务注册到管理中。</span><span class="sxs-lookup"><span data-stu-id="04fb3-105">Represents enrollment into management by the service of a certain update category.</span></span>

<span data-ttu-id="04fb3-106">继承自 [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md)。</span><span class="sxs-lookup"><span data-stu-id="04fb3-106">Inherits from [updatableAssetEnrollment](../resources/windowsupdates-updatableassetenrollment.md).</span></span>

## <a name="properties"></a><span data-ttu-id="04fb3-107">属性</span><span class="sxs-lookup"><span data-stu-id="04fb3-107">Properties</span></span>
|<span data-ttu-id="04fb3-108">属性</span><span class="sxs-lookup"><span data-stu-id="04fb3-108">Property</span></span>|<span data-ttu-id="04fb3-109">类型</span><span class="sxs-lookup"><span data-stu-id="04fb3-109">Type</span></span>|<span data-ttu-id="04fb3-110">说明</span><span class="sxs-lookup"><span data-stu-id="04fb3-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="04fb3-111">updateCategory</span><span class="sxs-lookup"><span data-stu-id="04fb3-111">updateCategory</span></span>|<span data-ttu-id="04fb3-112">microsoft.graph.windowsUpdates.updateCategory</span><span class="sxs-lookup"><span data-stu-id="04fb3-112">microsoft.graph.windowsUpdates.updateCategory</span></span>|<span data-ttu-id="04fb3-113">服务管理的更新类别。</span><span class="sxs-lookup"><span data-stu-id="04fb3-113">The category of updates that the service manages.</span></span> <span data-ttu-id="04fb3-114">支持 **updateCategory** 值的子集。</span><span class="sxs-lookup"><span data-stu-id="04fb3-114">Supports a subset of the values for **updateCategory**.</span></span> <span data-ttu-id="04fb3-115">可能的值是 `feature` ：。</span><span class="sxs-lookup"><span data-stu-id="04fb3-115">Possible values are: `feature`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="04fb3-116">关系</span><span class="sxs-lookup"><span data-stu-id="04fb3-116">Relationships</span></span>
<span data-ttu-id="04fb3-117">无。</span><span class="sxs-lookup"><span data-stu-id="04fb3-117">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="04fb3-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="04fb3-118">JSON representation</span></span>
<span data-ttu-id="04fb3-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="04fb3-119">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdates.updateManagementEnrollment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdates.updateManagementEnrollment",
  "updateCategory": "String"
}
```

