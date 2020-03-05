---
title: deviceManagementEnumValue 资源类型
description: 枚举值的定义信息
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8400aa7228fbc04e52a66074380f302f02e66823
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528857"
---
# <a name="devicemanagementenumvalue-resource-type"></a><span data-ttu-id="0d764-103">deviceManagementEnumValue 资源类型</span><span class="sxs-lookup"><span data-stu-id="0d764-103">deviceManagementEnumValue resource type</span></span>

<span data-ttu-id="0d764-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0d764-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0d764-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0d764-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0d764-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0d764-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0d764-107">枚举值的定义信息</span><span class="sxs-lookup"><span data-stu-id="0d764-107">Definition information for an enum value</span></span>

## <a name="properties"></a><span data-ttu-id="0d764-108">属性</span><span class="sxs-lookup"><span data-stu-id="0d764-108">Properties</span></span>
|<span data-ttu-id="0d764-109">属性</span><span class="sxs-lookup"><span data-stu-id="0d764-109">Property</span></span>|<span data-ttu-id="0d764-110">类型</span><span class="sxs-lookup"><span data-stu-id="0d764-110">Type</span></span>|<span data-ttu-id="0d764-111">说明</span><span class="sxs-lookup"><span data-stu-id="0d764-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0d764-112">值</span><span class="sxs-lookup"><span data-stu-id="0d764-112">value</span></span>|<span data-ttu-id="0d764-113">String</span><span class="sxs-lookup"><span data-stu-id="0d764-113">String</span></span>|<span data-ttu-id="0d764-114">原始枚举值文本</span><span class="sxs-lookup"><span data-stu-id="0d764-114">The raw enum value text</span></span>|
|<span data-ttu-id="0d764-115">displayName</span><span class="sxs-lookup"><span data-stu-id="0d764-115">displayName</span></span>|<span data-ttu-id="0d764-116">String</span><span class="sxs-lookup"><span data-stu-id="0d764-116">String</span></span>|<span data-ttu-id="0d764-117">此枚举值的显示名称</span><span class="sxs-lookup"><span data-stu-id="0d764-117">Display name for this enum value</span></span>|

## <a name="relationships"></a><span data-ttu-id="0d764-118">关系</span><span class="sxs-lookup"><span data-stu-id="0d764-118">Relationships</span></span>
<span data-ttu-id="0d764-119">无</span><span class="sxs-lookup"><span data-stu-id="0d764-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0d764-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0d764-120">JSON Representation</span></span>
<span data-ttu-id="0d764-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0d764-121">Here is a JSON representation of the resource.</span></span>
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



