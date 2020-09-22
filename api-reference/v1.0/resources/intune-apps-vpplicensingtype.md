---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c7dbaded456e4f4df9874635a27b7f46d0ca7a2c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094300"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="56413-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="56413-103">vppLicensingType resource type</span></span>

<span data-ttu-id="56413-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="56413-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="56413-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="56413-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="56413-106">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="56413-106">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>

## <a name="properties"></a><span data-ttu-id="56413-107">属性</span><span class="sxs-lookup"><span data-stu-id="56413-107">Properties</span></span>
|<span data-ttu-id="56413-108">属性</span><span class="sxs-lookup"><span data-stu-id="56413-108">Property</span></span>|<span data-ttu-id="56413-109">类型</span><span class="sxs-lookup"><span data-stu-id="56413-109">Type</span></span>|<span data-ttu-id="56413-110">说明</span><span class="sxs-lookup"><span data-stu-id="56413-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56413-111">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="56413-111">supportsUserLicensing</span></span>|<span data-ttu-id="56413-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="56413-112">Boolean</span></span>|<span data-ttu-id="56413-113">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="56413-113">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="56413-114">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="56413-114">supportsDeviceLicensing</span></span>|<span data-ttu-id="56413-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="56413-115">Boolean</span></span>|<span data-ttu-id="56413-116">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="56413-116">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="56413-117">关系</span><span class="sxs-lookup"><span data-stu-id="56413-117">Relationships</span></span>
<span data-ttu-id="56413-118">无</span><span class="sxs-lookup"><span data-stu-id="56413-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="56413-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56413-119">JSON Representation</span></span>
<span data-ttu-id="56413-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56413-120">Here is a JSON representation of the resource.</span></span>
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









