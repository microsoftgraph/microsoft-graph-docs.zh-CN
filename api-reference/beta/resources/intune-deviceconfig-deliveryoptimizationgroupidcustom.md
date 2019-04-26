---
title: deliveryOptimizationGroupIdCustom 资源类型
description: 自定义组 id 类型
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2d4f369c9a3b62480549f19d4a7c1d7b1d0bb196
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556163"
---
# <a name="deliveryoptimizationgroupidcustom-resource-type"></a><span data-ttu-id="19217-103">deliveryOptimizationGroupIdCustom 资源类型</span><span class="sxs-lookup"><span data-stu-id="19217-103">deliveryOptimizationGroupIdCustom resource type</span></span>

> <span data-ttu-id="19217-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="19217-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="19217-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19217-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19217-106">自定义组 id 类型</span><span class="sxs-lookup"><span data-stu-id="19217-106">Custom group id type</span></span>


<span data-ttu-id="19217-107">继承自[deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span><span class="sxs-lookup"><span data-stu-id="19217-107">Inherits from [deliveryOptimizationGroupIdSource](../resources/intune-deviceconfig-deliveryoptimizationgroupidsource.md)</span></span>

## <a name="properties"></a><span data-ttu-id="19217-108">属性</span><span class="sxs-lookup"><span data-stu-id="19217-108">Properties</span></span>
|<span data-ttu-id="19217-109">属性</span><span class="sxs-lookup"><span data-stu-id="19217-109">Property</span></span>|<span data-ttu-id="19217-110">类型</span><span class="sxs-lookup"><span data-stu-id="19217-110">Type</span></span>|<span data-ttu-id="19217-111">说明</span><span class="sxs-lookup"><span data-stu-id="19217-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19217-112">groupIdCustom</span><span class="sxs-lookup"><span data-stu-id="19217-112">groupIdCustom</span></span>|<span data-ttu-id="19217-113">String</span><span class="sxs-lookup"><span data-stu-id="19217-113">String</span></span>|<span data-ttu-id="19217-114">指定设备所属的任意组 ID</span><span class="sxs-lookup"><span data-stu-id="19217-114">Specifies an arbitrary group ID that the device belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="19217-115">关系</span><span class="sxs-lookup"><span data-stu-id="19217-115">Relationships</span></span>
<span data-ttu-id="19217-116">无</span><span class="sxs-lookup"><span data-stu-id="19217-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="19217-117">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="19217-117">JSON Representation</span></span>
<span data-ttu-id="19217-118">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19217-118">Here is a JSON representation of the resource.</span></span>
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





