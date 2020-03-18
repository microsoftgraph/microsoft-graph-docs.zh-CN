---
title: deviceManagementEnumValue 资源类型
description: 枚举值的定义信息
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 71fe0886c0e51e52c4ca5bad615f6e80aef99175
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42785454"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="697d4-103">deviceManagementEnumValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="697d4-103">deviceManagementEnumValue resource type</span></span>

> <span data-ttu-id="697d4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="697d4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="697d4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="697d4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="697d4-106">枚举值的定义信息</span><span class="sxs-lookup"><span data-stu-id="697d4-106">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="697d4-107">属性</span><span class="sxs-lookup"><span data-stu-id="697d4-107">Properties</span></span>
|<span data-ttu-id="697d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="697d4-108">Property</span></span>|<span data-ttu-id="697d4-109">类型</span><span class="sxs-lookup"><span data-stu-id="697d4-109">Type</span></span>|<span data-ttu-id="697d4-110">说明</span><span class="sxs-lookup"><span data-stu-id="697d4-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="697d4-111">值</span><span class="sxs-lookup"><span data-stu-id="697d4-111">value</span></span>|<span data-ttu-id="697d4-112">String</span><span class="sxs-lookup"><span data-stu-id="697d4-112">String</span></span>|<span data-ttu-id="697d4-113">原始枚举值文本</span><span class="sxs-lookup"><span data-stu-id="697d4-113">The raw enum value text</span></span>|
|<span data-ttu-id="697d4-114">displayName</span><span class="sxs-lookup"><span data-stu-id="697d4-114">displayName</span></span>|<span data-ttu-id="697d4-115">String</span><span class="sxs-lookup"><span data-stu-id="697d4-115">String</span></span>|<span data-ttu-id="697d4-116">此枚举值的显示名称</span><span class="sxs-lookup"><span data-stu-id="697d4-116">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="697d4-117">关系</span><span class="sxs-lookup"><span data-stu-id="697d4-117">Relationships</span></span>
<span data-ttu-id="697d4-118">无</span><span class="sxs-lookup"><span data-stu-id="697d4-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="697d4-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="697d4-119">JSON Representation</span></span>
<span data-ttu-id="697d4-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="697d4-120">Here is a JSON representation of the resource.</span></span>
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



