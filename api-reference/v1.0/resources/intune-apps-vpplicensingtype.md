---
title: vppLicensingType 资源类型
description: 包含 iOS 批量采购程序 (Vpp) 许可类型的属性。
ms.openlocfilehash: 4e02cc4ee100fe9fa6be0eb116cff18e343fd8ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008349"
---
# <a name="vpplicensingtype-resource-type"></a><span data-ttu-id="37de2-103">vppLicensingType 资源类型</span><span class="sxs-lookup"><span data-stu-id="37de2-103">vppLicensingType resource type</span></span>

> <span data-ttu-id="37de2-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="37de2-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37de2-105">包含 iOS 批量采购程序 (Vpp) 许可类型的属性。</span><span class="sxs-lookup"><span data-stu-id="37de2-105">Contains properties for iOS Volume-Purchased Program (Vpp) Licensing Type.</span></span>
## <a name="properties"></a><span data-ttu-id="37de2-106">属性</span><span class="sxs-lookup"><span data-stu-id="37de2-106">Properties</span></span>
|<span data-ttu-id="37de2-107">属性</span><span class="sxs-lookup"><span data-stu-id="37de2-107">Property</span></span>|<span data-ttu-id="37de2-108">类型</span><span class="sxs-lookup"><span data-stu-id="37de2-108">Type</span></span>|<span data-ttu-id="37de2-109">说明</span><span class="sxs-lookup"><span data-stu-id="37de2-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37de2-110">supportsUserLicensing</span><span class="sxs-lookup"><span data-stu-id="37de2-110">supportsUserLicensing</span></span>|<span data-ttu-id="37de2-111">布尔值</span><span class="sxs-lookup"><span data-stu-id="37de2-111">Boolean</span></span>|<span data-ttu-id="37de2-112">程序是否支持用户许可类型。</span><span class="sxs-lookup"><span data-stu-id="37de2-112">Whether the program supports the user licensing type.</span></span>|
|<span data-ttu-id="37de2-113">supportsDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="37de2-113">supportsDeviceLicensing</span></span>|<span data-ttu-id="37de2-114">布尔值</span><span class="sxs-lookup"><span data-stu-id="37de2-114">Boolean</span></span>|<span data-ttu-id="37de2-115">程序是否支持设备许可类型。</span><span class="sxs-lookup"><span data-stu-id="37de2-115">Whether the program supports the device licensing type.</span></span>|

## <a name="relationships"></a><span data-ttu-id="37de2-116">关系</span><span class="sxs-lookup"><span data-stu-id="37de2-116">Relationships</span></span>
<span data-ttu-id="37de2-117">无</span><span class="sxs-lookup"><span data-stu-id="37de2-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37de2-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="37de2-118">JSON Representation</span></span>
<span data-ttu-id="37de2-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37de2-119">Here is a JSON representation of the resource.</span></span>
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



