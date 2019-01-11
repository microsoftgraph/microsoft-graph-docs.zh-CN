---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: bbc52cfd4e14b2010dd133e4fa08e61a30fb63df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814110"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="d9a22-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9a22-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="d9a22-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9a22-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9a22-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="d9a22-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="d9a22-106">属性</span><span class="sxs-lookup"><span data-stu-id="d9a22-106">Properties</span></span>
|<span data-ttu-id="d9a22-107">属性</span><span class="sxs-lookup"><span data-stu-id="d9a22-107">Property</span></span>|<span data-ttu-id="d9a22-108">类型</span><span class="sxs-lookup"><span data-stu-id="d9a22-108">Type</span></span>|<span data-ttu-id="d9a22-109">说明</span><span class="sxs-lookup"><span data-stu-id="d9a22-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9a22-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="d9a22-110">supportsUserLicensing</span></span>|<span data-ttu-id="d9a22-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="d9a22-111">Boolean</span></span>|<span data-ttu-id="d9a22-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="d9a22-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="d9a22-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="d9a22-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="d9a22-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="d9a22-114">Boolean</span></span>|<span data-ttu-id="d9a22-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="d9a22-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d9a22-116">关系</span><span class="sxs-lookup"><span data-stu-id="d9a22-116">Relationships</span></span>
<span data-ttu-id="d9a22-117">无</span><span class="sxs-lookup"><span data-stu-id="d9a22-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d9a22-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9a22-118">JSON Representation</span></span>
<span data-ttu-id="d9a22-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9a22-119">Here is a JSON representation of the resource.</span></span>
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



