---
title: numberRange 资源类型
description: 号码范围定义。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 6c9c3b4f286bb9c3fa68beb24dd395e28d9633d4
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49273233"
---
# <a name="numberrange-resource-type"></a><span data-ttu-id="f6c6d-103">numberRange 资源类型</span><span class="sxs-lookup"><span data-stu-id="f6c6d-103">numberRange resource type</span></span>

<span data-ttu-id="f6c6d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f6c6d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f6c6d-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f6c6d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f6c6d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f6c6d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f6c6d-107">号码范围定义。</span><span class="sxs-lookup"><span data-stu-id="f6c6d-107">Number Range definition.</span></span>

## <a name="properties"></a><span data-ttu-id="f6c6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6c6d-108">Properties</span></span>
|<span data-ttu-id="f6c6d-109">属性</span><span class="sxs-lookup"><span data-stu-id="f6c6d-109">Property</span></span>|<span data-ttu-id="f6c6d-110">类型</span><span class="sxs-lookup"><span data-stu-id="f6c6d-110">Type</span></span>|<span data-ttu-id="f6c6d-111">说明</span><span class="sxs-lookup"><span data-stu-id="f6c6d-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f6c6d-112">lowerNumber</span><span class="sxs-lookup"><span data-stu-id="f6c6d-112">lowerNumber</span></span>|<span data-ttu-id="f6c6d-113">Int32</span><span class="sxs-lookup"><span data-stu-id="f6c6d-113">Int32</span></span>|<span data-ttu-id="f6c6d-114">较小的数字。</span><span class="sxs-lookup"><span data-stu-id="f6c6d-114">Lower number.</span></span>|
|<span data-ttu-id="f6c6d-115">upperNumber</span><span class="sxs-lookup"><span data-stu-id="f6c6d-115">upperNumber</span></span>|<span data-ttu-id="f6c6d-116">Int32</span><span class="sxs-lookup"><span data-stu-id="f6c6d-116">Int32</span></span>|<span data-ttu-id="f6c6d-117">上限数。</span><span class="sxs-lookup"><span data-stu-id="f6c6d-117">Upper number.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f6c6d-118">关系</span><span class="sxs-lookup"><span data-stu-id="f6c6d-118">Relationships</span></span>
<span data-ttu-id="f6c6d-119">无</span><span class="sxs-lookup"><span data-stu-id="f6c6d-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="f6c6d-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f6c6d-120">JSON Representation</span></span>
<span data-ttu-id="f6c6d-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f6c6d-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.numberRange"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.numberRange",
  "lowerNumber": 1024,
  "upperNumber": 1024
}
```




