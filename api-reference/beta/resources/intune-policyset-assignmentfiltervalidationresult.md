---
title: assignmentFilterValidationResult 资源类型
description: 表示验证 API 的结果。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a540bdec4265c544f565e560b6858755d0076178
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160520"
---
# <a name="assignmentfiltervalidationresult-resource-type"></a><span data-ttu-id="15ddc-103">assignmentFilterValidationResult 资源类型</span><span class="sxs-lookup"><span data-stu-id="15ddc-103">assignmentFilterValidationResult resource type</span></span>

<span data-ttu-id="15ddc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15ddc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="15ddc-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="15ddc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="15ddc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="15ddc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="15ddc-107">表示验证 API 的结果。</span><span class="sxs-lookup"><span data-stu-id="15ddc-107">Represents result of Validation API.</span></span>

## <a name="properties"></a><span data-ttu-id="15ddc-108">属性</span><span class="sxs-lookup"><span data-stu-id="15ddc-108">Properties</span></span>
|<span data-ttu-id="15ddc-109">属性</span><span class="sxs-lookup"><span data-stu-id="15ddc-109">Property</span></span>|<span data-ttu-id="15ddc-110">类型</span><span class="sxs-lookup"><span data-stu-id="15ddc-110">Type</span></span>|<span data-ttu-id="15ddc-111">说明</span><span class="sxs-lookup"><span data-stu-id="15ddc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15ddc-112">isValidRule</span><span class="sxs-lookup"><span data-stu-id="15ddc-112">isValidRule</span></span>|<span data-ttu-id="15ddc-113">布尔</span><span class="sxs-lookup"><span data-stu-id="15ddc-113">Boolean</span></span>|<span data-ttu-id="15ddc-114">有效规则或无效规则的指示器。</span><span class="sxs-lookup"><span data-stu-id="15ddc-114">Indicator to valid or invalid rule.</span></span>|

## <a name="relationships"></a><span data-ttu-id="15ddc-115">关系</span><span class="sxs-lookup"><span data-stu-id="15ddc-115">Relationships</span></span>
<span data-ttu-id="15ddc-116">无</span><span class="sxs-lookup"><span data-stu-id="15ddc-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="15ddc-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="15ddc-117">JSON Representation</span></span>
<span data-ttu-id="15ddc-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="15ddc-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.assignmentFilterValidationResult"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.assignmentFilterValidationResult",
  "isValidRule": true
}
```




