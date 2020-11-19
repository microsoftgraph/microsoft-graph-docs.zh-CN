---
title: deviceManagementEnumValue 资源类型
description: 枚举值的定义信息
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 86a97937872bd46e2fd71c781e90ba607f5baf9d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49275914"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="5f948-103">deviceManagementEnumValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="5f948-103">deviceManagementEnumValue resource type</span></span>

<span data-ttu-id="5f948-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5f948-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5f948-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5f948-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5f948-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f948-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f948-107">枚举值的定义信息</span><span class="sxs-lookup"><span data-stu-id="5f948-107">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="5f948-108">属性</span><span class="sxs-lookup"><span data-stu-id="5f948-108">Properties</span></span>
|<span data-ttu-id="5f948-109">属性</span><span class="sxs-lookup"><span data-stu-id="5f948-109">Property</span></span>|<span data-ttu-id="5f948-110">类型</span><span class="sxs-lookup"><span data-stu-id="5f948-110">Type</span></span>|<span data-ttu-id="5f948-111">说明</span><span class="sxs-lookup"><span data-stu-id="5f948-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f948-112">值</span><span class="sxs-lookup"><span data-stu-id="5f948-112">value</span></span>|<span data-ttu-id="5f948-113">String</span><span class="sxs-lookup"><span data-stu-id="5f948-113">String</span></span>|<span data-ttu-id="5f948-114">原始枚举值文本</span><span class="sxs-lookup"><span data-stu-id="5f948-114">The raw enum value text</span></span>|
|<span data-ttu-id="5f948-115">displayName</span><span class="sxs-lookup"><span data-stu-id="5f948-115">displayName</span></span>|<span data-ttu-id="5f948-116">字符串</span><span class="sxs-lookup"><span data-stu-id="5f948-116">String</span></span>|<span data-ttu-id="5f948-117">此枚举值的显示名称</span><span class="sxs-lookup"><span data-stu-id="5f948-117">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="5f948-118">关系</span><span class="sxs-lookup"><span data-stu-id="5f948-118">Relationships</span></span>
<span data-ttu-id="5f948-119">无</span><span class="sxs-lookup"><span data-stu-id="5f948-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5f948-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5f948-120">JSON Representation</span></span>
<span data-ttu-id="5f948-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5f948-121">Here is a JSON representation of the resource.</span></span>
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




