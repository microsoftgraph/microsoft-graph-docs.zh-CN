---
title: iosHomeScreenApp 资源类型
description: 表示主屏幕上应用的图标
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b6e4934565255e364012eedb54044b37281c1641
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32564132"
---
# <a name="ioshomescreenapp-resource-type"></a><span data-ttu-id="bed61-103">iosHomeScreenApp 资源类型</span><span class="sxs-lookup"><span data-stu-id="bed61-103">iosHomeScreenApp resource type</span></span>

> <span data-ttu-id="bed61-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bed61-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bed61-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bed61-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bed61-106">表示主屏幕上应用的图标</span><span class="sxs-lookup"><span data-stu-id="bed61-106">Represents an icon for an app on the Home Screen</span></span>


<span data-ttu-id="bed61-107">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span><span class="sxs-lookup"><span data-stu-id="bed61-107">Inherits from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="bed61-108">属性</span><span class="sxs-lookup"><span data-stu-id="bed61-108">Properties</span></span>
|<span data-ttu-id="bed61-109">属性</span><span class="sxs-lookup"><span data-stu-id="bed61-109">Property</span></span>|<span data-ttu-id="bed61-110">类型</span><span class="sxs-lookup"><span data-stu-id="bed61-110">Type</span></span>|<span data-ttu-id="bed61-111">说明</span><span class="sxs-lookup"><span data-stu-id="bed61-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bed61-112">displayName</span><span class="sxs-lookup"><span data-stu-id="bed61-112">displayName</span></span>|<span data-ttu-id="bed61-113">String</span><span class="sxs-lookup"><span data-stu-id="bed61-113">String</span></span>|<span data-ttu-id="bed61-114">继承自 [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md) 的应用的名称</span><span class="sxs-lookup"><span data-stu-id="bed61-114">Name of the app Inherited from [iosHomeScreenItem](../resources/intune-deviceconfig-ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="bed61-115">bundleID</span><span class="sxs-lookup"><span data-stu-id="bed61-115">bundleID</span></span>|<span data-ttu-id="bed61-116">String</span><span class="sxs-lookup"><span data-stu-id="bed61-116">String</span></span>|<span data-ttu-id="bed61-117">应用的 BundleID</span><span class="sxs-lookup"><span data-stu-id="bed61-117">BundleID of app</span></span>|

## <a name="relationships"></a><span data-ttu-id="bed61-118">关系</span><span class="sxs-lookup"><span data-stu-id="bed61-118">Relationships</span></span>
<span data-ttu-id="bed61-119">无</span><span class="sxs-lookup"><span data-stu-id="bed61-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="bed61-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bed61-120">JSON Representation</span></span>
<span data-ttu-id="bed61-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bed61-121">Here is a JSON representation of the resource.</span></span>
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





