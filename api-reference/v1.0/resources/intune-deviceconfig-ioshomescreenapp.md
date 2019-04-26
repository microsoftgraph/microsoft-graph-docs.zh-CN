---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 67c11096414db0dccad2ccf56ec184a4e3f30397
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32554735"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="06749-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="06749-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="06749-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="06749-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="06749-105">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="06749-105">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="06749-106">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="06749-106">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="06749-107">属性</span><span class="sxs-lookup"><span data-stu-id="06749-107">Properties</span></span>
|<span data-ttu-id="06749-108">属性</span><span class="sxs-lookup"><span data-stu-id="06749-108">Property</span></span>|<span data-ttu-id="06749-109">类型</span><span class="sxs-lookup"><span data-stu-id="06749-109">Type</span></span>|<span data-ttu-id="06749-110">说明</span><span class="sxs-lookup"><span data-stu-id="06749-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="06749-111">displayName</span><span class="sxs-lookup"><span data-stu-id="06749-111">displayName</span></span>|<span data-ttu-id="06749-112">String</span><span class="sxs-lookup"><span data-stu-id="06749-112">String</span></span>|<span data-ttu-id="06749-113">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="06749-113">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="06749-114">bundleID</span><span class="sxs-lookup"><span data-stu-id="06749-114">bundleID</span></span>|<span data-ttu-id="06749-115">String</span><span class="sxs-lookup"><span data-stu-id="06749-115">String</span></span>|<span data-ttu-id="06749-116">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="06749-116">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="06749-117">关系</span><span class="sxs-lookup"><span data-stu-id="06749-117">Relationships</span></span>
<span data-ttu-id="06749-118">无</span><span class="sxs-lookup"><span data-stu-id="06749-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="06749-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="06749-119">JSON Representation</span></span>
<span data-ttu-id="06749-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="06749-120">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosHomeScreenApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenApp",
  "displayName": "String",
  "bundleID": "String"
}
```



