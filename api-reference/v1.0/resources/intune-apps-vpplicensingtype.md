---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 73b46c9bcd8680ffbd78c1cfc85cc6dec85126e6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557927"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="377eb-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="377eb-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="377eb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="377eb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="377eb-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="377eb-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="377eb-106">属性</span><span class="sxs-lookup"><span data-stu-id="377eb-106">Properties</span></span>
|<span data-ttu-id="377eb-107">属性</span><span class="sxs-lookup"><span data-stu-id="377eb-107">Property</span></span>|<span data-ttu-id="377eb-108">类型</span><span class="sxs-lookup"><span data-stu-id="377eb-108">Type</span></span>|<span data-ttu-id="377eb-109">说明</span><span class="sxs-lookup"><span data-stu-id="377eb-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="377eb-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="377eb-110">supportsUserLicensing</span></span>|<span data-ttu-id="377eb-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="377eb-111">Boolean</span></span>|<span data-ttu-id="377eb-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="377eb-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="377eb-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="377eb-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="377eb-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="377eb-114">Boolean</span></span>|<span data-ttu-id="377eb-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="377eb-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="377eb-116">关系</span><span class="sxs-lookup"><span data-stu-id="377eb-116">Relationships</span></span>
<span data-ttu-id="377eb-117">无</span><span class="sxs-lookup"><span data-stu-id="377eb-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="377eb-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="377eb-118">JSON Representation</span></span>
<span data-ttu-id="377eb-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="377eb-119">Here is a JSON representation of the resource.</span></span>
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



