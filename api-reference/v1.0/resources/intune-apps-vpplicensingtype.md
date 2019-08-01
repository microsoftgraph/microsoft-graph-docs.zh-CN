---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 831961fd9e04bff577fe986a2e6309d1cdfbcca0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032128"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="cf849-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="cf849-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="cf849-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cf849-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf849-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="cf849-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="cf849-106">属性</span><span class="sxs-lookup"><span data-stu-id="cf849-106">Properties</span></span>
|<span data-ttu-id="cf849-107">属性</span><span class="sxs-lookup"><span data-stu-id="cf849-107">Property</span></span>|<span data-ttu-id="cf849-108">类型</span><span class="sxs-lookup"><span data-stu-id="cf849-108">Type</span></span>|<span data-ttu-id="cf849-109">说明</span><span class="sxs-lookup"><span data-stu-id="cf849-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf849-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="cf849-110">supportsUserLicensing</span></span>|<span data-ttu-id="cf849-111">Boolean</span><span class="sxs-lookup"><span data-stu-id="cf849-111">Boolean</span></span>|<span data-ttu-id="cf849-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="cf849-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="cf849-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="cf849-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="cf849-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="cf849-114">Boolean</span></span>|<span data-ttu-id="cf849-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="cf849-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf849-116">关系</span><span class="sxs-lookup"><span data-stu-id="cf849-116">Relationships</span></span>
<span data-ttu-id="cf849-117">无</span><span class="sxs-lookup"><span data-stu-id="cf849-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf849-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cf849-118">JSON Representation</span></span>
<span data-ttu-id="cf849-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cf849-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vppLicensingType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vppLicensingType",
  "supportsUserLicensing": true,
  "supportsDeviceLicensing": true
}
```



