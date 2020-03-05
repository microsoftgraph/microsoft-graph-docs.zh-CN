---
title: deliveryOptimizationGroupIdCustom 资源类型
description: 自定义组 id 类型
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 4f19576203d720eeb35c4268e6ea4f28c968c969
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42526790"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="7e66d-103">deliveryOptimizationGroupIdCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e66d-103">deliveryOptimizationGroupIdCustom resource type</span></span>

<span data-ttu-id="7e66d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="7e66d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7e66d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7e66d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e66d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7e66d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e66d-107">自定义组 id 类型</span><span class="sxs-lookup"><span data-stu-id="7e66d-107">Custom group id type</span></span>


<span data-ttu-id="7e66d-108">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="7e66d-108">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="7e66d-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e66d-109">Properties</span></span>
|<span data-ttu-id="7e66d-110">属性</span><span class="sxs-lookup"><span data-stu-id="7e66d-110">Property</span></span>|<span data-ttu-id="7e66d-111">类型</span><span class="sxs-lookup"><span data-stu-id="7e66d-111">Type</span></span>|<span data-ttu-id="7e66d-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e66d-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7e66d-113">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="7e66d-113">groupIdCustom</span></span>|<span data-ttu-id="7e66d-114">String</span><span class="sxs-lookup"><span data-stu-id="7e66d-114">String</span></span>|<span data-ttu-id="7e66d-115">指定设备所属的任意组 ID</span><span class="sxs-lookup"><span data-stu-id="7e66d-115">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="7e66d-116">关系</span><span class="sxs-lookup"><span data-stu-id="7e66d-116">Relationships</span></span>
<span data-ttu-id="7e66d-117">无</span><span class="sxs-lookup"><span data-stu-id="7e66d-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="7e66d-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e66d-118">JSON Representation</span></span>
<span data-ttu-id="7e66d-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e66d-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deliveryOptimizationGroupIdCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deliveryOptimizationGroupIdCustom",
  "groupIdCustom": "String"
}
```



