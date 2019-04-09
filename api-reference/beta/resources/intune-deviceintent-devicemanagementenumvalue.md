---
title: deviceManagementEnumValue 资源类型
description: 枚举值的定义信息
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: de1340223d45361825b2b8d8fc4e57194437f6b6
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523733"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="58fd1-103">deviceManagementEnumValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="58fd1-103">deviceManagementEnumValue resource type</span></span>

> <span data-ttu-id="58fd1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="58fd1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="58fd1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="58fd1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58fd1-106">枚举值的定义信息</span><span class="sxs-lookup"><span data-stu-id="58fd1-106">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="58fd1-107">属性</span><span class="sxs-lookup"><span data-stu-id="58fd1-107">Properties</span></span>
|<span data-ttu-id="58fd1-108">属性</span><span class="sxs-lookup"><span data-stu-id="58fd1-108">Property</span></span>|<span data-ttu-id="58fd1-109">类型</span><span class="sxs-lookup"><span data-stu-id="58fd1-109">Type</span></span>|<span data-ttu-id="58fd1-110">说明</span><span class="sxs-lookup"><span data-stu-id="58fd1-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58fd1-111">value</span><span class="sxs-lookup"><span data-stu-id="58fd1-111">value</span></span>|<span data-ttu-id="58fd1-112">String</span><span class="sxs-lookup"><span data-stu-id="58fd1-112">String</span></span>|<span data-ttu-id="58fd1-113">原始枚举值文本</span><span class="sxs-lookup"><span data-stu-id="58fd1-113">The raw enum value text</span></span>|
|<span data-ttu-id="58fd1-114">displayName</span><span class="sxs-lookup"><span data-stu-id="58fd1-114">displayName</span></span>|<span data-ttu-id="58fd1-115">String</span><span class="sxs-lookup"><span data-stu-id="58fd1-115">String</span></span>|<span data-ttu-id="58fd1-116">此枚举值的显示名称</span><span class="sxs-lookup"><span data-stu-id="58fd1-116">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="58fd1-117">关系</span><span class="sxs-lookup"><span data-stu-id="58fd1-117">Relationships</span></span>
<span data-ttu-id="58fd1-118">无</span><span class="sxs-lookup"><span data-stu-id="58fd1-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="58fd1-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="58fd1-119">JSON Representation</span></span>
<span data-ttu-id="58fd1-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="58fd1-120">Here is a JSON representation of the resource.</span></span>
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







