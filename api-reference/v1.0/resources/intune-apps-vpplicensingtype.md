---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 34314ee04dacbc422b2a9b09e8f6802d308c3d69
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27971471"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="5daf4-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="5daf4-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="5daf4-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5daf4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5daf4-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="5daf4-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="5daf4-106">属性</span><span class="sxs-lookup"><span data-stu-id="5daf4-106">Properties</span></span>
|<span data-ttu-id="5daf4-107">属性</span><span class="sxs-lookup"><span data-stu-id="5daf4-107">Property</span></span>|<span data-ttu-id="5daf4-108">类型</span><span class="sxs-lookup"><span data-stu-id="5daf4-108">Type</span></span>|<span data-ttu-id="5daf4-109">说明</span><span class="sxs-lookup"><span data-stu-id="5daf4-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5daf4-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="5daf4-110">supportsUserLicensing</span></span>|<span data-ttu-id="5daf4-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="5daf4-111">Boolean</span></span>|<span data-ttu-id="5daf4-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="5daf4-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="5daf4-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="5daf4-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="5daf4-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="5daf4-114">Boolean</span></span>|<span data-ttu-id="5daf4-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="5daf4-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5daf4-116">关系</span><span class="sxs-lookup"><span data-stu-id="5daf4-116">Relationships</span></span>
<span data-ttu-id="5daf4-117">无</span><span class="sxs-lookup"><span data-stu-id="5daf4-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5daf4-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="5daf4-118">JSON Representation</span></span>
<span data-ttu-id="5daf4-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5daf4-119">Here is a JSON representation of the resource.</span></span>
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



