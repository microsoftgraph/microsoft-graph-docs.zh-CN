---
title: iosDeviceType 资源类型
description: 包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 522ca687f9169066575d1bd8fb3db1e4345d9981
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52755600"
---
# <a name="iosdevicetype-resource-type"></a><span data-ttu-id="dd7cb-103">iosDeviceType 资源类型</span><span class="sxs-lookup"><span data-stu-id="dd7cb-103">iosDeviceType resource type</span></span>

<span data-ttu-id="dd7cb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd7cb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd7cb-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd7cb-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd7cb-106">包含移动应用可以在上面运行的可能的 iOS 设备类型的属性。</span><span class="sxs-lookup"><span data-stu-id="dd7cb-106">Contains properties of the possible iOS device types the mobile app can run on.</span></span>

## <a name="properties"></a><span data-ttu-id="dd7cb-107">属性</span><span class="sxs-lookup"><span data-stu-id="dd7cb-107">Properties</span></span>
|<span data-ttu-id="dd7cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd7cb-108">Property</span></span>|<span data-ttu-id="dd7cb-109">类型</span><span class="sxs-lookup"><span data-stu-id="dd7cb-109">Type</span></span>|<span data-ttu-id="dd7cb-110">Description</span><span class="sxs-lookup"><span data-stu-id="dd7cb-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd7cb-111">iPad</span><span class="sxs-lookup"><span data-stu-id="dd7cb-111">iPad</span></span>|<span data-ttu-id="dd7cb-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd7cb-112">Boolean</span></span>|<span data-ttu-id="dd7cb-113">应用是否应该在 iPad 上运行。</span><span class="sxs-lookup"><span data-stu-id="dd7cb-113">Whether the app should run on iPads.</span></span>|
|<span data-ttu-id="dd7cb-114">iPhoneAndIPod</span><span class="sxs-lookup"><span data-stu-id="dd7cb-114">iPhoneAndIPod</span></span>|<span data-ttu-id="dd7cb-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="dd7cb-115">Boolean</span></span>|<span data-ttu-id="dd7cb-116">应用是否应该在 iPhone 和 iPod 上运行。</span><span class="sxs-lookup"><span data-stu-id="dd7cb-116">Whether the app should run on iPhones and iPods.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dd7cb-117">关系</span><span class="sxs-lookup"><span data-stu-id="dd7cb-117">Relationships</span></span>
<span data-ttu-id="dd7cb-118">无</span><span class="sxs-lookup"><span data-stu-id="dd7cb-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="dd7cb-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="dd7cb-119">JSON Representation</span></span>
<span data-ttu-id="dd7cb-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd7cb-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosDeviceType"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosDeviceType",
  "iPad": true,
  "iPhoneAndIPod": true
}
```




