---
title: deviceManagementEnumValue 资源类型
description: 枚举值的定义信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 016c20153d7e4d9e970d5c10038aad4616a8e952
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943456"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="49620-103">deviceManagementEnumValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="49620-103">deviceManagementEnumValue resource type</span></span>

> <span data-ttu-id="49620-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="49620-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="49620-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="49620-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="49620-106">枚举值的定义信息</span><span class="sxs-lookup"><span data-stu-id="49620-106">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="49620-107">属性</span><span class="sxs-lookup"><span data-stu-id="49620-107">Properties</span></span>
|<span data-ttu-id="49620-108">属性</span><span class="sxs-lookup"><span data-stu-id="49620-108">Property</span></span>|<span data-ttu-id="49620-109">类型</span><span class="sxs-lookup"><span data-stu-id="49620-109">Type</span></span>|<span data-ttu-id="49620-110">说明</span><span class="sxs-lookup"><span data-stu-id="49620-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="49620-111">值</span><span class="sxs-lookup"><span data-stu-id="49620-111">value</span></span>|<span data-ttu-id="49620-112">String</span><span class="sxs-lookup"><span data-stu-id="49620-112">String</span></span>|<span data-ttu-id="49620-113">原始枚举值文本</span><span class="sxs-lookup"><span data-stu-id="49620-113">The raw enum value text</span></span>|
|<span data-ttu-id="49620-114">displayName</span><span class="sxs-lookup"><span data-stu-id="49620-114">displayName</span></span>|<span data-ttu-id="49620-115">String</span><span class="sxs-lookup"><span data-stu-id="49620-115">String</span></span>|<span data-ttu-id="49620-116">此枚举值的显示名称</span><span class="sxs-lookup"><span data-stu-id="49620-116">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="49620-117">关系</span><span class="sxs-lookup"><span data-stu-id="49620-117">Relationships</span></span>
<span data-ttu-id="49620-118">无</span><span class="sxs-lookup"><span data-stu-id="49620-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="49620-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="49620-119">JSON Representation</span></span>
<span data-ttu-id="49620-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="49620-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementEnumValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementEnumValue",
  "value": "String",
  "displayName": "String"
}
```




